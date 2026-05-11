---
type: concept
tags: [ads, roas, profitability, ips, khoi-14]
created: 2026-05-09
updated: 2026-05-09
sources: ["[[Khối 14e - Phân tích chỉ số ads]]"]
---

# ROAS theo biên lợi nhuận

> **Định nghĩa thẳng** *(theo PTL — Khối 14e dòng 76, 144, 207, 498-502)*: **ROAS** (Return on Ad Spend) = Doanh thu QC / Chi phí QC. **ROAS mục tiêu phụ thuộc biên lợi nhuận sản phẩm**, KHÔNG phải con số chung. Quy tắc cốt lõi: **CPA < biên LN sản phẩm** = điều kiện sống còn. **ROAS <1 = lỗ trực tiếp.**

## 🎯 Vì sao "ROAS 3x" KHÔNG có ý nghĩa nếu không biết biên LN

❌ **Sai lầm phổ biến**: "ROAS 3x là tốt" → áp dụng cho mọi ngành.

✅ **Đúng**: ROAS phụ thuộc biên LN — biên LN cao → ROAS thấp vẫn lời; biên LN thấp → ROAS cao mới hoà.

### Ví dụ minh hoạ

**Sản phẩm A — biên LN 80% (digital course)**:
- Doanh thu 10tr, ROAS 1.5× = chi 6.7tr ads → còn 10tr × 80% − 6.7tr = **+1.3tr lời**.

**Sản phẩm B — biên LN 20% (FMCG)**:
- Doanh thu 10tr, ROAS 1.5× = chi 6.7tr ads → còn 10tr × 20% − 6.7tr = **−4.7tr LỖ**.

→ Cùng ROAS 1.5× nhưng A lời, B lỗ.

## 📊 Bảng ROAS mục tiêu theo biên LN (theo PTL)

| Biên LN | Ngành | ROAS mục tiêu |
|---|---|---|
| **Thấp (15-25%)** | FMCG, retail, đồ điện tử | **>5-8×** |
| **Trung bình (40-60%)** | Thời trang, mỹ phẩm | **3-5×** |
| **Cao (70-90%)** | Digital, dịch vụ, course | **1.5-3×** đã có lãi |
| **TMĐT VN trung bình** *(gốc dòng 502, chưa cite nguồn)* | — | **2.5-4×** = tốt |

## 🧮 Công thức Break-Even ROAS

```
Break-even ROAS = 1 / Biên LN gộp × 100%
```

### Ví dụ tính toán

| Biên LN | Break-even ROAS | Diễn giải |
|---|---|---|
| 20% | 5.0× | Chi 1đ ads phải ra 5đ doanh thu mới hoà |
| 40% | 2.5× | Chi 1đ ads phải ra 2.5đ doanh thu mới hoà |
| 60% | 1.67× | Chi 1đ ads phải ra 1.67đ doanh thu mới hoà |
| **70-80% (TPCN)** | **1.25-1.43×** | Chi 1đ ads phải ra 1.3đ-1.4đ doanh thu mới hoà |

→ Trên break-even = lời. Dưới break-even = lỗ.

## 🎯 ROAS mục tiêu = Break-even × Hệ số an toàn

```
ROAS mục tiêu = Break-even ROAS × hệ số an toàn (1.5-3.0)
```

### Vì sao cần hệ số an toàn

- Chi phí khác ngoài ads (vận hành, nhân sự, kho).
- Refund + đổi trả.
- AOV biến động.
- Mất chi phí học máy ban đầu.

### Mẫu tính cho TPCN

**Giả định TPCN — biên LN 70%**:
- Break-even ROAS = 1 / 0.7 = **1.43×**.
- Hệ số an toàn 2.0× (TPCN có refund + chi phí vận hành cao):
- **ROAS mục tiêu = 1.43 × 2.0 = ~2.9×**.

→ Đặt **tROAS = 2.9×** (Smart Bidding Google) hoặc tương đương Meta/TikTok.

## 🔄 Liên hệ CPA vs ROAS

### Khi nào dùng CPA, khi nào dùng ROAS

| Dùng | Khi |
|---|---|
| **CPA mục tiêu** | Lead gen / dịch vụ — không có value đơn hàng cố định |
| **ROAS mục tiêu** | E-commerce — có value tracking, đơn hàng có giá rõ |

### Công thức CPA mục tiêu (lead gen)

```
CPA mục tiêu = Lợi nhuận gộp/sale × Tỷ lệ chốt lead→sale × Tỷ lệ NS marketing
```

**Ví dụ TPCN bán qua tư vấn dược sĩ**:
- Lợi nhuận gộp/sale: 500K
- Tỷ lệ chốt lead→sale: 30%
- Tỷ lệ NS marketing/lợi nhuận: 50%
- → CPA mục tiêu = 500K × 30% × 50% = **75K/lead**.

## 📊 ROAS theo nguồn doanh thu (đa kênh)

### Bài toán: ROAS từng kênh khác nhau

🚨 **Sửa sau QA round 2**: bảng số ROAS từng kênh em đặt trước đây (Search Brand 8-12×, YouTube 1.5-2×...) là **bịa** — KHÔNG có trong tài liệu PTL gốc và không có nguồn xác minh được. **Đã xoá**.

📎 *Em đề xuất nguyên tắc — KHÔNG có con số cụ thể*:
- **Search Brand**: thường ROAS cao nhất (bắt người đã biết brand) → đặt mục tiêu cao hơn benchmark chung.
- **Search Non-brand**: ROAS trung bình (bắt người tìm giải pháp) → benchmark chuẩn.
- **Meta Shopping/PMax**: ROAS phụ thuộc catalog + creative quality.
- **YouTube/Demand Gen**: ROAS thấp hơn (vai trò nuôi nóng) → kết hợp DDA + Engaged-view conversion để đánh giá đúng vai trò.
- **Display Remarketing**: ROAS cao nếu list nóng, target chính xác.

→ KHÔNG so ROAS giữa các kênh trực tiếp — vai trò khác nhau. **Anh phải tự đo baseline ROAS từng kênh từ data thực tế của TPCN trong 60-90 ngày đầu**, không áp benchmark trôi nổi.

→ Đo **Blended ROAS** (tổng tất cả kênh) làm KPI tổng:
```
Blended ROAS = Tổng doanh thu / Tổng spend tất cả kênh
```

## 🚨 5 sai lầm khi đặt ROAS

1. **Áp ROAS 3× cho mọi ngành** — biên LN 20% thì 3× vẫn lỗ.
2. **Tính ROAS theo last click** — đánh giá thấp upper funnel (YouTube/Display).
3. **Đặt tROAS quá cao** so với biên LN → Smart Bidding không serve được.
4. **Không tính refund/đổi trả** — ROAS gross đẹp nhưng net lỗ.
5. **Không tính LTV** — KH mua lần 2-3 → ROAS thật cao hơn ROAS lần 1.

## 🎯 LTV-based ROAS — bước nâng cao

### Khi nào dùng

- Sản phẩm có **mua lại** (TPCN, mỹ phẩm, thời trang).
- Có dữ liệu **chu kỳ mua** (ví dụ TPCN: 1 hộp = 1 tháng → mua lại sau 30-45 ngày).

### Công thức LTV (heuristic)

```
LTV = AOV × Purchase frequency × Gross margin × Customer lifespan
```

### Ví dụ TPCN

- AOV: 800K (1 combo)
- Purchase frequency: 6 lần/năm (mua hàng tháng)
- Gross margin: 70%
- Customer lifespan: 2 năm
- → **LTV = 800K × 6 × 70% × 2 = 6.72tr/khách**

→ CAC chấp nhận được = LTV × 30-50% = **2-3.4tr/khách**.

→ Nếu CPA lần đầu = 500K, chấp nhận lỗ ngắn hạn vì LTV gấp 13×.

## 🎯 Hành động cho anh Chương — TPCN

📎 *Em đề xuất*:

1. **Trước T4 (chạy ads)**: chốt **biên LN từng SKU TPCN**:
   - SKU A: 75% biên LN → ROAS mục tiêu ~2.7× (= 1/0.75 × 2.0)
   - SKU B: 60% biên LN → ROAS mục tiêu ~3.3× (= 1/0.60 × 2.0)
   - ...

2. **Setup tROAS** trong Google PMax + Meta Advantage+ Shopping theo từng SKU.

3. **Đo LTV** sau 60-90 ngày → áp dụng **LTV-based ROAS** cho campaign mua lần 1 (chấp nhận lỗ ngắn hạn).

4. **Dashboard Looker Studio** hiển thị:
   - Blended ROAS (tổng).
   - ROAS từng kênh.
   - Break-even ROAS theo SKU.
   - LTV/CAC ratio.

5. **KPI cứng cho team ads**:
   - Tháng 1-3: Blended ROAS ≥ break-even × 1.5 (đang xây funnel).
   - Tháng 4+: Blended ROAS ≥ break-even × 2.0 (ổn định).

## 🔗 Liên quan

- [[Khối 14e - Phân tích chỉ số ads]] — page mẹ
- [[Smart Bidding (Google)]] — Target ROAS strategy
- [[Khung diagnose phễu]] — đọc CPA/ROAS đúng cụm
- [[Khối 14b - ADS Google]] — Smart Bidding ROAS
- [[Khối 14a - ADS Facebook]] — Value optimization
