---
type: source
tags: [ips, khoi-14, ads, youtube, video, ptl]
created: 2026-05-09
updated: 2026-05-09
sources: ["[[raw/Đặc sản của Phạm Thành Long/IPS - 19 khối công việc/14_ ADS Các nền tảng/ADS YOUTUBE.docx]]"]
khoi: 14
---

# Khối 14d — ADS YouTube

> Sub-page của [[Khối 14 - ADS Các nền tảng]]. File gốc 391 dòng, citation-heavy với 77 footnote Google Help + Think with Google.

## ⚠️ Lỗi phát hiện trong gốc

- **Dòng 302** có ký tự Hebrew "בלבד" (nghĩa "only/duy nhất") chen giữa câu tiếng Việt — typo nhiễu trong gốc. Em chuẩn hoá thành "duy nhất".
- **Dòng 96** lệch giữa Help docs và Advertising Policies về non-skippable in-stream >30s — gốc tự cảnh báo. Khi triển khai lấy **Policies + trạng thái phê duyệt thực tế** làm chuẩn.
- **Dòng 95**: từ tháng 10/2025, cột "Views" trong Google Ads đổi tên thành "TrueView views" — chỉ đổi tên, không đổi cách tính tiền. Em không xác minh độc lập được mốc này, anh tự kiểm tra.
- **Dòng 108**: GA4 import có thể default ở Secondary — gốc dùng từ "có thể" hơi mơ hồ; em giữ nguyên sắc thái không xác nhận tuyệt đối.
- **Tài liệu KHÔNG dùng tên cụ thể "ABCD framework" của Google** — chỉ nhắc "5 giây đầu" + nghiên cứu Think with Google. Em không bịa thêm.

## 🎯 TL;DR

**Quảng cáo YouTube không phải "bấm nút trong UI"** — phải đi theo chuỗi: mục tiêu kinh doanh → tín hiệu chuyển đổi → kiến trúc tracking → loại campaign → audience → creative → bidding → đo lường → tối ưu. **Sai một mắt xích là sai cả hệ thống.**

**Bản đồ sản phẩm hiện tại**:
- **Video campaigns**: awareness + consideration.
- **Demand Gen**: conversion từ video / social-style inventory (thay thế "Video Action Campaign" cũ).
- **Performance Max**: all-channel, conversion đa kênh, ít kiểm soát hơn.
- **App campaigns**: app installs.

**3 nguyên tắc ngân sách**:
1. Ngân sách tháng ≈ daily × **30,4**.
2. Hệ thống có thể **overdeliver tới 2× daily** nhưng không vượt **30,4× tổng tháng**.
3. **Demand Gen + tCPA cần ngân sách ngày ≥ 15× target CPA** để máy học đủ data.

**Đo lường 3 lớp**:
- **Click conversion** — nhấp rồi convert.
- **Engaged-view conversion** — xem ≥10s skippable hoặc ≥5s in-feed/Shorts rồi convert (NẰM TRONG cột Conversions).
- **View-through conversion** — chỉ thấy không tương tác (chủ yếu reporting).

**Last click attribution sẽ đánh giá thấp YouTube** — phải dùng **data-driven attribution**.

**5 giây đầu quyết định** có được xem tiếp không.

## 🧭 Mục lục (theo gốc)

1. Tóm tắt điều hành (dòng 2-8)
2. Khung tư duy nền tảng — công thức 9 bước (dòng 9-12)
3. Mục tiêu chiến dịch + KPI — bảng 5 mục tiêu (dòng 13-44)
4. Bảng 7 định dạng quảng cáo (dòng 45-94)
5. Cơ chế đấu thầu, ngân sách, phân bổ (dòng 97-100)
6. Targeting + audience + remarketing (dòng 101-104)
7. Thiết lập dữ liệu + tracking (dòng 105-116)
8. Quy trình thực thi từ số không (dòng 117-156)
9. Công thức + SOP 10 giai đoạn (dòng 157-223)
10. Luồng tư duy quyết định + phân bổ chi phí + funnel mẫu (dòng 224-232)
11. Kỹ thuật nâng cao (dòng 233-249)
12. 8 sai lầm + benchmark + tài nguyên + 3 bước làm ngay (dòng 250-302)

## 🧱 Phần 1+2 — Tóm tắt + Khung tư duy

### Công thức gốc 9 bước (gốc dòng 11)

```
Mục tiêu kinh doanh → conversion event đúng → tracking → 
campaign type → audience theo nhiệt độ → creative → 
bidding → attribution → tối ưu từng tầng
```

### 3 thiếu sót gây hỏng hệ thống (gốc dòng 12)

1. **Thiếu conversion architecture** → kênh xem-view rẻ nhưng không doanh thu.
2. **Thiếu audience architecture** → remarketing quá hẹp/quá rộng.
3. **Thiếu measurement architecture** → tắt quảng cáo tốt, giữ quảng cáo xấu.

## 🎯 Phần 3 — 5 mục tiêu chiến dịch + KPI (bảng dòng 14-44)

| Mục tiêu | Campaign type khuyên | KPI chính | Lưu ý |
|---|---|---|---|
| **Awareness** | Video Reach + bumper / Target Frequency / Masthead | Reach, CPM, frequency, ad recall lift | 5s đầu vẫn quyết định recall |
| **Consideration** | Video Views (in-feed + skippable + Shorts) | View rate, watch time, CTR | Thumbnail + tiêu đề mạnh |
| **Lead Gen** | Demand Gen + offline conversions | CPL qualified, lead-to-sale rate | Phải có CRM nối ngược |
| **E-commerce** | Demand Gen prospecting + remarketing nóng + PMax/dynamic | CPA, ROAS, AOV | Cần feed sạch nếu PMax |
| **App Installs** | App campaign for installs → for engagement | CPI, cost per in-app event | Subtype theo giai đoạn |

## 🎬 Phần 4 — 7 format quảng cáo (bảng đầy đủ dòng 45-94)

| Định dạng | Mục tiêu mạnh nhất | Cách mua | Khi nên dùng | Lưu ý |
|---|---|---|---|---|
| **Skippable in-stream** | Awareness, consideration, remarketing, đôi khi conversion | tCPV, tCPM, hoặc theo subtype | Cần kể chuyện >6s, vừa reach vừa học intent | 5s đầu yếu = bị skip |
| **In-feed video** | Consideration cao hơn awareness | Đi cùng mục tiêu views/consideration | Thumbnail + tiêu đề mạnh | Creative yếu thumbnail = không ai bấm |
| **Shorts ads** | Reach, consideration, social-style discovery | Trong Video Views, Demand Gen, PMax, App | Có vertical video nhanh, hook mạnh, nhịp nhanh | Cut ngang lên dọc thường kém |
| **Bumper** | Awareness, nhắc nhớ, **echo remarketing** | tCPM | Thông điệp cực ngắn, tăng reach + ad recall | KHÔNG giải thích offer dài |
| **Non-skippable in-stream** | Awareness, message completion | tCPM / reservation | Cần chắc chắn nhận trọn thông điệp | **>30s trong auction KHÔNG được phép** |
| **Ad sequence** | Storytelling, education, launch | tCPM khuyến nghị | Dẫn người xem qua chuỗi thông điệp | **KHÔNG hỗ trợ keyword/topic/placement targeting** |
| **Masthead** | Massive reach cho launch lớn | Reservation CPM hoặc CPH | Launch, rebrand, event lớn | Không dành cho ngân sách nhỏ |

### Lưu ý đặc biệt sau bảng (gốc dòng 95-96)

- **Tháng 10/2025**: cột "Views" → "**TrueView views**" — chỉ đổi tên, không đổi cách tính tiền.
- **Non-skippable in-stream >30 giây trong auction là KHÔNG được phép** theo Advertising Policies — khi Help docs lệch với Policies, lấy Policies + trạng thái phê duyệt thực tế làm chuẩn.

## 💰 Phần 5 — Bidding + Ngân sách + Phân bổ

### Bidding strategies (gốc dòng 98)

| Strategy | Tối ưu gì |
|---|---|
| **tCPV** | TrueView views |
| **tCPM** | Reach/impressions; với ad sequence còn tối ưu sequence completion |
| **tCPA, Maximize conversions, tROAS, Maximize conversion value** | Conversion / value |
| **Target Frequency** | Brand awareness — đạt tần suất tuần/tháng mục tiêu |

### 3 nguyên tắc ngân sách (gốc dòng 99-100)

1. **Ngân sách tháng ≈ daily × 30,4** (daily KHÔNG phải hard cap).
2. **1 ngày có thể tiêu tới 2× daily**, tổng tháng KHÔNG vượt 30,4× daily.
3. **Demand Gen + tCPA: ngân sách ngày ≥ 15× target CPA**.

→ Nếu chưa đủ: bắt đầu bằng **Maximize conversions** hoặc **shallow conversion** (view content / add-to-cart / lead form start) làm tín hiệu phụ — KHÔNG ép purchase ngay.

## 🎯 Phần 6 — Audience + Remarketing

### 4 tầng nhiệt độ (gốc dòng 102, 130)

- **Cold** (chưa biết)
- **Warm** (xem video / vào site)
- **Hot** (vào sản phẩm / add-to-cart / form start)
- **Customer/CRM** (đã có dữ liệu)

**Cohort thời gian**: 1-7, 8-30, 31-90, **91-540 ngày**.

### Loại audience YouTube (gốc dòng 102)

Demographics, detailed demographics, affinity, life events, in-market, **custom segments** (cũ: custom intent/affinity), **your data segments**, **Customer Match**.

### Logic AND/OR (gốc dòng 103, 236)

- Nhiều audience criteria → mặc định **OR**.
- Audience giao demographic → **AND**.
- Muốn AND giữa 2 audience khác loại → dùng **Combined segments**.
- Quá nhiều targeting method đồng thời → impressions bị hạn chế mạnh.

### Điều kiện remarketing YouTube (gốc dòng 104, 116)

- Link YouTube ↔ Google Ads.
- Video + kênh đủ điều kiện personalized advertising.
- List status: **Open**.
- Tối thiểu **100 active users / 30 ngày**.
- **YouTube users list: thời hạn lưu thành viên tối đa 540 ngày**.
- Pre-fill tối đa 30 ngày gần nhất.
- ⚠️ **Bumper ads + non-skippable in-stream KHÔNG dùng tạo YouTube users list theo logic remarketing chuẩn**.
- Shorts ads trong Video Views: yêu cầu xem đủ lâu mới đủ điều kiện remarketing.

### Checklist 6 bước chẩn đoán list = 0 (gốc dòng 116)

1. ☐ Đã link YouTube với Google Ads chưa?
2. ☐ Đã bật data collection chưa?
3. ☐ Video không "made for kids" / nội dung nhạy cảm?
4. ☐ List status Open chưa?
5. ☐ Đủ 100 active users chưa?
6. ☐ Membership duration đã hết chưa?

## 🔌 Phần 7 — Tracking + Đo lường

### Nguyên tắc vàng (gốc dòng 107)

> **"Không cài đo lường xong thì không bật ngân sách."**

**4 lớp tối thiểu**: GTM + GA4 + Google tag/Google Ads conversion + link Google Ads ↔ GA4.

### 2 đường tạo conversion (gốc dòng 108)

- Tạo trực tiếp từ Google tag/Google Ads.
- Import từ GA4 events/key events.

⚠️ GA4 import **có thể default ở Secondary** → phải đổi sang **Primary** nếu dùng cho bidding.

### Auto-tagging bắt buộc cho (gốc dòng 109)

- Import GA4 conversions.
- Đo offline conversions bằng GCLID.

### 3 loại Conversion — định nghĩa CHÍNH XÁC (gốc dòng 110-112)

| Loại | Định nghĩa | Cột báo cáo |
|---|---|---|
| **Click conversion** | Nhấp rồi convert | Conversions |
| **Engaged-view conversion (EVC)** | Xem **≥10 giây với skippable in-stream** HOẶC **≥5 giây với in-feed + Shorts** rồi convert | **Conversions + All conversions** |
| **View-through conversion (VTC)** | Impression không tương tác rồi convert | **All conversions only** (KHÔNG nằm trong Conversions) |

**VTC ngoại lệ**: App campaigns, Demand Gen tối ưu VTC, PMax store goals — VTC nằm trong Conversions.
**VTC bị hạn chế bởi cross-site cookie blocking.**

→ Chi tiết: [[3 loại Conversion Click-Engaged-View-View-Through]].

### Data-Driven Attribution (gốc dòng 113)

Mọi conversion action đều đủ điều kiện DDA. Phân phối credit cho cả **clicks + video engagements** trên Search/Shopping/YouTube/Display/Demand Gen.

### Lỗi creative phổ biến (gốc dòng 115)

Video private/unavailable, file format sai, tracking pixel sai SSL, video/kênh tắt personalized ads → mất earned action reports + data segments.

## 🚀 Phần 8 — Quy trình thực thi từ số không

### Thiết lập tài khoản (gốc dòng 118-121)

- Tạo Google Ads → billing → **link YouTube qua Data Manager**.
- Kênh creator khác: dùng link video / **Brand Partner Access**.
- GTM: tạo account + container → nhập Google tag ID.
- GA4: tạo property + web data stream → lấy Measurement ID → xác nhận Realtime.
- CMS: dùng native integration; không có CMS → dùng GTM.
- Link GA4 ↔ Google Ads tại **Product links / Google Ads links** → bật chia sẻ data + audiences.
- Tạo conversion: Goals → Create conversion action → quét domain → kiểm Primary/Secondary.

### Audience tối thiểu cho account mới (gốc dòng 122-130)

- Website visitors 30 ngày.
- Viewed product/service page 30 ngày.
- Add to cart / begin checkout / form start.
- Purchasers / qualified leads.
- **YouTube users**: đã xem video, đã subscribe, đã truy cập kênh, đã xem 1 video cụ thể.
- **Customer Match** từ email/phone được phép.
- Cohort theo nhiệt độ: 1-7, 8-30, 31-90, 91-540 ngày.
- **Local business**: location hoạt động theo **giao cắt** với remarketing list — target HN + remarketing list = chỉ thành viên nằm trong HN.

### Cấu trúc chiến dịch — nguyên tắc (gốc dòng 132-138)

- 1 campaign = **1 mục tiêu chính + 1 conversion logic**.
- 1 ad group = **1 luận điểm audience chính**.
- 1 cụm creative = **1 lời hứa giá trị chính**.
- 1 conversion goal chính / campaign.
- **Đừng gom awareness/lead/sale/app vào 1 campaign.**

### Mẫu cấu trúc 5 mục tiêu (gốc dòng 139-144)

| Mục tiêu | Cấu trúc khuyến nghị |
|---|---|
| **Awareness** | 1 Video Reach campaign, broad + in-market/affinity nhẹ, mix skippable + bumper hoặc target frequency |
| **Consideration** | 1 Video Views campaign, in-feed + skippable + Shorts |
| **Lead gen** | 1 Demand Gen tối ưu conversion, 1-2 ad groups theo audience nóng/ấm, **import qualified lead bằng offline conversions nếu có CRM** |
| **E-commerce** | 1 Demand Gen prospecting + 1 remarketing nóng + 1 PMax hoặc dynamic remarketing với feed |
| **App installs** | App campaign for installs → for engagement khi có user base |

### Khung kịch bản video (gốc dòng 147-150)

```
0-5s:    Hook (móc chú ý)
5-15s:   Problem / Promise
15-30s:  Proof (bằng chứng, demo, testimonial, kết quả)
Cuối:    CTA rõ ràng
```

→ Chi tiết: [[5s Hook + Khung kịch bản video]].

### Sản xuất asset tối thiểu (gốc dòng 152)

- **Tỷ lệ khung hình**: horizontal **16:9** + vertical **9:16** + square **1:1**.
- HD nếu có.
- Nội dung quan trọng trong **safe zone** (tránh bị che bởi overlays/UI).
- Thumbnail + companion banner khi cần.
- **PMax + Shorts**: chủ động upload video asset thay vì để hệ thống tự tạo từ ảnh+text; **ít nhất 1 vertical video 10-60 giây** giúp đủ điều kiện Shorts trong PMax.

### A/B Testing đúng (gốc dòng 153-156)

- Chỉ đổi **1 biến/lần**.
- **Video experiments**: cho Video campaigns.
- **Demand Gen A/B experiments**: cho Demand Gen.
- Demand Gen test được: creative, audience, bidding, product feed; **KHÔNG nên test budget làm biến chính**.

### Đọc báo cáo 3 tầng (gốc dòng 155)

| Tầng | Chỉ số |
|---|---|
| **Media** | Spend, reach, CPM, TrueView views, view rate, CTR |
| **Response** | Engaged-view conv, click conv, view-through conv, cost/conv |
| **Business** | Qualified lead rate, purchase rate, ROAS, pipeline/revenue offline |

→ Dừng ở media → tối ưu video dễ xem; dừng ở click → giết upper funnel.

### Scaling (gốc dòng 156)

- KHÔNG scale từ 1-2 ngày đẹp.
- Awareness scale theo **reach + frequency lành mạnh**.
- Lead gen + e-commerce scale theo **cost/qualified result hoặc ROAS**.
- Ưu tiên mở rộng từ **creative thắng + audience thắng** → mới đến ngân sách.
- **PMax**: dùng **channel performance report**.

## 🧮 Phần 9 — Công thức + SOP 10 giai đoạn

### 3 công thức số quan trọng nhất (gốc dòng 185-188)

1. Ngân sách tháng ≈ daily × **30,4**.
2. Conversion/ngày ≈ daily ÷ target CPA (lập kế hoạch thô).
3. Demand Gen + tCPA: daily **≥ 15× tCPA**?

### SOP 10 giai đoạn (gốc dòng 190-222)

| Giai đoạn | Việc | Đúng | Sai |
|---|---|---|---|
| **Nền tảng** | Tạo Google Ads, billing, link YouTube + GA4 | Đã link, thấy quyền/data source | Chưa link YouTube mà định remarketing video |
| **Tracking** | GTM + Google tag + GA4 stream + test realtime | GA4 realtime + Google tag nhận event | Bật chiến dịch khi chưa thấy data |
| **Conversion** | Tạo web conversions / import GA4, xác Primary/Secondary | Conversion bidding là Primary | Import xong vẫn Secondary |
| **Audience** | Lists web + YouTube users + Customer Match, tách 1-7/8-30/31-90 | Audience có mục đích rõ | Mọi người vào chung 1 list |
| **Cấu trúc** | 1 campaign / 1 mục tiêu / 1 conversion logic | Awareness/lead/sale riêng | Trộn nhiều mục tiêu trong 1 campaign |
| **Creative** | ≥3 tỷ lệ + hook 5s + CTA rõ | Asset đa định dạng, hợp phễu | 1 video ngang chạy mọi nơi |
| **Thí nghiệm** | Chỉ thay 1 biến | Test 2 creative cùng audience | Đổi audience + bid + creative cùng lúc |
| **Launch QA** | Policy + list Open + conversion test ghi nhận | Conversion test + audience đủ điều kiện | Launch khi list = 0 |
| **Báo cáo** | Media → response → business | Có cả view + engaged-view + offline quality | Chỉ CPM hoặc chỉ last click |
| **Scale** | Creative thắng + audience thắng → ngân sách | Mở rộng theo dữ liệu | Tăng mạnh ngân sách khi chưa ổn định |

## 🧠 Phần 10 — Luồng quyết định + Phân bổ

### Flowchart luồng quyết định campaign type (gốc dòng 225)

```
Awareness:
  - Reach rộng       → Video Reach
  - Tần suất rõ      → Target Frequency
  - Launch lớn       → Masthead

Consideration:
  - Chủ động bấm xem → Video Views (in-feed)
  - Chạm nhiều lần   → Skippable + Shorts + Bumper
  - Kể chuyện nhiều bước → Ad Sequence

Lead gen:
  - Có CRM           → Demand Gen + offline conversion
  - Chưa có CRM      → Demand Gen + lead conversion online

E-commerce:
  - Có feed          → Demand Gen + feed + remarketing
  - Có feed + cần all-channel → Performance Max + video assets
  - Không feed       → Demand Gen video/image + web remarketing

App installs:
  - Install          → App campaign for installs
  - In-app action/value → App campaign tCPA / tROAS
```

### Phân bổ ngân sách e-commerce mẫu (gốc dòng 227-229)

> ⚠️ **KHÔNG phải benchmark chính thức** — chỉ là pie chart minh hoạ của tác giả.

- Prospecting video / Demand Gen lạnh: **50%**
- Remarketing 8-30 ngày: **20%**
- Remarketing nóng 1-7 ngày / bỏ giỏ: **15%**
- Creative test: **10%**
- Dự phòng + mở rộng audience thắng: **5%**

### Funnel mẫu (gốc dòng 230-232)

> ⚠️ **KHÔNG chuẩn ngành** — chỉ minh hoạ cách đọc.

```
100,000 impressions
→ 25,000 TrueView views
→ 1,500 website visits
→ 180 leads / add-to-cart
→ 45 qualified leads / purchases
→ 12 sales giá trị cao
```

→ Báo cáo đúng: **impressions → views → visits → micro-conversions → business outcomes**.

## 🚀 Phần 11 — Kỹ thuật nâng cao

### Custom Segments (cũ: custom intent / custom affinity — gốc dòng 235)

Tạo bằng **keywords + URLs + apps** liên quan nhu cầu mua hàng. Hữu ích cho performance advertisers.

### Combined Segments (gốc dòng 236)

Công cụ chính thống cho **intersection AND** giữa các loại audience khác.
**Cảnh báo**: dùng quá nhiều targeting method đồng thời → impressions bị hạn chế mạnh.

### Customer Match (gốc dòng 237)

Re-engage trên **Search/Shopping/Gmail/YouTube/Display**.

Chia thành nhóm: **mua gần đây / mua giá trị cao / lead chưa chốt / khách ngủ đông** → message khác nhau.

### Frequency Capping + Sequencing (gốc dòng 238-241)

- **Video campaigns**: frequency capping cấp campaign theo impressions, views, hoặc cả hai.
- ⚠️ **Demand Gen: KHÔNG hỗ trợ frequency capping** → cần kiểm soát reach/frequency chặt thì giữ Video campaign riêng.
- **Target Frequency** (gốc dòng 240): nhập tần suất mong muốn theo tuần/tháng. Lưu ý: KHÔNG dùng shared budget, KHÔNG hoạt động với Google Video Partners, contextual targeting không hỗ trợ.
- **Video ad sequence**: kể chuyện theo thứ tự; tăng ad recall khi phối skippable + bumper theo "introduce/reinforce/echo"; **không cho target keywords/topics/placements** — chỉ audience + demographics cấp campaign.

### Bidding Automation, Rules, Scripts (gốc dòng 242-245)

- Đặt đúng objective trước → giao máy học.
- ⚠️ **Demand Gen: click-based bidding KHÔNG dùng để tối ưu conversion efficiency** — phải dùng **tCPA, tROAS, Maximize conversions, Maximize conversion value**.
- Goal sâu (purchase) có thể để 1 goal nông hơn ở **non-biddable** để hỗ trợ learning ban đầu.
- **Automated Rules** — điều kiện đơn giản (no-code).
- **Google Ads Scripts** — JavaScript trong IDE Google Ads, kể cả manager scripts cho nhiều account.

**Ứng dụng thực chiến**:
- Cảnh báo spend tăng nhưng conversion không vào.
- Dừng asset group khi landing hỏng.
- Email khi list remarketing tụt ngưỡng.
- Đẩy báo cáo channel mix hàng ngày.

### Enhanced Conversions for Leads (gốc dòng 247) — BẢN NÂNG CẤP

- Bản nâng cấp của offline conversion import.
- Dùng **first-party data hashed** → tăng độ chính xác bidding + đo engaged-view conv + cross-device conv tốt hơn.
- Vẫn nên **lưu GCLID**.
- Upload quá muộn → KHÔNG nhập được.

### Dynamic Remarketing trên YouTube (gốc dòng 248)

⚠️ **Native dynamic remarketing chủ yếu thuộc Display + PMax + App campaigns** — KHÔNG phải Video campaign chuẩn YouTube.

Muốn YouTube-first → dùng **Demand Gen + product feed** hoặc **PMax + video assets/feed**.

### Performance Max (gốc dòng 249)

- All-channel, tối ưu chuyển đổi/value toàn inventory Google (gồm YouTube).
- Cần tracking tốt + conversion goal rõ + asset đủ + feed tốt.
- Trade-off: ít kiểm soát.
- **Channel performance report** cho PMax → biết YouTube đóng góp gì.
- ⚠️ Học nghề video, test storytelling, sequencing, kiểm soát frequency tay → Video/Demand Gen được thiết kế chủ đích là **không thay thế được** bởi PMax.

## 🚨 Phần 12 — 8 sai lầm + Benchmark + 3 bước làm ngay

### 8 sai lầm phổ biến (gốc dòng 251-255)

1. **Chạy trước, đo sau** → khoá quy trình: chỉ launch khi có conversion test + audience test + xác nhận data vào.
2. **Chọn sai campaign type** (Video campaign cho app installs, hoặc awareness KPI chấm lead gen) → map lại từ business goal sang campaign type + bid strategy.
3. **Target quá hẹp** vì chồng audience + location hẹp + placement hẹp → hiểu logic AND/OR + Combined segments + kiểm location cắt audience.
4. **Không import offline conversions cho lead gen** → tối ưu lead rác nhưng CPL đẹp → enhanced conversions for leads hoặc GCLID-based import.
5. **Đánh giá video chỉ bằng last click** → quan sát đủ click + engaged-view + view-through → chọn attribution phù hợp.
6. **Creative không có hook 5 giây đầu** hoặc 1 asset ngang cho mọi bề mặt (đặc biệt Shorts) → cấu trúc creative theo phễu + đa tỷ lệ khung hình.
7. **List remarketing = 0 không biết vì sao** → checklist 6 bước.
8. **Để PMax tự tạo video kém chất lượng** rồi đổ lỗi cho YouTube → upload video assets chủ động.

### KPI mẫu theo ngành (gốc dòng 257-278)

⚠️ **Benchmark công khai theo ngành cho YouTube KHÔNG đồng nhất** — thay đổi mạnh theo quốc gia, format, inventory, attribution, độ rộng target, chất lượng creative.

→ **30 ngày đầu KHÔNG ép so với benchmark thị trường** — xây baseline nội bộ theo từng tầng phễu.

### 3 giới hạn (gốc dòng 297-298)

1. Benchmark công khai YouTube không đồng nhất.
2. Một số tính năng (Brand Lift, Conversion Lift, Masthead reservation) phụ thuộc tính đủ điều kiện tài khoản hoặc hỗ trợ Google.
3. Google Help đôi khi mô tả khác nhau giữa các trang về format/inventory → ưu tiên policy hiện hành + trạng thái khả dụng thực tế.

### 3 bước làm ngay (gốc dòng 299-302)

1. **Dựng hệ đo lường chuẩn trước**: GA4 realtime + Google Ads conversion test + auto-tagging bật + conversion bidding là Primary + YouTube link Google Ads. **Thiếu 1 → chưa được bật ngân sách**.
2. **Tách audience theo nhiệt độ + thời gian**: tối thiểu cold/warm/hot/customer; warm-hot có cohort 1-7, 8-30, 31-90 ngày; YouTube list đủ điều kiện. **Mọi người chung 1 list hoặc list = 0 → chưa được scale**.
3. **Test đơn giản nhưng sạch**: 1 campaign = 1 mục tiêu, 1 experiment = 1 biến; báo cáo đọc đủ CPM/views/engaged-view conv/business outcome. **Đổi nhiều thứ + chấm bằng last click → chưa tối ưu, chỉ đoán**.

## 💬 Trích dẫn

> "Học theo chuỗi nguyên nhân — không phải bấm nút trong giao diện." *(dòng 3)*

> "Không cài đo lường xong thì không bật ngân sách." *(dòng 107)*

> "5 giây đầu quyết định bạn có được xem tiếp không." *(dòng 7)*

> "Bạn chưa tối ưu — bạn chỉ đang đoán." *(dòng 302)*

## 🔗 Liên kết

- [[Khối 14 - ADS Các nền tảng]] — page mẹ
- [[3 loại Conversion Click-Engaged-View-View-Through]] — đặc thù Video/Display
- [[5s Hook + Khung kịch bản video]] — creative chuẩn
- [[Smart Bidding (Google)]] — bidding chung Google ecosystem
- [[Quality Score vs Ad Rank]] — khái niệm Google
- [[Khung diagnose phễu]] — đọc 3 tầng media-response-business
- [[Khối 14b - ADS Google]] — Google Ads ecosystem cùng platform
- [[Khối 3 - Chiến lược YouTube]] — organic YouTube để bồi paid
