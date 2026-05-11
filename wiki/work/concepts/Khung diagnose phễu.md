---
type: concept
tags: [ads, diagnose, funnel, kpi, ips, khoi-14]
created: 2026-05-09
updated: 2026-05-09
sources: ["[[Khối 14a - ADS Facebook]]", "[[Khối 14e - Phân tích chỉ số ads]]"]
---

# Khung diagnose phễu — Triệu chứng → Nguyên nhân → Hành động

> **Định nghĩa thẳng** *(theo PTL — Khối 14a dòng 208-215 + 14e dòng 426-447)*: Khi hiệu suất ads xấu, KHÔNG đoán mò. Đọc theo **thứ tự CPM → CTR → LPV rate → CVR → CPA/CPL/ROAS**. Mỗi bậc tương ứng 1 vấn đề cụ thể. Đọc cụm chứ không đọc lẻ.

## 🎯 Nguyên tắc cốt lõi

**Đọc cụm — không đọc lẻ.**

Vd: CTR 3% (cao) trông tốt → nhưng nếu CR 0.1% → có lỗi landing page.
Vd: CPC 5K (thấp) trông rẻ → nhưng nếu Frequency 6 → tệp đã cháy, sắp tăng giá.

→ Mỗi chỉ số chỉ có nghĩa khi đặt cạnh chỉ số khác.

## 📊 Bảng 6 cụm triệu chứng phổ biến nhất

> Gộp từ Khối 14a (Meta) + Khối 14e (chung 4 nền tảng).

| # | Triệu chứng | Nguyên nhân khả dĩ | Hành động |
|---|---|---|---|
| 1 | **CPM cao + CTR thấp** | Tệp KH cạnh tranh, target sai, creative không phù hợp | Đổi tệp / mở rộng audience, làm lại creative |
| 2 | **CTR cao + CR thấp** | Trang đích chậm, không khớp QC, UX kém, giá không hấp dẫn | Tối ưu landing page, tăng tốc trang, đồng bộ thông điệp |
| 3 | **CR cao + CPA cao** | CPC quá đắt, từ khoá/đối tượng đắt mà giá trị đơn hàng thấp | Tối ưu Quality Score, đổi từ khoá rẻ hơn, tăng AOV |
| 4 | **Frequency >5 và CR giảm** | Tệp đã "cháy" (saturated) | Đổi creative, mở rộng tệp, tạm tắt và quay lại sau |
| 5 | **Impression Share thấp** *(Google)* | Ngân sách hạn chế hoặc Ad Rank thấp | Tăng ngân sách hoặc tăng Quality Score |
| 6 | **View Rate thấp** *(YouTube)* | Hook đầu video không thu hút, video quá dài | Làm lại 5s đầu, rút ngắn video còn 15-20s |

## 🔍 Đọc theo bậc — quy trình 5 bước (gốc 14a dòng 208-215)

### Quy tắc: ĐỌC TỪNG TẦNG, không nhảy

```
┌─────────────────────────────────────────┐
│ Tầng 1: CPM         (Awareness)         │
│   ↓                                     │
│ Tầng 2: CTR         (Click attraction)  │
│   ↓                                     │
│ Tầng 3: LPV rate    (Landing page)      │
│   ↓                                     │
│ Tầng 4: CVR         (Conversion)        │
│   ↓                                     │
│ Tầng 5: CPA/CPL/ROAS (Business outcome) │
└─────────────────────────────────────────┘
```

### Bậc 1 — CPM cao bất thường?

**Nguyên nhân**:
- Audience cạnh tranh (peak season, ngách hot).
- Creative thiếu hấp dẫn → engagement rate thấp → bị bid up.
- Thay đổi placement (manual placement giới hạn → CPM cao hơn Advantage+).

**Hành động**:
- Mở rộng audience (broad / Advantage+).
- Thay creative.
- Bật Advantage+ Placements.

### Bậc 2 — CTR thấp?

**Nguyên nhân**:
- Hook/offer/creative kém.
- Audience sai.
- Thumbnail kém (đặc biệt YouTube/Demand Gen).

**Hành động**:
- A/B test hook (5 hook khác nhau).
- Refresh creative mỗi 2-4 tuần.
- Soát search terms (Google) → thêm negative keywords.

### Bậc 3 — LPV rate (Landing Page View) thấp dù CTR tốt?

**Nguyên nhân**:
- Landing page chậm (>2.5s mobile).
- Mismatch ad ↔ landing page (ad nói A, LP show B).
- Mobile UX kém.

**Hành động**:
- Test PageSpeed Insights → tối ưu mobile.
- Sync headline ad ↔ headline LP.
- Test mobile thật (không chỉ desktop preview).

### Bậc 4 — LPV tốt + CVR thấp?

**Nguyên nhân**:
- Offer kém (giá cao, value thấp).
- Proof yếu (thiếu testimonial, certificate, review).
- UX form/checkout kém.
- Đặt sai conversion event tracking.

**Hành động**:
- A/B test offer (giá, bonus, guarantee).
- Thêm proof (review, case study, FAQ).
- Test form rút ngắn.
- Verify conversion event bắn đúng (Pixel Helper / Test Events).

### Bậc 5 — CVR tốt + CPA cao?

**Nguyên nhân**:
- Bid strategy sai (Maximize Clicks thay vì Maximize Conversions).
- Audience đắt nhưng AOV thấp.
- Frequency quá cao (>5).
- Placement đắt (ưu tiên Audience Network thấp hơn).

**Hành động**:
- Đổi bid sang Target CPA hoặc Target ROAS.
- Loại trừ audience đắt.
- Refresh creative để giảm frequency.

## 🎯 Cụm câu hỏi đọc 3 tầng phễu

> Theo PTL Khối 14e dòng 421-425:

| Tầng | Chỉ số | Câu hỏi |
|---|---|---|
| **1 — Awareness** | Reach, Impressions, CPM, Frequency | "QC có đến đúng người không?" |
| **2 — Consideration** | CTR, CPC, View Rate, Engagement | "Họ có quan tâm không?" |
| **3 — Conversion** | CR, CPA, ROAS | "Họ có mua/đăng ký không và lời/lỗ?" |

## 📊 Đọc 3 tầng báo cáo cho YouTube/Demand Gen (gốc 14d dòng 155)

| Tầng | Chỉ số |
|---|---|
| **Media** | Spend, reach, CPM, TrueView views, view rate, CTR |
| **Response** | Engaged-view conv, click conv, view-through conv, cost/conv |
| **Business** | Qualified lead rate, purchase rate, ROAS, pipeline/revenue offline |

→ Dừng ở **media** → tối ưu video dễ xem.
→ Dừng ở **click** → giết upper funnel.
→ Đọc đến **business** mới biết campaign nào ra tiền thật.

## 🚨 5 sai lầm khi đọc số

1. **Đọc lẻ** — chỉ nhìn CTR mà không xem CR → sửa nhầm chỗ.
2. **Đánh giá quá sớm** — sau 1-2 ngày kết luận → chưa qua [[Learning Phase (50 events tuần)]].
3. **Không phân tầng** — gộp TOF/MOF/BOF vào 1 báo cáo → CPA đẹp giả vì BOF kéo lên.
4. **Last click cho YouTube** — đánh giá thấp video → tắt sai.
5. **So benchmark cứng** — benchmark VN không chuẩn hoá → tự xây baseline nội bộ.

## 🛠️ Quy trình tối ưu chuẩn 5 bước (gốc 14e dòng 449-453)

1. **Đặt KPI rõ ràng**: CPA mục tiêu, ROAS mục tiêu dựa biên LN + benchmark ngành.
2. **A/B Testing có hệ thống**: Test **1 yếu tố/lần** — không đổi nhiều thứ cùng lúc.
3. **Phân tích theo phân khúc**: Tách dữ liệu theo thiết bị, vị trí, thời gian, đối tượng.
4. **Liên tục cập nhật creative**: Đổi mới mỗi **2-4 tuần** để tránh ad fatigue.
5. **Tracking đa kênh**: GA4 + Pixel + server-side tracking cho attribution chính xác.

## 📅 Tần suất theo dõi

| Tần suất | Chỉ số |
|---|---|
| **Hàng ngày** | Clicks, CTR, CPC, Daily Cost, Impression Share |
| **Hàng tuần** | Conversions, Conversion Rate, CPA, Quality Score |
| **Hàng tháng** | ROAS, ROI, Conversion Value |

## 🎯 Hành động cho anh Chương — Team ads TPCN

📎 *Em đề xuất*:

1. **Dashboard Looker Studio** gom 4 nền tảng theo 3 tầng phễu (Media → Response → Business).
2. **Weekly meeting** sáng T2 — review mỗi cluster theo bảng 6 cụm triệu chứng.
3. **Quy tắc 1 sửa/tuần**: chỉ thay đổi 1 biến lớn/tuần (creative, audience, hoặc bid).
4. **In khung diagnose** dán cạnh bàn người chạy ads — tham chiếu nhanh khi bug.

## 🔗 Liên quan

- [[Khối 14a - ADS Facebook]] — phần 6 nguyên tắc tối ưu CPM→CTR→LPV→CVR→CPA
- [[Khối 14e - Phân tích chỉ số ads]] — bảng triệu chứng đầy đủ
- [[Learning Phase (50 events tuần)]] — không đánh giá quá sớm
- [[Quality Score vs Ad Rank]] — Impression Share thấp = QS thấp
- [[ROAS theo biên lợi nhuận]] — đặt KPI ROAS đúng
