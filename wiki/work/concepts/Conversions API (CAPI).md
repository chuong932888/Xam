---
type: concept
tags: [facebook, tracking, capi, pixel, analytics, paid-media, data]
created: 2026-05-09
updated: 2026-05-09
sources: ["[[Khối 4 - Chiến lược Facebook Fanpage]]"]
---

# Conversions API (CAPI)

## Khái niệm

**Conversions API (CAPI)** là hệ thống tracking phía máy chủ (server-side) của Meta, cho phép doanh nghiệp gửi dữ liệu sự kiện chuyển đổi **trực tiếp từ server** đến hệ thống quảng cáo của Meta, thay vì thông qua trình duyệt của người dùng.

Nói đơn giản:
- **Pixel (Facebook Pixel)**: đặt code trên website, đo từ phía trình duyệt người dùng
- **CAPI**: backend của doanh nghiệp gửi dữ liệu trực tiếp về Meta API

## Tại sao CAPI quan trọng (vấn đề Pixel không giải quyết được)

### iOS ATT — vấn đề cốt lõi

Từ iOS 14.5 (2021), Apple triển khai **App Tracking Transparency (ATT)** — yêu cầu người dùng cấp phép trước khi app/trình duyệt theo dõi hành vi. Phần lớn người dùng iOS **từ chối cấp phép**.

Kết quả:
- Pixel chạy trên Safari (iOS) bị **chặn hoàn toàn** hoặc bị giới hạn nghiêm trọng
- Dữ liệu chuyển đổi từ thiết bị iOS không về Meta → hệ thống học sai, tối ưu sai
- Ước tính: **20-40% conversion** bị mất nếu chỉ dùng Pixel

### CAPI bypass được vì sao?

CAPI không chạy trong trình duyệt — nó chạy trên **server của doanh nghiệp**. Khi người dùng thực hiện hành động (mua hàng, điền form, đăng ký), server của doanh nghiệp ghi nhận sự kiện và gửi về Meta API — **không phụ thuộc vào cài đặt quyền riêng tư của trình duyệt hay thiết bị**.

## So sánh Pixel vs. CAPI

| Đặc điểm | Pixel (Client-side) | CAPI (Server-side) |
|---|---|---|
| Nơi chạy | Trình duyệt người dùng | Server của doanh nghiệp |
| Bị iOS ATT ảnh hưởng | Có — bị chặn/giới hạn | Không — bypass hoàn toàn |
| Bị adblocker ảnh hưởng | Có | Không |
| Độ trễ dữ liệu | Gần như real-time | Có thể có độ trễ (thường < 1 giờ) |
| Dễ setup | Dễ (copy-paste code) | Phức tạp hơn — cần backend dev |
| Dữ liệu phong phú | Giới hạn | Có thể gửi nhiều parameter hơn |

**Thực hành tốt nhất: dùng CẢ HAI song song** — Pixel cho real-time data, CAPI bù đắp phần bị mất.

## Lợi ích đo được

**Dữ liệu từ Meta Q4 2025:**
- Dùng CAPI kết hợp với Pixel: tăng **+24% incremental conversions** so với chỉ dùng model attribution tiêu chuẩn
- CPL giảm khi hệ thống được nuôi đủ dữ liệu để học chính xác hơn

**Lợi ích cụ thể:**
1. **Hệ thống học chính xác hơn** — machine learning có đủ dữ liệu để tối ưu
2. **Thoát learning phase nhanh hơn** — đủ 50 sự kiện/tuần dễ hơn
3. **Attribution chính xác hơn** — biết được campaign nào thực sự tạo ra chuyển đổi
4. **Event match quality cao hơn** — Meta khớp được sự kiện với đúng người dùng

## Cách setup CAPI

**Cần có:**
- Một backend server (website có server-side code — Node.js, PHP, Python...)
- Quyền truy cập vào Meta Business Manager
- Developer hoặc kỹ thuật viên setup

**Các bước cơ bản:**

1. **Lấy Access Token** từ Meta Business Manager → Settings → System Users
2. **Cài đặt Meta Business SDK** vào backend (có SDK cho Python, PHP, Node.js, Ruby, Java)
3. **Map sự kiện** — mỗi khi user thực hiện hành động (mua, đăng ký, xem trang...) → backend gửi event tương ứng về CAPI
4. **Test với Events Manager** — dùng Test Event Tool trong Meta Business Suite để kiểm tra dữ liệu về đúng chưa
5. **Đặt Event Deduplication** — vì Pixel và CAPI đều gửi event, cần gắn `event_id` giống nhau để Meta không đếm 2 lần

**Các sự kiện quan trọng cần setup (theo thứ tự ưu tiên cho TPCN):**

| Sự kiện | Khi nào gửi |
|---|---|
| `PageView` | Mỗi khi user vào trang |
| `ViewContent` | Khi xem trang sản phẩm TPCN |
| `AddToCart` | Thêm sản phẩm vào giỏ |
| `InitiateCheckout` | Bắt đầu thanh toán |
| `Lead` | Điền form / để lại số điện thoại |
| `Purchase` | Hoàn thành mua hàng (kèm giá trị đơn) |

## Giải pháp không cần code (nếu chưa có dev)

Nếu chưa có backend developer, có các lựa chọn thay thế:

| Giải pháp | Công cụ | Phù hợp khi |
|---|---|---|
| **Shopify** | Shopify tích hợp CAPI sẵn | Bán hàng qua Shopify |
| **WooCommerce plugin** | Facebook for WooCommerce | Website WordPress + WooCommerce |
| **Google Tag Manager (GTM) Server-side** | GTM + CAPI connector | Có GTM, cần giải pháp middle-ground |
| **Zapier/Make.com** | CAPI connector qua automation | Lead form đơn giản (không phải purchase) |

> Cho TPCN VN giai đoạn đầu: nếu dùng landing page đơn giản và form Messenger/Zalo, tối thiểu cần setup CAPI cho sự kiện `Lead` (khi form được submit).

## Áp dụng cho TPCN — bắt buộc từ ngày 1

**CAPI là hạ tầng bắt buộc, không phải tuỳ chọn.**

Lý do cụ thể cho TPCN:
- TPCN bán cho phụ nữ 30-55 tuổi — tệp này dùng iPhone nhiều → iOS conversion bị chặn nặng nếu chỉ dùng Pixel
- Lead gen (để lại số điện thoại) là mục tiêu chính → sự kiện `Lead` phải về Meta chính xác để tối ưu CPL
- Nếu thiếu CAPI, hệ thống máy học của Meta tối ưu sai tệp người dùng → scale không được

**Ưu tiên setup:**

```
Ngày 1-7: Setup Pixel (nhanh, làm trước)
Ngày 7-14: Setup CAPI cho sự kiện Lead và Purchase (quan trọng nhất)
Ngày 14-30: Kiểm tra Event Match Quality trên Events Manager — mục tiêu score ≥ 7/10
Sau đó: Tối ưu deduplication, thêm các sự kiện phụ (ViewContent, AddToCart)
```

**Tích hợp với CRM:**
CAPI nên gửi thêm dữ liệu từ CRM về Meta — ví dụ: khi lead trong CRM trở thành khách hàng trả tiền (offline conversion), gửi sự kiện `Purchase` về CAPI. Điều này giúp Meta tối ưu tìm thêm người có khả năng mua cao.

**Liên kết:** [[Machine Learning Window (Meta)]] | [[Blended MER]] | [[Partnership Ads & Whitelisted Creator]] | [[Khối 4 - Chiến lược Facebook Fanpage]]
