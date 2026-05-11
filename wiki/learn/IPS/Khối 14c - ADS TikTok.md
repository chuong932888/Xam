---
type: source
tags: [ips, khoi-14, ads, tiktok, gmv-max, ptl]
created: 2026-05-09
updated: 2026-05-09
sources: ["[[raw/Đặc sản của Phạm Thành Long/IPS - 19 khối công việc/14_ ADS Các nền tảng/ADS TIKTOK.docx]]"]
khoi: 14
---

# Khối 14c — ADS TikTok

> Sub-page của [[Khối 14 - ADS Các nền tảng]]. File gốc 395 dòng, 8 phần + 70 footnote.

## ⚠️ Lỗi phát hiện trong gốc

- **5 footnote case study gắn SAI hoàn toàn** (Edikted [60], Very [62], American Eagle [64], Baseus [66], Haus Von Albe [68]) — số trích dẫn lệch khỏi nguồn thực tế trong reference. **Kết quả con số case vẫn chính xác** nhưng URL footnote sai chỗ.
- **Số budget tối thiểu 50 USD/20 USD** áp dụng tài liệu TikTok Ads Manager quốc tế — **VN có thể có ngưỡng nội tệ khác**. Anh tự xác minh khi setup.
- **Mâu thuẫn nội bộ về scale 30%/ngày** (dòng 122 vs 127): 2 quy tắc khác nhau cho 2 mode khác nhau (Ads Manager thủ công vs GMV Max Max delivery). Em đã làm rõ ngữ cảnh.
- **Bảng kịch bản ngân sách "Bão hoà"** (dòng 144) câu "1-5× actual spend under Target ROI" mất ngữ cảnh "trong mùa khuyến mãi" — em đã thêm lại.
- **Lộ trình Gantt có ngày cụ thể** (2026-05-01 đến 2026-06-20+) — đây là **ví dụ minh hoạ**, KHÔNG phải kế hoạch cố định.

## 🎯 TL;DR

**Từ tháng 7/2025, GMV Max là loại chiến dịch mặc định + duy nhất hỗ trợ cho Shop Ads mới** trên TikTok Shop. Người mới phải học theo thứ tự: **mục tiêu kinh doanh → dữ liệu đo lường → creative → cấu trúc chiến dịch → remarketing → scale**.

**Bán trong Shop**: Product GMV Max hoặc LIVE GMV Max.
**Bán về website**: Sales/Conversions + Pixel + Events API.

**Creative là biến số số một**, broad audience thắng over-segmentation, scale chỉ khi đã qua [[Learning Phase (50 events tuần)|Learning Phase]] (50 conversions hoặc 7 ngày).

**Quy tắc tối thượng**: tối ưu từ "đường đi mua hàng", không phải từ "Ads Manager".

## 🧭 Mục lục 8 phần (theo gốc)

1. **Executive summary** — 4 đoạn tổng quan.
2. **Bản đồ hệ thống** — 3 lớp + 5 lựa chọn chiến lược + kiến trúc tài khoản.
3. **Tư duy chiến lược + KPI** — funnel, KPI tầng, công thức funnel.
4. **Kiến trúc dữ liệu, tracking, audience** — Pixel/CAPI, checklist tracking, UTM, 4 nhóm audience.
5. **Thiết kế chiến dịch + ngân sách + bidding** — cấu trúc 3 tầng, bidding, GMV Max mode.
6. **Creative + A/B test + 10 kịch bản** — TikTok-first, Spark Ads, template video.
7. **Remarketing + tối ưu + scaling** — 4 cửa sổ remarketing, sequencing, automated rules, Gantt 90 ngày.
8. **Chính sách + 6 case studies + lộ trình 30/60/90** — Ad Policies, SPS/AHR, 3 bước làm ngay.

## 🧱 Phần 1+2 — Tư duy + Bản đồ hệ thống

### 5 câu hỏi quyết định (gốc dòng 6)

1. Đang bán cho ai?
2. Đang kéo họ đi từ bước nào sang bước nào?
3. Creative nào hợp với bước đó?
4. Event nào dùng để tối ưu?
5. KPI nào quyết định giữ hay cắt?

### 3 lớp hệ thống (gốc dòng 8)

| Lớp | Tên | Vai trò |
|---|---|---|
| 1 | **TikTok Shop / Seller Center** | Quản shop, sản phẩm, tồn kho, affiliate, Account Health, Shop Performance Score |
| 2 | **TikTok Ads Manager** | Campaign, ad group, ad, audience, bidding, split test, automated rules, reporting |
| 3 | **Data layer** | TikTok Shop native signals, TikTok Pixel, Events API, UTM, GA4 |

### Quy tắc cứng — primary ad account (gốc dòng 9)

**Mỗi TikTok Shop chỉ có 1 primary ad account dùng GMV Max tại 1 thời điểm.** Đổi primary ad account → quyền GMV Max của tài khoản cũ bị thu hồi, campaign GMV Max đang chạy có thể bị pause.

### Kiến trúc tài khoản nên dùng (gốc dòng 36-41)

- 1 **Business Center** gắn với shop.
- 1 primary ad account cho GMV Max.
- Thư viện creative từ: account chính thức + business account + tài khoản được uỷ quyền + Spark Ads post + ACA (Affiliate Creatives for Ads).
- Có website → tách chiến dịch website vào luồng Ads Manager riêng với Pixel + Events API + UTM.

### Quy ước đặt tên (khuyến nghị tác giả, KHÔNG phải quy định TikTok — gốc dòng 42)

```
VN | Shop | Product GMV Max | Serum A | Always-on
VN | Web | Sales | ATC | Broad | UGC Set 1
```

## 🎯 Phần 3 — Tư duy + KPI

### Sai lầm: lấy targeting làm chiến lược

Đúng: chiến lược nằm ở **mục tiêu kinh doanh + hành trình mua**.

### TikTok objective 3 nhóm

- **Awareness**: Reach.
- **Consideration**: Traffic, Video Views, Engagement, Lead Generation.
- **Conversion**: Sales (Web Conversions, App Promotion), Shop.

### KPI theo tầng funnel

| Đích | KPI |
|---|---|
| TikTok Shop | Gross revenue, Orders, ROI |
| Website | Purchase, CPA, ROAS, CTA Purchase, VTA Purchase |

### Attribution Analytics (gốc dòng 45)

So: cửa sổ ghi nhận, time to conversion, touchpoints to conversion, assisted conversions.
**Assisted shop metrics nhìn lại 28 ngày.**

### Video-level metrics trong Product GMV Max (gốc dòng 66)

Product clicks, ad conversion rate, **2s/6s/25/50/75/100% view rate**.

### Công thức funnel (gốc dòng 67-69)

| Tầng | Mục tiêu creative |
|---|---|
| Cold | Chứng minh vấn đề / sự tò mò |
| Warm | Chứng minh sản phẩm / niềm tin / lý do mua |
| Hot | Chốt ưu đãi / khẩn cấp / giảm ma sát |
| Existing buyers | Cross-sell, upsell, tái mua |

### Shop Activity audience (gốc dòng 70)

Hành vi: **PDP View, Add to Cart, Initiate Checkout, Complete Payment** với lookback **7/14/30/60/90/180 ngày**.

### Engagement audience nguồn

- Organic video.
- Ad content.
- LIVE.

### Lookalike (gốc dòng 70, 109)

- Cần tối thiểu **1.000 source users**.
- Source phải là người "đã làm việc có giá trị" — purchase, complete payment, high-value customer, ít nhất là initiate checkout.
- 3 mức: **Narrow / Balanced / Broad**.

### Custom audience

- Tối thiểu **1.000 matched users**.
- Có thể auto-refresh.

## 🔌 Phần 4 — Tracking + Audience

### Closed-loop signals của Shop (gốc dòng 74)

- TikTok Shop có closed-loop signals → Shop Ads chạy được **không cần Pixel website**.
- Case Love & Pebble: Shop Ads + affiliate creative dùng tín hiệu tại chỗ.
- **Bán về website → bắt buộc Pixel + nên có Events API**.

### Pixel + Events API + Deduplication (gốc dòng 75)

- TikTok khuyến nghị Pixel + Events API **dùng cùng nhau**.
- Gửi cùng 1 event qua cả 2 kênh → **deduplication bắt buộc + phải có `event_id`**.
- Hệ thống dùng event đầu tiên, làm giàu dữ liệu nếu trùng, tránh double count.
- **GTM server-side**: TikTok hỗ trợ flow cài đặt mặc định để tự cấu hình `event_id` deduplication.

→ Chi tiết: [[Pixel + CAPI + Event Deduplication]].

### Standard Events bắt buộc (gốc dòng 84)

ViewContent, AddToCart, InitiateCheckout, Purchase.

### Parameters quan trọng (gốc dòng 87-88)

- `content_ids, content_type, value, currency, quantity`.
- `value + currency` cho ROAS / VBO (Value-Based Optimization).
- `content_ids + content_type` cho shopping/catalog logic.

### QA tools

- **Test Events** trong Event Manager — quét QR test real-time trên mobile (dòng 92-94).
- **Pixel Helper 2.0** (dòng 96).

### UTM tối thiểu (gốc dòng 102-103)

```
utm_source=tiktok
utm_medium=paid_social
utm_campaign=seller_gmvmax_awareness_or_websales
utm_content=creative01_hook_demo
utm_term=aud_broad_or_lal_purchase30
```

### 4 nhóm audience (gốc dòng 105-109)

| Nhóm | Mô tả | Quy tắc |
|---|---|---|
| **Prospecting rộng** | Broad 18+ hoặc rộng theo category | LIVE Shopping/GMV Max khuyến nghị 18+ vì <18 không mua TikTok Shop |
| **Custom Audience** | Website traffic, engagement, lead, business account, customer file, shop activity | Min **1.000 matched users** |
| **Shop Activity** | PDP View / AddToCart / InitiateCheckout / CompletePayment | Lookback 7-180 ngày, có include/exclude, auto-refresh |
| **Lookalike** | Từ source quality cao | Min **1.000 source users**, 3 mức Narrow/Balanced/Broad |

## 🏗️ Phần 5 — Campaign + Budget + Bidding

### TikTok Ads Manager 3 tầng (gốc dòng 112)

- **Campaign**: objective + budget cấp campaign.
- **Ad group**: placements, audience, budget, schedule, optimization goal, bid.
- **Ad**: format, creative, caption, CTA, tracking.

### Cấu trúc nên dùng (gốc dòng 114-117)

| Nhu cầu | Campaign type |
|---|---|
| Always-on bán sản phẩm | **Product GMV Max** |
| Bùng nổ doanh số phiên live | **LIVE GMV Max** gắn lịch LIVE cố định |
| Website riêng | Sales hoặc Conversions + Pixel/Events API |

### LIVE GMV Max best practice (gốc dòng 116)

- Campaign chạy **tối thiểu 3 ngày**.
- Live session ổn định khung giờ và lượng phát.
- **Phiên LIVE >3 giờ** tăng GMV nhanh hơn.
- **Phát >8 giờ/ngày** tăng GMV mạnh hơn nữa.

### 2 Bidding strategies (gốc dòng 119)

| Strategy | Khi dùng |
|---|---|
| **Maximum Delivery** | Dùng ngân sách lấy nhiều kết quả nhất. Điểm bắt đầu dễ hơn cho người không có CPA cứng. |
| **Cost Cap** | Giữ chi phí kết quả quanh CPA mục tiêu. Hữu ích nếu ràng buộc CPA chặt; **dễ nghẽn chi tiêu nếu bid quá thấp**. |

### Ngưỡng nền tảng (gốc dòng 121-124)

| Ngưỡng | Giá trị | Ghi chú |
|---|---|---|
| Budget min — campaign daily | >50 USD | ⚠️ Quốc tế; VN có thể khác |
| Budget min — ad group daily | >20 USD | ⚠️ Quốc tế; VN có thể khác |
| Tăng budget post-learning (Ads Manager thủ công) | ≤30%/lần, cách nhau ~2 ngày | Bảo vệ learning |
| CBO chờ trước thay đổi lớn | 3 ngày HOẶC 50 conversions | — |
| Ad group budget — bidding strategy | ≥10× CPA hoặc 10× avg daily CPA | Hỗ trợ delivery |

### GMV Max — 2 modes (gốc dòng 125-127)

| Mode | Khi dùng | Best practice |
|---|---|---|
| **Target ROI** | Always-on để giữ hiệu quả | ROI ổn định |
| **Max Delivery** | Đẩy mạnh doanh số, launch mới hoặc mùa sale | Khuyến nghị 3-5 ngày đầu cho shop/sản phẩm mới. Budget khởi điểm **≥10× AOV**. Scale **~30%/ngày**. Có data Target ROI trước → set Max delivery = actual spend cũ HOẶC **1-5× actual spend cũ TRONG MÙA KHUYẾN MÃI**. **Vượt 5× → ROI tụt mạnh**. |

→ Chi tiết: [[GMV Max - Product vs LIVE]].

### Công thức triển khai (gốc dòng 146-150)

- 1 campaign = 1 mục tiêu rõ.
- 1 ad group = 1 giả thuyết rõ về audience/offer/creative bucket.
- 1 ad group = **3-5 creative khác biệt rõ**.
- 1 campaign = **3-5 ad group đa dạng** nếu manual.
- KHÔNG copy ad group mới hàng loạt; KHÔNG để phần lớn account cùng ở Learning Phase.

## 🎬 Phần 6 — Creative + A/B Test + 10 Kịch bản

### Quy tắc 1 — TikTok-first (gốc dòng 152)

- Video dọc 9:16, có âm thanh, ít nhất 720p, đúng safe zone, có người xuất hiện, phong cách tự nhiên, bám trend, hook mạnh, USP rõ, CTA rõ.
- Quảng cáo "**made for TikTok**" có completion rate cao hơn quảng cáo repurpose.
- Quảng cáo có tính giải trí giữ người xem lâu hơn.
- Sound-off → người dùng dễ skip hơn.
- **50% tác động tới recall/awareness đến từ 2-2,5 giây đầu.**

### Spark Ads (gốc dòng 153)

- Dùng post organic của bạn hoặc creator được uỷ quyền.
- **Cộng dồn comment/share/like/follow vào bài gốc.**
- Phân tích top 200 Spark Ads: creator involvement phổ biến.
- 4 pattern nổi bật:
  - **Unboxing**
  - **Product-in-use**
  - **Step-by-step**
  - **Reply-to-comment**
- Nói trực diện vào camera tăng hooking power.

### Cấu trúc video chuẩn (gốc dòng 155-156)

```
0-3s:    Hook
3-15s:   Bằng chứng / USP
15-30s:  Demo / social proof
3-5s cuối: Offer / CTA
```

**Thông số khuyến nghị**:
- Proposition trong **3 giây đầu**.
- Hook ưu tiên **6 giây đầu**.
- Text overlay **5-10 từ/giây**.
- CTA rõ ràng.

→ Chi tiết: [[5s Hook + Khung kịch bản video]].

### Split Test (gốc dòng 158)

Test được: targeting, placement, bidding & optimization, budget strategy, creative assets, catalog, creative, custom, Smart+.

**Best practice split test**:
- Hypothesis rõ.
- Biến khác biệt đủ lớn.
- Audience đủ rộng.
- Chạy ít nhất **7 ngày**.
- Estimated power ít nhất **80%**.
- KHÔNG chỉnh giữa chừng.

### 4 mẹo creative tác động lớn nhất (gốc dòng 205-209)

1. **Người xuất hiện cùng sản phẩm > chỉ quay sản phẩm.**
2. **Trend là "xe chở hàng", không phải "hàng hoá".** Sản phẩm vẫn là hero.
3. **Không ép tất cả video ngắn.** Spark Ads thắng có thể dài >38 giây nếu câu chuyện đủ cuốn. Nguyên tắc: **ngắn nếu yếu, dài nếu hay**.
4. **Duy trì creative supply liên tục.** Thêm creative mới vào ad group hiện tại > tạo ad group mới để kéo dài tuổi thọ nhóm.

## 🔁 Phần 7 — Remarketing + Tối ưu + Scaling

### Remarketing là TẦNG CHỐT LỜI (gốc dòng 211)

Không phải "bám đuôi" — là tầng lợi nhuận.

### 4 cửa sổ remarketing (gốc dòng 213-233)

| Cửa sổ | Audience | Creative |
|---|---|---|
| **Very warm** | PDP View 7-14 ngày | Demo ngắn + bằng chứng + CTA |
| **Hot** | ATC / Initiate Checkout 7-14 ngày | Offer, bonus, lý do mua ngay |
| **Re-open** | PDP/ATC/IC 30 ngày, **exclude purchase 7 ngày** | Review, creator proof, objection handling |
| **Existing buyers** | Purchase 30/60/180 ngày | Cross-sell, upsell, refill, combo. Mục tiêu **tăng LTV**. |

### Creative sequencing (gốc dòng 236-241)

| Lần | Nội dung |
|---|---|
| Lần 1 | Tò mò / nỗi đau / use-case |
| Lần 2 | Review / creator / social proof |
| Lần 3 | Xử lý phản đối / so sánh / demo sâu |
| Lần cuối | Offer / bundle / urgency / CTA mạnh |

### Tối ưu sau launch (gốc dòng 243)

- **KHÔNG thay đổi trong Learning Phase.**
- Scale conversion tốt nhất khi ad group đạt **50 conversions trong 1 tuần** + đáp ứng KPI.
- Sau learning: tăng ngân sách **20-30% an toàn hơn** tăng sốc.
- Performance giảm → sửa creative/bid/targeting, KHÔNG clone hàng loạt.

### Automated Rules (gốc dòng 245)

⚠️ **KHÔNG hỗ trợ campaign tạo trong Seller Center.** Muốn automation mạnh → tạo trong Ads Manager hoặc dùng **API for Business / Marketing API**.

### 3 mẫu rule đề xuất (gốc dòng 247-249)

1. **Rule bảo vệ ngân sách**: spend vượt ngưỡng mà không có purchase/order → cảnh báo hoặc pause.
2. **Rule scale mềm**: ad group đạt KPI 3 ngày liên tục → tăng budget 20-30%.
3. **Rule dayparting có điều kiện**: chỉ với LIVE hoặc business có khung giờ rõ. Cơ sở chính thức cho dayparting mạnh nhất ở **LIVE Shopping Ads** và **lead generation ads**.

## ⚖️ Phần 8 — Policy + Case Studies + Roadmap

### TikTok review xét gì (gốc dòng 254)

- Ngành hàng.
- Caption/text.
- Hình ảnh/video.
- Audio.
- Thị trường + nhóm tuổi mục tiêu.
- Độ nhất quán giữa ad và landing page.
- Chức năng landing page.

**Phần lớn ads review trong 24 giờ.** Ad đã duyệt vẫn có thể bị review lại nếu nhận phản hồi xấu hoặc phát hiện vi phạm sau.

### 8 lỗi hay chết nhất với seller mới (gốc dòng 255-263)

1. Creative và landing page không nhất quán.
2. Caption nói một đằng, video một nẻo.
3. Claim giảm giá không đúng.
4. Ảnh/video mờ, text lỗi chính tả hoặc "gimmick spelling".
5. Nhét QR code trong ad creative.
6. Gesture giả "swipe up" không được hỗ trợ.
7. Nội dung nhạy cảm, dangerous products, misinformation, **healthcare/pharma không đúng market rule**.
8. **Việt Nam: ngôn ngữ ad/landing nên là tiếng Việt hoặc tiếng Anh; disclaimer ngành bắt buộc ở ngôn ngữ địa phương.**

→ ⚠️ TPCN thuộc **healthcare/pharma** → bắt buộc check kỹ market rule VN trước launch.

### Shop Performance Score + Account Health (gốc dòng 264)

| Chỉ số | Thang | Đo gì |
|---|---|---|
| **SPS** (Shop Performance Score) | 0-5 | Product satisfaction + fulfillment/logistics + customer service |
| **TikTok Account Health** | — | Vi phạm của official/marketing creator accounts trong **90 ngày** |
| **AHR** (Account Health Rating) | 0-1000 trong **180 ngày** | Compliance — có thể dẫn đến enforcement nếu thấp |

→ **Quảng cáo tốt mà shop fulfillment tệ → vẫn gãy hệ thống.**

### 6 case studies (gốc dòng 269-286)

| Brand | Kết quả |
|---|---|
| **Love & Pebble** | 3.2× ROAS, hơn 240 conversions, 250.000 impressions; sales tăng **1.194%**, CPA giảm **409%** so với BAU |
| **Edikted** | GMV +111%, orders +98%, hơn 1 triệu visitors trong 5 ngày; **#1 GMV ngành fashion** thời gian campaign |
| **Very** | ROAS +12%, CVR +38%; sau đó tăng đầu tư VSA thêm 52% |
| **American Eagle** | ROAS +100%, CPA hiệu quả hơn 46%, **CVR tăng 10×** |
| **Baseus** | Conversion rate +60%, peak CVR 8.03%, ROAS toàn chiến dịch **gấp 5 lần** |
| **Haus Von Albe** | Hơn 2.090 website conversions, CTR 1.23%, organic followers +8.3K |

⚠️ **Footnote case study gắn SAI** — kết quả con số đúng, URL footnote sai.

**Kết luận case studies**: creative native + creator content là đòn bẩy số 1; broad/intent-based thắng over-segmentation; paid mạnh khi nối với organic, affiliate, search hoặc data layer.

### Lộ trình Gantt 90 ngày — 6 section (gốc dòng 250-251)

1. **Nền tảng**: kết nối shop, BC, ad account, primary GMV Max + chuẩn hoá danh mục, PDP, pricing, voucher, tồn.
2. **Dữ liệu**: setup Pixel + Events API + UTM + QA + tạo audiences nền + dashboard KPI.
3. **Creative**: sản xuất 15-30 video đầu + Spark/creator/ACA pipeline.
4. **Campaign**: launch Product GMV Max / website sales test + split test.
5. **Tối ưu**: remarketing PDP-ATC-IC-Purchase + scale winner +20-30%.
6. **Mở rộng**: LIVE GMV Max / Search / cross-sell / API automation.

### Checklist 30/60/90 ngày

**30 ngày đầu**:
- ☐ Kết nối shop-BC-ad account; xác nhận primary ad account cho GMV Max.
- ☐ Chuẩn hoá PDP, giá, voucher, tồn.
- ☐ Setup audience nền.
- ☐ Web → xong Pixel + Events API + UTM + QA.
- ☐ Chuẩn bị **15-30 video** đầu tiên.
- ☐ Launch Product GMV Max hoặc website sales test.
- ☐ KHÔNG sửa ads quá sớm.
- **Tiêu chí đạt**: tracking đúng, vài creative sống được, baseline CTR/PDP/ATC/order.

**60 ngày đầu**:
- ☐ Tạo tệp remarketing 7/14/30 ngày.
- ☐ Tách bucket creative theo hook/offer/creator/demo.
- ☐ Bắt đầu split test nghiêm túc.
- ☐ Review assisted metrics, time to conversion, video reporting.
- ☐ Thêm Spark/ACA/creator pipeline.
- **Tiêu chí đạt**: xác định **20% creative tạo 80% kết quả**; có rule giữ/cắt; audience nóng có doanh số ổn định.

**90 ngày đầu**:
- ☐ Scale winner 20-30%.
- ☐ Thử LIVE GMV Max nếu có điều kiện.
- ☐ Mở search hoặc website sales bổ sung.
- ☐ Đưa automation/rules/API vào báo cáo và vận hành.
- ☐ Chuẩn hoá scorecard shop health + account health.
- **Tiêu chí đạt**: ≥1-2 hệ chiến dịch always-on; scale không phá learning; shop đủ khoẻ.

### 3 bước làm ngay (gốc dòng 304-306)

1. **Khoá mô hình kinh doanh** — TikTok Shop hay website. Đúng = đã xác định đích chuyển đổi, event tối ưu, dashboard.
2. **Dựng xong hạ tầng dữ liệu + creative tối thiểu trước khi scale.** Đúng = QA xong, audience nền đủ, có ít nhất 15-30 video đầu hoặc 3-5 creative khác biệt cho mỗi ad group test.
3. **Chỉ scale khi đã có winner thật.** Đúng = qua learning, KPI đáp ứng, scale theo nấc.

## 💬 Trích dẫn

> "Đừng tối ưu từ Ads Manager — hãy tối ưu từ đường đi mua hàng." *(dòng 6)*

> "Creative là biến số số một." *(dòng 5)*

> "Remarketing không phải chiến dịch phụ — là tầng lợi nhuận." *(dòng 5)*

> "Trend chỉ nên là xe chở hàng, không phải hàng hoá." *(dòng 207)*

> "Quảng cáo tốt mà shop fulfillment tệ thì vẫn gãy hệ thống." *(dòng 264)*

## 🔗 Liên kết

- [[Khối 14 - ADS Các nền tảng]] — page mẹ
- [[GMV Max - Product vs LIVE]] — concept đặc thù TikTok
- [[Learning Phase (50 events tuần)]] — chung Meta + TikTok
- [[Pixel + CAPI + Event Deduplication]] — hạ tầng tracking
- [[5s Hook + Khung kịch bản video]] — creative
- [[TOF-MOF-BOF Funnel + Audience Layers]] — funnel
- [[Special Ad Category + chính sách Health-YMYL]] — bắt buộc cho TPCN
