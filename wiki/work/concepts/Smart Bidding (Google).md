---
type: concept
tags: [ads, google, smart-bidding, ips, khoi-14]
created: 2026-05-09
updated: 2026-05-09
sources: ["[[Khối 14b - ADS Google]]"]
---

# Smart Bidding — Google Ads

> **Định nghĩa thẳng** *(theo PTL — Khối 14b)*: Smart Bidding là **bộ chiến lược đấu thầu tự động** của Google Ads dùng ML để bid theo từng auction (real-time), dựa trên dữ liệu device, location, time, audience, browser, OS, language. Quy tắc cốt lõi: **Smart Bidding KHÔNG chữa được tracking sai**. Truyền value sai → bid sai.

## 🎯 6 chiến lược Smart Bidding chính

| Chiến lược | Tối ưu cho | Khi dùng |
|---|---|---|
| **Maximize Conversions** | Số conversion (không CPA cứng) | Mới bắt đầu, chưa biết CPA mục tiêu |
| **Target CPA (tCPA)** | CPA gần mục tiêu | Đã biết CPA chấp nhận được, có ≥30 conversions/tháng |
| **Maximize Conversion Value** | Tổng giá trị conversion | E-com có value tracking rõ |
| **Target ROAS (tROAS)** | ROAS gần mục tiêu | Đã biết ROAS mục tiêu + có value tracking sạch |
| **Maximize Clicks** | Số click | Awareness/traffic giai đoạn đầu (KHÔNG cho lead/sale) |
| **Target Impression Share** | Vị trí trên SERP | Brand defense (giữ top brand keyword) |

## 🧱 4 tips Smart Bidding (gốc 14b dòng 322)

### Tip 1 — Dùng cùng account-default goals

- Phần lớn campaign dùng **cùng goal** → tận dụng **cross-campaign learning**.
- Đừng đặt goal riêng từng campaign trừ khi có lý do business cứng.

### Tip 2 — Tối ưu value, không chỉ count

- Truyền **value thật** (giá đơn hàng) qua conversion event.
- E-com KHÔNG có value tracking = Smart Bidding tối ưu mù.
- Mỗi conversion có value khác → cần tROAS hoặc Maximize Conversion Value.

→ Case **1STOPlighting**: chuyển toàn bộ Shopping sang **Target ROAS** → **profit +214%** (gốc 14b dòng 366).

### Tip 3 — Đừng đánh giá sau 2-3 ngày

- Smart Bidding cần **vài chu kỳ chuyển đổi** để học (~1-2 tuần).
- Đổi bid strategy → KHÔNG kết luận sau 2-3 ngày.
- Đổi tROAS target từ 300% → 500% → cần ít nhất 2 tuần để thấy hiệu quả mới.

### Tip 4 — Seasonality adjustments chỉ cho biến động ngắn hạn

- Dùng **Seasonality adjustments** cho:
  - Sale 3-7 ngày (vd: Black Friday).
  - Event đặc biệt (Tết, ngày 8/3, ngày 20/10).
- KHÔNG dùng để sửa **vấn đề cấu trúc dài hạn**.

## 🚦 Lộ trình tiến hoá Smart Bidding theo data

📎 *Em đề xuất khung tiến hoá — PTL gốc KHÔNG cung cấp ngưỡng số conversions/tháng cụ thể. Anh tự điều chỉnh theo data thực tế khi triển khai.*

| Giai đoạn data | Chiến lược khuyến nghị |
|---|---|
| **Mới bắt đầu** — chưa có data | Manual CPC hoặc Maximize Clicks |
| **Có baseline** — đã có conversions đều | Maximize Conversions |
| **Đã biết CPA** — có CPA chấp nhận được | Target CPA |
| **Có value tracking** — đo được giá trị đơn hàng | Maximize Conversion Value |
| **Đã biết ROAS** + value sạch | **Target ROAS** ← đỉnh cao |

## ⚠️ Smart Bidding ở Demand Gen

> Theo gốc 14d dòng 243 (YouTube/Demand Gen):

⚠️ **Click-based bidding (Maximize Clicks) KHÔNG dùng để tối ưu conversion efficiency** trên Demand Gen — phải dùng:
- tCPA
- tROAS
- Maximize Conversions
- Maximize Conversion Value

→ Demand Gen + tCPA: ngân sách ngày **≥ 15× target CPA** để đủ data học.

## 🏗️ 3 lớp bidding theo độ chín

### Lớp 1 — Highest Volume / Lowest Cost (an toàn)

- Maximize Conversions hoặc Maximize Clicks.
- Không có CPA/ROAS cứng → AI tự tối ưu.
- **Điểm bắt đầu cho người mới**.

### Lớp 2 — Cost / ROAS Goal (khi đã biết ngưỡng)

- Target CPA hoặc Target ROAS.
- Đã biết business viable ở mức nào.
- AI giữ kết quả gần goal.

### Lớp 3 — Bid Cap (dao sắc)

- Đặt trần CPC cứng.
- **Người mới hay cầm ngược** — đặt quá thấp → không phân phối; đặt quá cao → tốn tiền.
- Chỉ dùng khi đã chạy 6-12 tháng + biết rõ CPC chấp nhận được.

## 🚨 5 sai lầm Smart Bidding

1. **Tracking sai mà bật Smart Bidding** → AI học từ data sai → tối ưu sai mọi thứ. **PHẢI sửa tracking trước**.
2. **Đặt tCPA quá thấp** so với realistic → AI không đủ phân phối → ad không serve.
3. **Đổi tROAS liên tục** (mỗi tuần một số) → AI không kịp học → kết quả tệ. Đổi ≤1 lần/tháng.
4. **Trộn Primary + Secondary conversion sai** → bid theo Secondary → tối ưu nhầm hành động.
5. **Mong tROAS thay tracking** — Smart Bidding không thay được data đầu vào sạch.

## 📊 Liên hệ với Quality Score & Ad Rank

Smart Bidding **bid theo từng auction**. Auction win/lose phụ thuộc:
- Bid (Smart Bidding tự đặt)
- **Quality Score** (cần expected CTR + ad relevance + landing page experience cao)
- **Ad Rank** (bid × Quality + thresholds + context)

→ Smart Bidding chỉ tối ưu phần "bid". Quality Score + landing page phải tự lo.

→ Chi tiết: [[Quality Score vs Ad Rank]].

## 🎯 Hành động cho anh Chương — TPCN

📎 *Em đề xuất*:

| Giai đoạn | Smart Bidding |
|---|---|
| **T4 (mới launch)** | Maximize Clicks cho Search awareness; Maximize Conversions cho lead gen |
| **T5-T6 (đã có baseline conversions đều)** | Chuyển sang **Target CPA** với CPA mục tiêu = biên LN × 0.7 (an toàn) |
| **T7+ (có value tracking sạch)** | Chuyển PMax + Shopping sang **Target ROAS** mục tiêu 2.9-3.5× *(theo biên LN TPCN)* |
| **T9+ (ổn định)** | Maximize Conversion Value cho Shopping/PMax |

## 🔗 Liên quan

- [[Khối 14b - ADS Google]] — page mẹ
- [[Quality Score vs Ad Rank]] — bid không phải tất cả của auction
- [[3 loại Conversion Click-Engaged-View-View-Through]] — tracking sạch là tiền đề
- [[ROAS theo biên lợi nhuận]] — đặt tROAS đúng mức
