---
type: concept
tags: [ads, learning-phase, meta, tiktok, ips, khoi-14]
created: 2026-05-09
updated: 2026-05-09
sources: ["[[Khối 14a - ADS Facebook]]", "[[Khối 14c - ADS TikTok]]"]
---

# Learning Phase — 50 events/tuần

> **Định nghĩa thẳng** *(theo PTL — Khối 14a Facebook + 14c TikTok)*: Learning Phase là giai đoạn ad set/campaign **học để phân phối hiệu quả**. Quy tắc cứng: cần **~50 optimization events/tuần** mỗi ad set để thoát Learning Phase. Không đạt → **learning limited** → tối ưu kém.

## 🎯 Vì sao Learning Phase quyết định thành bại

Cả Meta và TikTok đều dùng **machine learning** để quyết ai thấy quảng cáo. Học cần data:
- **Quá ít data** (ad set <50 events/tuần) → hệ thống đoán mò → CPM cao, conversion thấp.
- **Đổi creative/audience/budget liên tục** trong learning → reset, học lại từ đầu.
- **Chia ad set quá nhỏ** → không ad set nào đủ 50 events/tuần → toàn bộ account learning limited.

Đây là lý do **người mới hay thất bại**: chia 10 ad set, mỗi cái 5-10 events/tuần → cả 10 đều học sai.

## 📊 Ngưỡng cụ thể từng nền tảng

| Nền tảng | Ngưỡng thoát Learning | Ngưỡng giảm biến động |
|---|---|---|
| **Meta** | **~50 optimization events/tuần** mỗi ad set | — |
| **TikTok** | **50 conversions** (dấu hiệu chính) HOẶC 7 ngày | Sau ~25 kết quả |

→ TikTok rộng rãi hơn về thời gian (7 ngày OK) nhưng vẫn cần 50 conversions để hoàn toàn thoát.

## ⚠️ 4 hành động RESET Learning Phase

Mọi thay đổi dưới đây làm ad set/campaign học lại từ đầu:

1. **Đổi audience** đáng kể (thêm/bớt segment, đổi LAL%).
2. **Đổi creative** (thay video, đổi headline chính).
3. **Đổi optimization event** (vd Purchase → AddToCart).
4. **Đổi budget mạnh** (>20-30% trong 1 lần).

→ Quy tắc PTL Meta (gốc 14a dòng 122): **không quá 30% mỗi lần**, cách nhau **~2 ngày**.
→ Quy tắc TikTok GMV Max Max delivery: **scale ~30%/ngày** OK, nhưng KHÔNG vượt **5× actual spend cũ Target ROI** trong mùa sale.

## 🎯 Cách xử lý ĐÚNG khi không đủ 50 events/tuần

⚠️ **KHÔNG mở target rộng vô tội vạ** — cách sai phổ biến.

**Cách đúng — lùi event lên gần hơn**:

| Event hiện tại | Lùi xuống | Khi nào dùng |
|---|---|---|
| Purchase | AddToCart | Site mới, traffic ít |
| Lead (form submit) | LPV (Landing Page View) | Form khó submit, ít data |
| Qualified Lead | Lead | CRM chậm phản hồi |

→ Sau khi hệ thống học tốt với event gần → quay lại event xa.

## 🏗️ 4 nguyên tắc cấu trúc account để TỐI ƯU learning

1. **Consolidate ad sets** — Meta khuyến nghị (gốc 14a dòng 216). Gộp ad set tương tự để đạt 50 events nhanh hơn.
2. **1 campaign = 1 mục tiêu rõ** — không gom awareness/lead/sale vào 1 campaign.
3. **1 ad group = 1 giả thuyết audience/offer/creative** (TikTok — gốc 14c dòng 146).
4. **3-5 creative khác biệt rõ** mỗi ad group — đa dạng trong cùng ad group thay vì nhiều ad group giống nhau.

## 🚦 Cách đọc Learning Phase status

### Meta — 3 trạng thái

| Trạng thái | Ý nghĩa | Hành động |
|---|---|---|
| **Learning** | Đang học, chưa đủ 50 events | Đợi, KHÔNG sửa |
| **Active** | Đã thoát learning | OK đọc số tối ưu |
| **Learning Limited** | Học bị giới hạn (không đủ data hoặc audience hẹp quá) | Lùi event hoặc gộp ad set |

### TikTok — 2 mode khác nhau

- **Ads Manager thủ công**: tăng budget không quá **30%/lần, cách 2 ngày**.
- **GMV Max Max Delivery**: scale **~30%/ngày** OK (nhưng KHÔNG >5× actual spend cũ).

## 📅 Quy tắc thời gian "không đụng vào"

| Tình huống | Thời gian KHÔNG sửa |
|---|---|
| Mới launch | **72h đầu**: chỉ kiểm lỗi kỹ thuật, KHÔNG đánh giá CPA/ROAS |
| Đổi bid strategy | **2-3 ngày tối thiểu** trước khi đánh giá |
| Đổi creative | Vài chu kỳ chuyển đổi (~1 tuần) trước khi kết luận |
| CBO chờ trước thay đổi lớn (TikTok) | **3 ngày HOẶC 50 conversions** (cái nào đến trước) |

## 🚨 5 sai lầm phá Learning Phase

1. **Đổi nhiều thứ cùng lúc** — không biết cái gì gây thay đổi.
2. **Đánh giá sau 1-2 ngày** — quá sớm để có data ý nghĩa.
3. **Tăng budget sốc 50-100%** — reset learning.
4. **Tắt-bật ad set** — reset learning.
5. **Nhân bản ad set giống nhau** — auction overlap (Meta) + chia loãng data.

## 🎯 Hành động cho anh Chương / team ads TPCN

📎 *Áp dụng cụ thể cho TPCN — em (agent) suy luận từ best practice*:

1. **Setup giai đoạn đầu (T4)**: với traffic TPCN còn ít, dự kiến KHÔNG đạt 50 Purchase/tuần ngay. Chuẩn bị **lùi event xuống AddToCart** hoặc **Lead** trong 1-2 tháng đầu, quay lại Purchase khi data đã dày.
2. **Cấu trúc account**: tối đa **3-5 campaign chính** (TOF/MOF/BOF + brand vs non-brand). KHÔNG vượt 10 campaign trong 90 ngày đầu.
3. **Quy tắc 1 sửa/tuần**: đặt lịch reviewer mỗi thứ 2 sáng, chỉ thay đổi **1 biến lớn/tuần** (creative, audience, hoặc budget — không cùng lúc).

## 🔗 Liên quan

- [[Khối 14a - ADS Facebook]] — phần ngân sách/scaling
- [[Khối 14c - ADS TikTok]] — phần GMV Max + bidding
- [[Pixel + CAPI + Event Deduplication]] — đếm events đúng
- [[Khung diagnose phễu]] — đọc số sau khi thoát learning
