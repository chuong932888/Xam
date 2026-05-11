---
type: concept
tags: [ads, pixel, capi, tracking, meta, tiktok, ips, khoi-14]
created: 2026-05-09
updated: 2026-05-09
sources: ["[[Khối 14a - ADS Facebook]]", "[[Khối 14c - ADS TikTok]]"]
---

# Pixel + CAPI + Event Deduplication

> **Định nghĩa thẳng**: **Pixel** = tag JavaScript ghi event từ trình duyệt. **CAPI (Conversions API)** = đường gửi event từ máy chủ. **Dedup** = cơ chế tránh đếm trùng khi cùng 1 event được gửi qua cả 2 đường. Cả Meta và TikTok đều khuyến nghị **dùng CẢ 2 song song + dedup bằng `event_id`**.

## 🎯 Vì sao cần CẢ 2 (Pixel + CAPI)?

### Pixel-only (chỉ trình duyệt)
**Vấn đề**:
- Bị **ad blocker** chặn.
- Bị **iOS 14+ ATT** giới hạn (App Tracking Transparency).
- **Cookie cross-site** đang dần biến mất (browser privacy).
- User tắt JavaScript → mất event.

→ Match rate giảm → hệ thống học sai → CPA tăng.

### CAPI-only (chỉ server)
**Vấn đề**:
- Mất event front-end (vd: button click, scroll).
- Không có trình duyệt context (cookie, fbp, fbc, ttclid).
- Setup phức tạp hơn.

### Pixel + CAPI + Dedup = trục đo lường vững nhất

- **Pixel** bắt event browser-side.
- **CAPI** bắt event server-side, vẫn về Meta/TikTok kể cả khi browser bị chặn.
- **Dedup** đảm bảo cùng 1 event không bị đếm 2 lần.

→ Kết quả: **Event Match Quality (EMQ) cao hơn** → hệ thống hiểu đúng ai mua → tối ưu chính xác.

## 🔧 Cách dedup hoạt động

### Quy tắc cứng (gốc 14a dòng 62, 14c dòng 75)

- Cùng 1 event (vd Purchase order #1234) gửi cả Pixel + CAPI.
- Phải có **`event_id`** (hoặc event name + timestamp) ở CẢ 2.
- Hệ thống dùng event đầu tiên đến, làm giàu data nếu trùng, tránh double count.

### Yêu cầu kỹ thuật

| Trường | Bắt buộc | Mô tả |
|---|---|---|
| `event_id` | ✅ | ID duy nhất cho 1 sự kiện (vd `transaction_id` hoặc UUID) |
| `event_name` | ✅ | Tên chuẩn: ViewContent, AddToCart, InitiateCheckout, Purchase, Lead |
| `event_time` | ✅ | Unix timestamp |
| `action_source` | ✅ | "website" / "app" / "physical_store" |
| User data | ✅ | email, phone (đã hash SHA-256) hoặc fbp/fbc/ttclid |

## 🏗️ 3 cách triển khai (theo độ khó)

| Cách | Tool | Phù hợp | Khó | Ưu/nhược |
|---|---|---|---|---|
| **GTM Server-side** | GTM + Cloud Run/Stape | Có dev/server | Cao | Linh hoạt nhất, tự control 100% |
| **Native CMS plugin** | Shopify, WooCommerce có sẵn module | Plugin trên CMS | Trung | Setup nhanh, ít custom |
| **Direct API integration** | Code Node.js/Python gửi POST | Custom backend | Cao | Tốn dev nhưng kiểm soát tối đa |

→ **TikTok GTM server-side** hỗ trợ flow cài đặt mặc định để tự cấu hình `event_id` deduplication (gốc 14c dòng 75).

## 📋 Standard Events bắt buộc

### Meta (gốc 14a dòng 61)

| Event | Khi nào bắn | Bắt buộc parameters |
|---|---|---|
| `ViewContent` | Xem trang sản phẩm | `content_ids, content_type, value, currency` |
| `AddToCart` | Thêm vào giỏ | `content_ids, content_type, value, currency` |
| `InitiateCheckout` | Bắt đầu thanh toán | `value, currency, num_items` |
| `Lead` | Submit form lead | `content_name, value (nếu có)` |
| `Purchase` | Hoàn tất mua | `value, currency, content_ids, content_type` |
| `CompleteRegistration` | Đăng ký tài khoản | — |

### TikTok (gốc 14c dòng 84)

| Event | Khi nào bắn | Bắt buộc parameters |
|---|---|---|
| `ViewContent` | Xem trang sản phẩm | `content_ids, content_type, value, currency` |
| `AddToCart` | Thêm vào giỏ | `content_ids, content_type, value, currency, quantity` |
| `InitiateCheckout` | Bắt đầu thanh toán | `value, currency, contents` |
| `Purchase` | Hoàn tất mua | `value, currency, contents, order_id` |

### Mapping Meta ↔ GA4 ↔ TikTok

| Funnel step | Meta | GA4 | TikTok |
|---|---|---|---|
| View product | ViewContent | view_item | ViewContent |
| Add to cart | AddToCart | add_to_cart | AddToCart |
| Begin checkout | InitiateCheckout | begin_checkout | InitiateCheckout |
| Lead | Lead | generate_lead | (custom: SubmitForm) |
| Purchase | Purchase | purchase | Purchase |
| Sign up | CompleteRegistration | sign_up | (custom: Registration) |

## 🛠️ QA tools — kiểm tra setup đúng

### Meta

| Tool | Mục đích |
|---|---|
| **Test Events Tool** (Events Manager) | Quét QR test real-time trên mobile/desktop |
| **Event Match Quality (EMQ)** | Chỉ số khớp sự kiện — mục tiêu Excellent (≥7) |
| **Diagnostics** | Phát hiện lỗi: missing parameters, deprecated events |
| **Event coverage ratio** | Server vs browser — nếu chỉ Pixel có thì EMQ thấp |
| **Pixel Helper Chrome extension** | Debug Pixel real-time |

### TikTok

| Tool | Mục đích |
|---|---|
| **Test Events** trong Event Manager | Quét QR test real-time |
| **Pixel Helper 2.0** | QA trên Chrome (gốc 14c dòng 96) |

## 📊 Event Match Quality (EMQ) — Meta

PTL gốc chỉ nói: theo dõi **Event Match Quality** trong Events Manager + diagnostics + event coverage ratio (gốc Khối 14a dòng 63, 220, 287). **KHÔNG** cung cấp thang điểm hay ngưỡng cụ thể.

📎 *Em đề xuất — KHÔNG có trong PTL gốc*: theo Meta Help, EMQ thường được Meta hiển thị dạng **Good / Great / Excellent**. Anh tự xác minh trong Events Manager → Data Sources → tab Diagnostics khi setup.

**Cách nâng EMQ** *(industry standard — không phải PTL gốc liệt kê)*:
1. Gửi nhiều **user data** đã hash: email, phone, fname, lname, city, zip, country, dob.
2. Gửi **fbp, fbc, ttclid** (browser cookies).
3. Bật **Advanced Matching**.
4. Dedup chuẩn (không gửi 2 lần khác `event_id`).

## 🚨 7 lỗi tracking phổ biến

1. **Không bật CAPI** — chỉ Pixel → match rate kém với iOS users.
2. **Dedup sai event_id** — Pixel gửi `event_id=123`, CAPI gửi `event_id=456` → đếm trùng → CPA hiển thị thấp giả.
3. **Thiếu `value` + `currency`** — không tính được ROAS, không dùng được Value Optimization.
4. **Sai `content_type`** — nên là `product` cho retail; sai → không match catalog.
5. **Pixel ở `<body>` thay vì `<head>`** — chậm bắn, có thể miss event.
6. **Submit URL có `?fbclid=` nhưng strip mất** — mất attribution.
7. **Không hash email/phone** — vi phạm policy + giảm match rate.

## 📅 Quy trình QA hàng tuần

> Đẩy vào [[Checklist QA tracking đa kênh]].

- ☐ **Hàng tuần** (sáng T2):
  - Vào Events Manager → check EMQ tất cả events (mục tiêu **Great/Excellent** theo Meta UI).
  - Test Events trên 2-3 sản phẩm.
  - So spend Meta vs purchases CRM — đối chiếu để phát hiện gap *(ngưỡng cụ thể anh tự đặt theo dữ liệu thực tế — em không bịa con số)*.
- ☐ **Hàng tháng**:
  - Audit deprecated events.
  - Cập nhật Pixel/CAPI version mới nhất.
  - Review event coverage ratio (server vs browser).

## 🎯 Hành động cho anh Chương — Setup TPCN

📎 *Em đề xuất*:

1. **Trước launch ads (T4)** — setup Pixel + CAPI cho:
   - Website TPCN (chính)
   - Landing page Squeeze ([[Khối 11 - Quy trình Squeeze Page]])
   - Sales page TPCN ([[Khối 10 - Squeeze Page]])
2. **Chọn cách triển khai**: nếu dùng Shopify/WooCommerce → native plugin trước; nếu custom → GTM server-side.
3. **EMQ mục tiêu** ở mức Great/Excellent (Meta UI) trước khi bật ngân sách lớn.
4. **Dedup `event_id`** = `transaction_id` của order (đảm bảo unique).

## 🔗 Liên quan

- [[Khối 14a - ADS Facebook]] — phần 3 hạ tầng Meta
- [[Khối 14c - ADS TikTok]] — phần 4 tracking TikTok
- [[Checklist QA tracking đa kênh]] — tool áp dụng tuần
- [[UTM template chuẩn 4 nền tảng]] — UTM bổ sung cho Pixel/CAPI
