---
type: tool
tags: [ads, tracking, qa, checklist, ips, khoi-14]
created: 2026-05-09
updated: 2026-05-09
sources: ["[[Khối 14a - ADS Facebook]]", "[[Khối 14b - ADS Google]]", "[[Khối 14c - ADS TikTok]]", "[[Khối 14d - ADS YouTube]]"]
---

# Checklist QA Tracking Đa Kênh — In Tường

> **Cách dùng**: in 1 trang, dán cạnh bàn người chạy ads. **Hàng tuần (sáng T2)** review từng mục. **Không tick đủ — không bật ngân sách >5tr/ngày.**

---

## 🔥 NGUYÊN TẮC VÀNG

> **"Không cài đo lường xong thì không bật ngân sách."** *(PTL — Khối 14d)*

---

## A. Hạ tầng tracking (kiểm 1 lần khi setup, sau đó hàng tháng)

### A1 — Meta (Facebook + Instagram)

- [ ] **Business Portfolio** verified business + verified domain.
- [ ] **Pixel** cài trong `<head>` toàn site, bắn `PageView` trên mọi trang.
- [ ] **Conversions API (CAPI)** triển khai (GTM server-side / native plugin / direct API).
- [ ] **Standard Events** đầy đủ: ViewContent, AddToCart, InitiateCheckout, Lead, Purchase, CompleteRegistration.
- [ ] **Dedup** Pixel + CAPI bằng `event_id` = `transaction_id` hoặc UUID.
- [ ] **Test Events Tool** cho thấy event bắn đúng.
- [ ] **Event Match Quality (EMQ)** ở mức **Great/Excellent** (theo Meta UI display).
- [ ] Diagnostics tab không có lỗi nghiêm trọng.
- [ ] Event Coverage Ratio: server vs browser cao *(em không bịa ngưỡng cụ thể — anh đặt theo data thực tế)*.
- [ ] Offline Events đã setup (nếu có CRM).

### A2 — Google Ads + GA4

- [ ] **Google tag** hoặc GTM cài toàn site.
- [ ] **GA4** property + web data stream + Measurement ID có data Realtime.
- [ ] **GA4 ↔ Google Ads** đã link qua Product Links / Google Ads Links.
- [ ] **Conversion actions** đã định nghĩa (tối thiểu Purchase, Lead).
- [ ] Conversion bidding là **Primary**, micro-conversions là **Secondary**.
- [ ] **Auto-tagging** đã bật.
- [ ] **GCLID** truyền đầy đủ qua URL (không bị strip).
- [ ] **Enhanced Conversions** đã bật (cho lead gen).
- [ ] **Consent Mode** triển khai (nếu có banner consent).

### A3 — TikTok

- [ ] **TikTok Pixel** base code trong `<head>`.
- [ ] **Events API** (CAPI) song song.
- [ ] **Standard Events**: ViewContent, AddToCart, InitiateCheckout, Purchase.
- [ ] Parameters: `content_ids, content_type, value, currency, quantity`.
- [ ] Dedup bằng `event_id`.
- [ ] **Test Events** trong Event Manager — quét QR test mobile.
- [ ] **Pixel Helper 2.0** không báo lỗi.
- [ ] **TikTok Shop** kết nối Business Center + 1 primary ad account cho GMV Max.

### A4 — YouTube (qua Google Ads)

- [ ] **YouTube channel** đã link Google Ads (qua Data Manager).
- [ ] **Data collection** đã bật trên kênh.
- [ ] **YouTube users list** có ≥ **100 active users / 30 ngày**.
- [ ] List status = **Open**.
- [ ] Video không "made for kids" (nếu không phải KH trẻ em).

---

## B. UTM Tracking (kiểm hàng tuần)

- [ ] **Mọi link đi web** từ ads có UTM đầy đủ.
- [ ] UTM template chuẩn (xem [[UTM template chuẩn 4 nền tảng]]).
- [ ] `utm_source` đúng (meta/google/tiktok/youtube).
- [ ] `utm_medium` đúng (paid_social/cpc/paid_video).
- [ ] `utm_campaign` theo naming convention.
- [ ] `utm_content` phân biệt creative.
- [ ] GA4 Acquisition reports thấy UTM đúng.

---

## C. Cross-domain + Cross-device

- [ ] **Cross-domain GA4** đã setup (nếu user đi domain bán → domain thanh toán).
- [ ] **Google signals** đã bật (nhận diện đa thiết bị).
- [ ] iOS users tracking OK (có CAPI fallback khi Pixel bị block).

---

## D. Privacy + Consent

- [ ] **Cookie banner** xin đồng ý hợp lệ (GDPR-style nếu có user EU).
- [ ] **Consent Mode** truyền tín hiệu đồng ý đến Meta/Google/TikTok.
- [ ] **Privacy Policy** + Terms hiển thị footer.
- [ ] User data hash SHA-256 trước khi gửi (email, phone).

---

## E. KPI Dashboard (kiểm hàng tuần)

- [ ] **Looker Studio dashboard** gom 4 nền tảng.
- [ ] 5 tab: Executive / Funnel / Creative / Audience / Diagnostics.
- [ ] So spend Meta vs purchases CRM → đối chiếu để phát hiện gap *(ngưỡng anh đặt theo baseline thực tế)*.
- [ ] So spend Google vs purchases GA4 → đối chiếu tương tự.
- [ ] Anomaly alerts đã setup (GA4 + Meta automated rules).

---

## F. Compliance (đặc biệt cho TPCN — kiểm hàng tháng)

- [ ] **Account Quality** Meta không có warning.
- [ ] **Tài khoản MXH** xác thực số ĐT VN (Nghị định 147/2024).
- [ ] **Số đăng ký Cục ATTP** hiển thị trên trang sản phẩm.
- [ ] **Disclaimer** "Sản phẩm này không phải là thuốc..." trên LP.
- [ ] **Ads từ chối** rate < 5% — nếu cao hơn, root cause analysis.

---

## G. Quy trình QA hàng tuần (sáng thứ 2)

| Việc | Tool | Thời gian |
|---|---|---|
| Check EMQ Meta tất cả events | Events Manager | 5 phút |
| Test Events 2-3 sản phẩm Meta | Test Events Tool | 10 phút |
| Test Pixel TikTok | Pixel Helper 2.0 | 5 phút |
| Check GA4 Realtime | GA4 | 5 phút |
| Đối chiếu spend vs CRM/orders | Dashboard Looker | 15 phút |
| Anomaly check 4 nền tảng | Dashboard | 10 phút |
| Reject rate ads | Meta + Google + TikTok | 10 phút |

**Tổng: ~1 giờ/tuần.**

---

## H. Quy trình QA hàng tháng (đầu tháng)

- [ ] Audit deprecated events Meta/Google/TikTok.
- [ ] Cập nhật Pixel/CAPI version mới nhất.
- [ ] Review event coverage ratio.
- [ ] Cập nhật Meta Advertising Standards mới nhất.
- [ ] Review Account Quality + AHR (TikTok).
- [ ] Backup conversion actions definition (snapshot).

---

## 🚦 Tiêu chí ĐƯỢC PHÉP scale ngân sách

| Status | Quyết định |
|---|---|
| < 80% mục tick | ⛔ KHÔNG bật ngân sách >2tr/ngày — fix trước |
| 80-95% | ⚠️ Bật ngân sách 2-5tr/ngày, fix trong 7 ngày |
| ≥ 95% | ✅ Bật ngân sách bất kỳ |

---

> **In file này, đặt cạnh bàn người chạy ads. Mỗi sáng T2 tick đủ trước khi mở Ads Manager.**

— Theo công thức [[Khối 14 - ADS Các nền tảng]] · thầy [[Phạm Thành Long]]

## 🔗 Liên quan

- [[Khối 14 - ADS Các nền tảng]]
- [[Pixel + CAPI + Event Deduplication]]
- [[UTM template chuẩn 4 nền tảng]]
- [[3 loại Conversion Click-Engaged-View-View-Through]]
