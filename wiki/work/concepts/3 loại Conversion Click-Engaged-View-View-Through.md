---
type: concept
tags: [ads, conversion, attribution, youtube, google, ips, khoi-14]
created: 2026-05-09
updated: 2026-05-09
sources: ["[[Khối 14d - ADS YouTube]]"]
---

# 3 loại Conversion — Click / Engaged-View / View-Through

> **Định nghĩa thẳng** *(theo PTL — Khối 14d dòng 110-112)*: Google Ads phân biệt **3 loại conversion** dựa trên hành vi user trước khi convert. Hiểu sai 3 loại này → đánh giá thấp/cao sai vai trò của video, Display, YouTube. **Last click attribution sẽ đánh giá thấp YouTube**.

## 📊 Bảng 3 loại — phân biệt CHÍNH XÁC

| Loại | Định nghĩa | Cột báo cáo | Áp dụng |
|---|---|---|---|
| **Click conversion** | User **NHẤP** ad rồi convert | Conversions | Search, Shopping (chính), Display |
| **Engaged-View Conversion (EVC)** | User **xem ≥10s skippable in-stream** HOẶC **≥5s in-feed/Shorts** rồi convert | **Conversions + All conversions** | YouTube Video (chính) |
| **View-Through Conversion (VTC)** | User chỉ **THẤY ad** (impression không tương tác) rồi convert | **All conversions only** *(KHÔNG nằm trong Conversions)* | Display, Video |

## 🎯 Vì sao có 3 loại?

### Vấn đề khi chỉ có Click conversion

- **YouTube/Display ads** thường KHÔNG khiến user click ngay. User xem → nhớ thương hiệu → tuần sau search Google → mua.
- Nếu chỉ đo Click conversion trên YouTube → KPI thấp giả → tắt YouTube → mất kênh thúc đẩy phễu trên.

### Engaged-View ra đời (2021+)

- Google công nhận: **xem 10s skippable** (đã qua điểm Skip) là **action có ý nghĩa** — user chủ động chọn không skip.
- **Xem 5s in-feed/Shorts** — đã chủ động vuốt và xem.
- → Tính engaged-view vào **Conversions** chính thức (không chỉ All conversions).

### View-Through dành cho ai

- Brand campaigns (awareness).
- App campaigns (cài app sau khi thấy ad).
- Demand Gen tối ưu VTC.
- PMax store goals.

→ Hầu hết campaign khác: VTC chỉ trong All conversions, **không nằm trong Conversions** (tránh bid sai).

## ⏱️ Ngưỡng giây cụ thể (gốc 14d dòng 111)

| Format | Engaged-View threshold |
|---|---|
| **Skippable in-stream** | **≥10 giây** |
| **In-feed video** | **≥5 giây** |
| **Shorts ads** | **≥5 giây** |

→ Nếu user xem 8s skippable rồi skip → **KHÔNG** tính engaged-view.

## 🚨 Hạn chế cross-site cookie blocking

VTC bị **giảm độ chính xác** do:
- Browser block third-party cookies (Safari ITP, Firefox ETP, Chrome 2024+).
- iOS 14+ ATT.

→ VTC ngày càng kém tin cậy → **đừng làm bid logic chính dựa vào VTC**.

📎 *PTL gốc YouTube nói "VTC bị hạn chế bởi cross-site cookie blocking" — KHÔNG cung cấp con số % cụ thể về mức độ giảm.*

## 📈 Cách đọc báo cáo đúng

### Cột "Conversions" trong Google Ads

```
Conversions = Click conversions + Engaged-view conversions
              (KHÔNG có VTC, trừ ngoại lệ App/Demand Gen VTC/PMax store)
```

→ **Đây là cột Smart Bidding tối ưu**.

### Cột "All conversions"

```
All conversions = Conversions + View-through conversions
```

→ Để đọc tổng quan, KHÔNG để bid.

### Cột "View-through conversions" riêng

→ Để đo tác động awareness của Display/Video.

## 🎯 Data-Driven Attribution (DDA) + 3 loại conversion

> Gốc 14d dòng 113:

- Mọi conversion action đủ điều kiện DDA.
- DDA phân phối credit cho cả **clicks + video engagements** trên Search/Shopping/YouTube/Display/Demand Gen.

→ DDA + 3 loại conversion = đo lường công bằng nhất cho video ads.

## 🚨 5 sai lầm phổ biến

### 1. Đánh giá YouTube chỉ bằng Click conversion

❌ "YouTube không ra đơn → tắt"
✅ Nhìn cả Engaged-view conversions trong cột Conversions + DDA assist credit.

### 2. Để VTC vào Smart Bidding goal

❌ Bật Maximize VTC cho campaign Search → bid sai mục tiêu
✅ VTC chỉ cho Display/Video brand awareness, KHÔNG cho Search direct response.

### 3. Tin VTC như Click conversion

❌ "Display có 1.000 VTC = 1.000 sale"
✅ VTC bị cookie blocking — số thật có thể chỉ 30-50% số hiển thị.

### 4. Không phân biệt cột Conversions vs All conversions

❌ Dùng All conversions làm KPI chính cho lead gen → bid sai
✅ Conversions = bid; All conversions = đọc tổng quan.

### 5. Last click attribution cho YouTube

❌ Last click → YouTube luôn bị 0 credit
✅ Data-Driven Attribution — chia credit công bằng cho touchpoint.

## 🏗️ Setup đúng trong Google Ads

### Bước 1 — Tạo conversion action

1. Goals → Conversions → Create conversion action.
2. Chọn category (Purchase, Lead, Sign-up...).
3. **Count**: One per click (lead gen) hoặc Every (e-commerce).
4. **Conversion windows**: setup theo Google Ads UI khuyến nghị + chu kỳ ra quyết định mua thực tế của ngành. *(Em — agent — không bịa con số mặc định; PTL gốc không cung cấp ngưỡng cụ thể cho windows.)*
5. **Attribution model**: **Data-Driven** (mặc định mới của Google Ads).

### Bước 2 — Set Primary/Secondary

| Mục tiêu | Primary | Secondary |
|---|---|---|
| **Lead gen** | `qualified_lead` (offline import) | `generate_lead` (online) |
| **E-commerce** | `purchase` | `add_to_cart`, `begin_checkout` |
| **App installs** | `app_install` | `in_app_event` |

→ **Smart Bidding chỉ tối ưu cho Primary**.

## 🎯 Hành động cho anh Chương — TPCN

📎 *Em đề xuất*:

1. **Setup conversion action** với attribution windows phù hợp chu kỳ mua TPCN (ngành ngách → click-through nên dài để cover research period). Anh tham khảo Google Ads UI khuyến nghị + adjust theo data thực tế.
2. **Attribution model**: Data-Driven Attribution (DDA).
3. **Báo cáo team** sử dụng 3 cột riêng:
   - Conversions (cho bid Smart Bidding).
   - All conversions (đọc tổng quan).
   - View-through conversions (đánh giá vai trò YouTube/Display awareness).
4. **Đừng tắt YouTube khi Click conversion = 0** trong tháng đầu — đo Engaged-view + DDA credit trước.

## 🔗 Liên quan

- [[Khối 14d - ADS YouTube]] — page mẹ
- [[Khối 14b - ADS Google]] — Click conversion chính
- [[Smart Bidding (Google)]] — bid theo Primary conversion
- [[Khối 14e - Phân tích chỉ số ads]] — view-through conversion trong bảng chỉ số
