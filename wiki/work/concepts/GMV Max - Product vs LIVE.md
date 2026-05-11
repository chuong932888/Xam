---
type: concept
tags: [ads, tiktok, gmv-max, ips, khoi-14]
created: 2026-05-09
updated: 2026-05-09
sources: ["[[Khối 14c - ADS TikTok]]"]
---

# GMV Max — Product vs LIVE

> **Định nghĩa thẳng** *(theo PTL — Khối 14c)*: GMV Max là **loại chiến dịch mặc định + duy nhất** hỗ trợ Shop Ads mới trên TikTok Shop từ **tháng 7/2025**. Chia 2 loại: **Product GMV Max** (cho sản phẩm thường ngày) và **LIVE GMV Max** (cho phiên live shopping). Triết lý: Tự động hoá toàn bộ — TikTok AI ghép sản phẩm + creative + audience.

## 🎯 Vì sao GMV Max là cuộc cách mạng cho TikTok Shop seller

Trước 7/2025: seller dùng PSA (Product Shopping Ads), VSA (Video Shopping Ads), LSA (LIVE Shopping Ads) — phải tự setup từng campaign cho từng video.

Từ 7/2025:
- **GMV Max làm hết**: tự ghép creative trong shop + organic post + ad post + creator content.
- **Tự target**: AI dùng signal của Shop (PDP view, ATC, Purchase) để tìm người mua.
- **Tự bid**: Target ROI hoặc Max Delivery, không cần đặt CPC/CPM thủ công.

→ Seller mới **dễ launch** hơn nhiều — chỉ cần creative tốt + sản phẩm/giá tốt + LIVE đều.

## 📊 So sánh Product GMV Max vs LIVE GMV Max

| | Product GMV Max | LIVE GMV Max |
|---|---|---|
| **Khi dùng** | Bán hàng video/sản phẩm thường ngày trong Shop | Shop có LIVE đều, host, lịch phát |
| **KPI chính** | Gross revenue, ROI, Orders, Cost per order | LIVE GMV, ROI, traffic vào live, đơn hàng LIVE |
| **Creative input** | Toàn bộ creative sẵn có (shop + organic + ad) | Phiên LIVE đang phát (real-time) |
| **Best practice thời lượng** | Always-on | **>3 giờ/phiên** tăng GMV nhanh hơn; **>8 giờ/ngày** mạnh hơn |
| **Campaign duration** | Always-on | **Tối thiểu 3 ngày** |
| **Phụ thuộc** | Catalog sạch + creative đa dạng | Chất lượng LIVE + lịch phát ổn định |

## 🚦 GMV Max — 2 modes (gốc 14c dòng 125-127)

### Mode 1 — Target ROI (always-on)

**Khi dùng**:
- Always-on để giữ hiệu quả.
- Sản phẩm/shop đã có baseline doanh số.

**Đặc điểm**:
- TikTok giữ ROI gần mục tiêu bạn đặt.
- ROI ổn định, scale chậm hơn.
- Dùng làm "trục chính" duy trì doanh thu.

### Mode 2 — Max Delivery (đẩy mạnh)

**Khi dùng**:
- Shop/sản phẩm mới (chưa có data Target ROI).
- Launch sản phẩm mới.
- Mùa sale (Tết, 6/6, 8/8, 11/11, 12/12).

**Best practice**:
- Khuyến nghị dùng **3-5 ngày đầu** cho shop/sản phẩm mới.
- Budget khởi điểm **≥10× AOV** (Average Order Value).
- Scale **~30%/ngày** (TikTok cho phép tăng nhanh hơn Ads Manager thủ công).
- Có data Target ROI trước → set Max delivery = actual spend cũ HOẶC **1-5× actual spend cũ TRONG MÙA KHUYẾN MÃI**.
- ⚠️ **Vượt 5× → ROI tụt mạnh.**

## 🏗️ Kiến trúc account dùng GMV Max (gốc 14c dòng 9, 36-41)

### Quy tắc cứng — 1 primary ad account

**Mỗi TikTok Shop chỉ có 1 primary ad account dùng GMV Max tại 1 thời điểm.**

⚠️ Đổi primary ad account → quyền GMV Max của tài khoản cũ **bị thu hồi** + campaign GMV Max đang chạy có thể **bị pause**.

### Kiến trúc nên dùng

```
Business Center (1 cái, gắn với shop)
├── Primary Ad Account (cho GMV Max)
├── Catalog (Shop)
├── Pixel + Events API (nếu có web song song)
└── Creative Library:
    ├── Shop product videos (organic)
    ├── Brand official account posts
    ├── Authorized creator content (Spark Ads)
    └── ACA (Affiliate Creatives for Ads)
```

## 🎬 Creative input cho GMV Max

GMV Max **tự ghép** từ 4 nguồn:

1. **Shop product video** — video gắn trong shop.
2. **Brand official TikTok account** — bài đăng organic của brand.
3. **Authorized creator content** — creator đã uỷ quyền (Spark Ads).
4. **ACA — Affiliate Creatives for Ads** — content từ affiliate đã chấp nhận.

→ **Càng nhiều creative khác biệt** → AI có nhiều input để A/B → kết quả tốt hơn.

## 📅 Roadmap GMV Max cho seller mới

### Tuần 1-2 — Setup
- ☐ Kết nối Shop ↔ Business Center ↔ Primary Ad Account.
- ☐ Chuẩn hoá PDP, giá, voucher, tồn kho.
- ☐ Sản xuất **15-30 video creative** đầu tiên (theo [[5s Hook + Khung kịch bản video]]).
- ☐ Setup audience nền (Shop Activity, custom audience).

### Tuần 3-4 — Launch Max Delivery
- ☐ Bắt đầu **Product GMV Max — Max Delivery** với budget **10× AOV**.
- ☐ Chạy 3-5 ngày — KHÔNG sửa gì trong [[Learning Phase (50 events tuần)]].
- ☐ Đạt 50 conversions → thoát learning.

### Tuần 5-8 — Chuyển sang Target ROI
- ☐ Chuyển sang **Target ROI** với mục tiêu = ROAS thực tế đã đo được × 0.9 (an toàn).
- ☐ Always-on duy trì doanh số.
- ☐ Bắt đầu tách bucket creative (hook/offer/creator/demo).

### Tuần 9-12 — Mở LIVE GMV Max
- ☐ Chuẩn hoá lịch LIVE (≥3 giờ/phiên, ≥3 ngày/tuần).
- ☐ Launch **LIVE GMV Max** gắn lịch live cố định.
- ☐ Scale Product GMV Max winner +20-30%.

## 🚨 5 sai lầm GMV Max

1. **Đổi primary ad account giữa chừng** → mất hết campaign GMV Max đang chạy.
2. **Set Max delivery budget quá thấp** (<10× AOV) → AI không đủ data học → không serve.
3. **Vượt 5× actual spend cũ Target ROI** trong mùa sale → ROI tụt mạnh.
4. **Catalog/Shop product info kém** → AI không có gì để render → impressions thấp.
5. **Không có creative đa dạng** → AI ghép giống nhau → hiệu suất giảm sau 2 tuần.

## 🎯 Áp dụng TPCN

📎 *Em đề xuất*:

| Giai đoạn | GMV Max |
|---|---|
| **T4 (TikTok Shop launch)** | Product GMV Max — Max Delivery 3-5 ngày, budget 10× AOV TPCN (vd AOV 500K → budget 5tr/ngày) |
| **T5 (đã có 50 conversions)** | Chuyển Target ROI với mục tiêu 3.0× (TPCN biên LN cao) |
| **T6+ (có host LIVE)** | Mở LIVE GMV Max với lịch ≥3 phiên/tuần, ≥3 giờ/phiên |
| **Mùa Tết / 11.11** | Tăng Max Delivery 1-3× actual spend cũ, KHÔNG vượt 5× |

⚠️ **Lưu ý quan trọng cho TPCN**: TikTok có **market rule riêng cho healthcare/pharma** ở VN. Trước launch GMV Max phải:
- Verify shop là TPCN có giấy phép.
- Nội dung video tuân Luật QC 16/2012 + Nghị định 38/2021 (xem [[Khối 14f - Từ cấm FB Ads (cảnh báo nhân viên)]] phần pháp lý VN).
- Disclaimer "Sản phẩm này không phải là thuốc..." trên video + caption.

## 🔗 Liên quan

- [[Khối 14c - ADS TikTok]] — page mẹ
- [[Learning Phase (50 events tuần)]] — 50 conversions để thoát
- [[5s Hook + Khung kịch bản video]] — creative cho GMV Max
- [[TOF-MOF-BOF Funnel + Audience Layers]] — Shop Activity audience
- [[Khối 14f - Từ cấm FB Ads (cảnh báo nhân viên)]] — pháp lý VN cho TPCN
