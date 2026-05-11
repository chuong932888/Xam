---
type: source
tags: [ips, khoi-14, ads, metrics, kpi, ptl]
created: 2026-05-09
updated: 2026-05-09
sources: ["[[raw/Đặc sản của Phạm Thành Long/IPS - 19 khối công việc/14_ ADS Các nền tảng/Phân tích chỉ số quảng cáo.docx]]"]
khoi: 14
---

# Khối 14e — Phân tích chỉ số quảng cáo

> Sub-page của [[Khối 14 - ADS Các nền tảng]]. File gốc 521 dòng — phân tích **43 chỉ số đo lường** trên 4 nền tảng + công thức + benchmark + diagnose phễu.

## ⚠️ Lỗi phát hiện trong gốc — đọc TRƯỚC khi áp dụng

1. **Công thức `CPC = CPM / (CTR × 10)`** (dòng 147) — **chỉ đúng khi CTR tính bằng % nguyên** (vd: 1.5, không phải 0.015). Bản chất gốc là `CPC = CPM / (CTR × 1000)` với CTR thập phân. Tài liệu KHÔNG giải thích điều kiện này → người đọc dễ nhầm.
2. **"Facebook 1,8 tỷ DAU"** (dòng 87) — số liệu **2020-2021**, **đã lỗi thời**. Meta DAU thực tế (FB+IG+WA) đã >**3 tỷ** từ 2024. Số 1,8 tỷ là DAU riêng FB ở mốc cũ.
3. **"Google 3,5 tỷ lượt tìm kiếm/ngày"** (dòng 162) — đây là **lượt tìm kiếm Google Search**, KHÔNG phải lượt nhấp/hiển thị quảng cáo. Cách diễn đạt dễ gây hiểu nhầm.
4. **"Tháng 10/2025 đổi tên Views → TrueView views"** (dòng 233) — em không xác minh được mốc, anh tự kiểm tra Google Ads UI.
5. **Quality Ranking / Engagement Rate Ranking / Conversion Rate Ranking** (dòng 156) — đúng về lịch sử (Meta thay 2019), nhưng **hiện chỉ hiển thị above/at/below average** chứ KHÔNG phải điểm số.
6. **Công thức `Ad Rank = Max CPC × Quality Score (cộng các yếu tố khác)`** (dòng 222) — đơn giản hoá quá. Công thức Google chính thức gồm thêm: ngưỡng Ad Rank, ngữ cảnh truy vấn, hiệu ứng dự kiến của tiện ích/định dạng.
7. **"ROAS 2,5-4× ngành TMĐT VN tốt"** (dòng 502) — KHÔNG cite nguồn cụ thể. Đánh dấu "chưa xác minh".

## 🎯 TL;DR

Cốt lõi:
1. **Chỉ số là phương tiện, lợi nhuận mới là mục đích.**
2. **Đọc theo cụm chứ không đọc lẻ** — vd CTR cao + CR thấp = lỗi landing page.
3. **Mỗi nền tảng có chỉ số đặc trưng**:
   - Google: Quality Score
   - YouTube: View Rate
   - TikTok: Engagement Rate / GMV
   - Facebook: Frequency / CTR Link

**Khung 3 bước chẩn đoán**:
- Đọc theo phễu (Awareness → Consideration → Conversion).
- Chẩn đoán cụm triệu chứng.
- Quy trình tối ưu (KPI rõ → A/B test 1 biến → phân tích phân khúc → đổi creative 2-4 tuần/lần → tracking đa kênh).

## 📊 Bảng 43 chỉ số đầy đủ

> ⚠️ Quá dài để đặt hết trong 1 bảng. Em chia 5 nhóm theo phễu để dễ tra.

### Nhóm 1 — Hiển thị (Awareness layer)

| # | Chỉ số | Định nghĩa | Công thức | Áp dụng | Ngưỡng |
|---|---|---|---|---|---|
| 1 | **Impressions** | Tổng số lần QC xuất hiện; cùng 1 người xem nhiều lần vẫn cộng | — | tất cả | — |
| 2 | **Reach** | Số người KHÔNG TRÙNG LẶP đã xem QC ít nhất 1 lần | — | FB, GG (display), YT, TT | — |
| 3 | **Frequency** | Số lần TB mỗi người thấy QC | Impressions / Reach | tất cả | ≤3 tốt; **>3-5 = cháy tệp, CR giảm** |
| 4 | **CPM** | Chi phí cho 1.000 hiển thị | (Cost / Impressions) × 1000 | tất cả | Cao đột biến → tệp cạnh tranh / peak season |
| 5 | **uCPM** | Chi phí cho 1.000 NGƯỜI tiếp cận khác nhau | — | FB | — |

### Nhóm 2 — Nhấp + Tương tác (Consideration layer)

| # | Chỉ số | Định nghĩa | Công thức | Áp dụng | Ngưỡng |
|---|---|---|---|---|---|
| 6 | **Clicks** | Tổng số nhấp vào QC | — | tất cả | — |
| 7 | **CTR** | Tỷ lệ nhấp | (Clicks / Impressions) × 100% | tất cả | (xem benchmark) |
| 8 | **CTR (All)** | CTR tính TẤT CẢ nhấp (like, comment, share, click link) | — | FB | — |
| 9 | **CTR (Link)** | CTR chỉ tính nhấp ra liên kết ngoài | — | FB | **0,6-1,5%** tốt; **<0,6%** kém |
| 10 | **CTR (Unique)** | % người duy nhất đã nhấp | Unique Clicks / Reach | FB | — |
| 11 | **CPC** | Chi phí TB cho 1 nhấp | Cost / Clicks | tất cả | Cao thường do CTR thấp hoặc Quality Score thấp |
| 12 | **CPC (Link)** | Chi phí TB cho 1 nhấp ra liên kết | — | FB | — |
| 13 | **CPC (Destination)** | Chi phí TB cho 1 nhấp dẫn đến web/app | — | TT | — |
| 14 | **Engagement Rate** | (Like+Comment+Share+Click) / Reach (FB); (Like+Comment+Share)/Reach × 100% (TT) | — | FB, TT | TT thường cao do văn hoá tương tác |
| 15 | **3s/15s Video Views** | Số người xem video ≥3s hoặc ≥15s | — | FB | — |

### Nhóm 3 — Chuyển đổi (Conversion layer)

| # | Chỉ số | Định nghĩa | Công thức | Áp dụng | Ngưỡng |
|---|---|---|---|---|---|
| 16 | **Conversions** | Hành động có giá trị (mua, đăng ký, lead, ATC, gọi…) | — | tất cả | — |
| 17 | **CR / CVR** | Tỷ lệ chuyển đổi | (Conversions / Clicks) × 100% | tất cả | Thấp → vấn đề landing page/quy trình mua |
| 18 | **CPA** | Chi phí TB cho 1 chuyển đổi | Cost / Conversions | tất cả | **< biên LN sản phẩm** |
| 19 | **Cost per Result** | Chi phí mỗi kết quả theo mục tiêu | — | FB | — |
| 20 | **ROAS** | Doanh thu QC / Chi phí QC | — | tất cả | <1 = lỗ trực tiếp |
| 21 | **ROI** | (Lợi nhuận − Chi phí) / Chi phí × 100% | — | tất cả | — |

### Nhóm 4 — Đặc trưng Google Search

| # | Chỉ số | Định nghĩa | Áp dụng | Ngưỡng |
|---|---|---|---|---|
| 22 | **Impression Share (IS)** | % lần QC hiển thị / tổng lần đủ điều kiện | GG | Cao = khai thác hết tiềm năng; Thấp → ngân sách hoặc Ad Rank thấp |
| 23 | **Top of page rate** | % lần QC xuất hiện ở đầu trang | GG | — |
| 24 | **Absolute top of page rate** | % lần QC ở vị trí #1 tuyệt đối | GG | CTR cao nhất nhưng đắt nhất |
| 25 | **Quality Score** | Điểm chất lượng từng từ khoá, thang 1-10. Cấu thành: Expected CTR + Ad Relevance + Landing Page Experience | GG | **8-10** tốt; **<5** cần tối ưu gấp |
| 26 | **Ad Rank** | Thứ hạng QC. Max CPC × Quality Score (+ yếu tố khác) | GG | — |
| 27 | **View-through Conversions** | CĐ từ người chỉ XEM (không click) QC Display/Video | GG, TT | — |

### Nhóm 5 — Đặc trưng YouTube + TikTok

| # | Chỉ số | Định nghĩa | Áp dụng | Ngưỡng |
|---|---|---|---|---|
| 28 | **Views (TrueView)** | ≥30s hoặc hết video nếu ngắn hơn, HOẶC tương tác. Shorts: ≥10s | YT | — |
| 29 | **View Rate** | Lượt xem TrueView / Số lần hiển thị | YT | **15-30%** tốt; thấp → hook đầu yếu |
| 30 | **CPV** | Chi phí TB cho 1 lượt xem TrueView | YT | Tăng → creative cũ hoặc cạnh tranh tăng |
| 31 | **Target CPV** | CPV mục tiêu nhà QC đặt ra | YT | Đặt quá thấp → không phân phối |
| 32 | **Video Played To 25/50/75/100%** | % người xem đến từng mốc | YT, TT | — |
| 33 | **Earned Actions** | View, like, share, sub trên video khác sau khi xem QC | YT | — |
| 34 | **Earned Subscribers/Likes/Shares** | Sub, like, share kênh phát sinh sau xem QC | YT | — |
| 35 | **Brand Lift** | Mức tăng nhận biết, ghi nhớ, ý định mua thương hiệu | YT | Cần Google sales rep kích hoạt |
| 36 | **Viewability** | % QC thực sự được nhìn thấy trên màn hình | YT | — |
| 37 | **Watch Time / Average Watch Time** | Thời gian TB người xem dành cho video | YT, TT | Cao → thuật toán ưu tiên |
| 38 | **Video Views (TT)** | Lượt xem từ giây đầu tiên | TT | — |
| 39 | **Paid Likes / Follows** | Like + follow phát sinh từ phiên hiển thị QC | TT | — |

### Nhóm 6 — TikTok Shop GMV

| # | Chỉ số | Định nghĩa | Áp dụng |
|---|---|---|---|
| 40 | **GMV** (Gross Merchandise Value) | Tổng giá trị giao dịch từ VSA/LSA/PSA | TT Shop |
| 41 | **Click-to-Checkout %** | % người nhấp QC đi đến trang thanh toán | TT Shop |
| 42 | **Checkout-to-Order %** | % giao dịch hoàn tất / lượt thanh toán | TT Shop |

### Nhóm 7 — Đặc trưng Facebook (đo chất lượng QC)

| # | Chỉ số | Định nghĩa | Áp dụng |
|---|---|---|---|
| 43 | **Quality / Engagement / Conversion Rate Ranking** | 3 chỉ số thay Relevance Score (Meta đổi 2019). ⚠️ Hiện hiển thị above/at/below average chứ không phải điểm số | FB |

### ⚠️ Chỉ số gốc KHÔNG có (em xác nhận để anh biết)

Tài liệu này **KHÔNG** liệt kê: **Hook rate**, **Hold rate** (chỉ nhắc gián tiếp qua "3s Video Views" + "Hook 3s đầu"), **MER**, **MROAS**, **AOV**, **LTV**, **CAC**.

## 🔍 Cách diagnose phễu — Bảng triệu chứng → nguyên nhân → hành động (gốc dòng 426-447)

| Triệu chứng | Nguyên nhân khả dĩ | Hành động |
|---|---|---|
| **CPM cao + CTR thấp** | Tệp KH cạnh tranh, target sai, creative không phù hợp | Đổi tệp / mở rộng audience, làm lại creative |
| **CTR cao + CR thấp** | Trang đích chậm, không khớp với QC, UX kém, giá không hấp dẫn | Tối ưu landing page, tăng tốc trang, đồng bộ thông điệp |
| **CR cao + CPA cao** | CPC quá đắt, từ khoá/đối tượng đắt mà giá trị đơn hàng thấp | Tối ưu Quality Score, đổi từ khoá rẻ hơn, tăng AOV |
| **Frequency >5 và CR giảm** | Tệp đã "cháy" (saturated) | Đổi creative, mở rộng tệp, tạm tắt và quay lại sau |
| **Impression Share thấp** (Google) | Ngân sách hạn chế hoặc Ad Rank thấp | Tăng ngân sách hoặc tăng Quality Score |
| **View Rate thấp** (YouTube) | Hook đầu video không thu hút, video quá dài | Làm lại 5s đầu, rút ngắn video còn 15-20s |

→ Chi tiết: [[Khung diagnose phễu]].

### Logic CPC qua công thức (gốc dòng 147-152)

⚠️ **Công thức `CPC = CPM / (CTR × 10)` chỉ đúng khi CTR ở dạng % nguyên (1.5, không phải 0.015)**.

| Triệu chứng | Hành động |
|---|---|
| CPC tăng vọt + CPM ổn định | Vấn đề CTR thấp → đổi creative |
| CPM tăng đột biến | Tệp cạnh tranh cao hoặc mùa peak (Tết, lễ) |
| Muốn giảm CPC | Giảm CPM (tệp ít cạnh tranh) HOẶC tăng CTR (creative tốt hơn) |

### Đọc 3 tầng phễu (gốc dòng 421-425)

| Tầng | Chỉ số | Câu hỏi |
|---|---|---|
| **1 — Awareness** | Reach, Impressions, CPM, Frequency | "QC có đến đúng người không?" |
| **2 — Consideration** | CTR, CPC, View Rate, Engagement | "Họ có quan tâm không?" |
| **3 — Conversion** | CR, CPA, ROAS | "Họ có mua/đăng ký không và lời/lỗ?" |

## 🧮 Công thức kinh doanh

> ⚠️ Tài liệu KHÔNG có LTV, CAC, AOV, MER, MROAS — em chỉ liệt kê những gì có trong gốc.

### 14 công thức chính thức + heuristic

1. `Frequency = Impressions / Reach`
2. `CPM = (Cost / Impressions) × 1.000`
3. `CTR = (Clicks / Impressions) × 100%`
4. `CPC = Cost / Clicks`
5. `CR (CVR) = (Conversions / Clicks) × 100%`
6. `CPA = Total Cost / Total Conversions`
7. `ROAS = Revenue / Cost`
8. `ROI = (Profit − Cost) / Cost × 100%`
9. `CPC = CPM / (CTR × 10)` *(rút gọn quan hệ — CTR % nguyên)*
10. `Ad Rank = Max CPC × Quality Score (+ yếu tố khác)` *(Google)*
11. `Engagement Rate (TT) = (Like + Comment + Share) / Reach × 100%`
12. `View Rate = TrueView Views / Impressions`
13. `CTR Unique = Unique Clicks / Reach`
14. `Engagement Rate (FB) = Tổng tương tác (like+comment+share+click) / Reach`

### Nguyên tắc cốt lõi liên quan kinh doanh (rút từ dòng 76, 144, 207, 498-502)

- **CPA < biên LN sản phẩm** = điều kiện sống còn.
- **ROAS mục tiêu phụ thuộc biên LN**:

| Biên LN | Ngành | ROAS mục tiêu |
|---|---|---|
| **Thấp** | FMCG, retail | **>5-8×** |
| **Trung bình** | Thời trang, mỹ phẩm | **3-5×** |
| **Cao** | Digital, dịch vụ | **1,5-3×** đã có lãi |
| TMĐT VN trung bình *(chưa cite nguồn)* | — | **2,5-4×** = tốt |

→ Chi tiết: [[ROAS theo biên lợi nhuận]].

📎 *Em (agent) thêm — TPCN*: TPCN VN thường thuộc nhóm **biên LN trung-cao** (gross margin 60-80%) → có thể nhắm ROAS **3-5×** ở giai đoạn đầu. Anh tự xác minh với dữ liệu thực tế khi triển khai — gốc KHÔNG cung cấp benchmark TPCN riêng.

## 📊 Benchmark theo ngành (gốc dòng 459-502)

### CTR theo nền tảng

| Nền tảng | CTR tốt | Ghi chú |
|---|---|---|
| Facebook Ads | CTR All ~0,9% (TB toàn ngành); CTR Link **0,6-1,5%** | Cao hơn: B2C/E-com. Thấp hơn: B2B, tài chính |
| Google Search | **3-5%** | Top ngành Du lịch, B2C: 5-8% |
| Google Display | **0,5-1%** | Hiếm khi vượt 2% (banner blindness) |
| Google Shopping | **2-3%** | Có hình + giá nên CTR tốt |
| YouTube Ads | View Rate **15-30%**; CTR click out **0,5-1%** | Trọng tâm là xem |
| TikTok Ads | **1-3%**, có thể đạt **5%+** với creative xuất sắc | UGC-native cho hiệu quả vượt trội |

### CPC trung bình toàn cầu

| Nền tảng | CPC TB | Ghi chú |
|---|---|---|
| Google Search | ~**2,69 USD** | Ngành đắt: bảo hiểm >50 USD, luật >40 USD |
| Google Display | ~**0,63 USD** | Rẻ hơn nhưng intent thấp |
| Facebook Ads | **0,5-2 USD** tuỳ ngành | VN thường thấp hơn |
| TikTok Ads | ~**1 USD**, có thể thấp hơn ở giai đoạn mới | Tăng dần khi cạnh tranh tăng |

## 🛠️ Quy trình tối ưu chuẩn 5 bước (gốc dòng 449-453)

1. **Đặt KPI rõ ràng**: CPA mục tiêu, ROAS mục tiêu dựa trên biên LN + benchmark ngành.
2. **A/B Testing có hệ thống**: Test **1 yếu tố/lần** (creative, headline, audience, landing page) — KHÔNG đổi nhiều thứ cùng lúc.
3. **Phân tích theo phân khúc**: Tách dữ liệu theo thiết bị, vị trí, thời gian, đối tượng.
4. **Liên tục cập nhật creative**: Đổi mới mỗi **2-4 tuần** để tránh ad fatigue.
5. **Tracking đa kênh**: GA4 + Pixel + server-side tracking để có attribution chính xác.

## 📅 Tần suất theo dõi chỉ số (gốc dòng 224-227, 514-515)

| Tần suất | Chỉ số |
|---|---|
| **Hàng ngày** | Clicks, CTR, CPC, Daily Cost, Impression Share |
| **Hàng tuần** | Conversions, Conversion Rate, CPA, Quality Score |
| **Hàng tháng** | ROAS, ROI, Conversion Value |

## 📐 Tối ưu theo nền tảng (rút gọn)

### Tối ưu YouTube (gốc dòng 285-290)

- Thông điệp chính trong **5-10 giây đầu** để tránh skip.
- Video càng ngắn → View Rate càng cao. Cắt 30s → 20s nếu giữ được thông điệp.
- View Rate tăng → CPV giảm tự nhiên.
- CTA rõ ràng đặt cả trong video và overlay.
- Theo dõi 7-10 ngày đầu, điều chỉnh theo: **Lượt xem, CTR, CPV, View Rate, Conversion Rate**.

### Tối ưu TikTok (gốc dòng 369-375)

- 3 yếu tố cốt lõi cải thiện CPM/CTR: **Audience + Creative + Ad Score**.
- Tái sử dụng nội dung từ creator/KOL/UGC → tăng tin cậy & Engagement Rate.
- **Hook 3 giây đầu** quyết định người xem dừng hay vuốt qua.
- CPM cao ở: tài chính, BĐS, bảo hiểm.
- Kiểm tra TikTok Pixel **hàng tuần** để đảm bảo tracking không lỗi.
- ROAS TikTok không phản ánh đúng nếu không tích hợp dữ liệu đa kênh.

### Tối ưu Facebook (gốc dòng 153-157)

- Comment & Inbox **không phải đơn hàng** — chi phí trên ĐƠN HÀNG mới quyết định.
- Frequency >3 với tệp nhỏ → giá QC tăng vọt sau ngày 2-3 ("cháy tệp").
- Conversion tracking chính xác cần **Meta Pixel + Conversions API**.

## ⏱️ Thời gian học thuật toán theo nền tảng (gốc dòng 411-415)

| Nền tảng | Thời gian học |
|---|---|
| TikTok | **3-5 ngày** (nhanh nhất) |
| Facebook | **3-7 ngày** |
| Google | **7-14 ngày** |
| YouTube | **7-14 ngày** |

## 🎯 So sánh "phù hợp nhất cho" (gốc dòng 406-410)

| Nền tảng | Phù hợp ngành |
|---|---|
| Facebook | E-com, B2C, retargeting |
| Google | Dịch vụ địa phương, B2B, lead-gen |
| YouTube | Branding, ra mắt sản phẩm |
| TikTok | FMCG trẻ, fashion, beauty |

## 🎓 5 khuyến nghị thực hành cuối tài liệu (gốc dòng 513-518)

1. **Xây dashboard tổng hợp** (Looker Studio) để theo dõi tất cả nền tảng cùng lúc.
2. Theo dõi tần suất phù hợp (đã ghi ở trên).
3. **Đầu tư vào creative** — phần lớn vấn đề CTR/CPC bắt nguồn từ chất lượng nội dung, không phải target.
4. **A/B test có hệ thống** — mỗi lần 1 biến, đủ ngân sách + thời gian (>3-7 ngày) để có ý nghĩa thống kê.
5. **Đa kênh**: Search (intent cao) + Social (khám phá) + Video (branding) — không bỏ trứng vào 1 giỏ.

## 💬 Trích dẫn

> "Chỉ số là phương tiện, không phải mục đích." *(dòng 508)*

> "Đọc cụm, không đọc lẻ." *(dòng 509)*

> "Tracking là nền tảng." *(dòng 511)*

> "Benchmark là tham chiếu, không phải KPI." *(dòng 512)*

> "CPA phải nhỏ hơn biên lợi nhuận sản phẩm." *(dòng 76)*

## 🔗 Liên kết

- [[Khối 14 - ADS Các nền tảng]] — page mẹ
- [[Khung diagnose phễu]] — bảng triệu chứng → nguyên nhân → hành động
- [[ROAS theo biên lợi nhuận]] — quyết ngưỡng có lãi
- [[Quality Score vs Ad Rank]] — đặc thù Google
- [[3 loại Conversion Click-Engaged-View-View-Through]] — chi tiết VTC vs EVC vs Click
- [[Checklist QA tracking đa kênh]] — tool áp dụng tuần
