---
type: source
tags: [ips, khoi-14, ads, facebook, meta, ptl]
created: 2026-05-09
updated: 2026-05-09
sources: ["[[raw/Đặc sản của Phạm Thành Long/IPS - 19 khối công việc/14_ ADS Các nền tảng/ADS FACEBOOK.docx]]"]
khoi: 14
---

# Khối 14a — ADS Facebook (Meta)

> Sub-page của [[Khối 14 - ADS Các nền tảng]]. File gốc 443 dòng, 7 phần.

## ⚠️ Lỗi phát hiện trong gốc — đã hiệu chỉnh

- **Mốc "tháng 4/2026"** trong gốc nói tương lai về CAPI bắt buộc cho conversion leads — hiện đã qua (2026-05-09). Khi triển khai phải kiểm chứng tình trạng thực tế trong Events Manager.
- **"Data Studio"** đã được Google đổi tên thành **Looker Studio** từ 2022 — em dùng tên mới khi ghi.
- **"1,400 nguồn dữ liệu"** Looker Studio kết nối — số có thể phóng đại, anh tự xác minh nếu cần.
- **2 ví dụ minh hoạ trong gốc dùng ngành xăm (ngành cũ của anh)** — em thay bằng ngữ cảnh trung tính. KHÔNG ghi nội dung xăm vào Não.

## 🎯 TL;DR

Facebook Ads 2026 = **hệ thống phân phối xác suất** dựa trên dữ liệu, chất lượng quảng cáo và tín hiệu chuyển đổi. Người mới phải đi theo chuỗi logic: **mục tiêu kinh doanh → objective → conversion location → performance goal → event → creative → landing page → đo lường**. Lệch một mắt xích là tối ưu sai hướng.

**Công thức thực chiến**: Offer × Tracking sạch × Objective đúng × Creative hợp ngữ cảnh × Landing page ít ma sát × Vòng lặp tối ưu kỷ luật.

**3 sai lầm chết người**:
1. Muốn ra đơn nhưng tối ưu cho click.
2. Chia quá nhiều ad set → learning limited.
3. Micro-target interest stack quá hẹp khi Meta đã tinh gọn detailed targeting.

**Quy tắc cứng nhất**: cần **~50 optimization events/tuần** mỗi ad set để thoát [[Learning Phase (50 events tuần)|Learning Phase]]. Không đủ → lùi event lên gần hơn (Purchase → AddToCart, Lead → LPV) thay vì mở target rộng vô tội vạ.

## 🧭 Mục lục 7 phần (theo gốc)

1. **Tóm tắt điều hành** — 6 objective Meta mới + business portfolio + công thức + 3 sai lầm.
2. **Tư duy nền tảng** — 3 tầng mục tiêu, 50 events/tuần, bỏ tư duy target chi tiết, 5 nguyên tắc.
3. **Hạ tầng tài khoản & đo lường** — business portfolio, checklist kỹ thuật, offline events, CAPI, event mapping Meta-GA4.
4. **Funnel + audience + remarketing** — TOF/MOF/BOF, 4 lớp audience, retention windows, dynamic ads, 4 case study.
5. **Creative + landing page + A/B testing** — dynamic creative, 4 format cơ bản, công thức copy 6 bước, checklist landing page, 5 kịch bản A/B test.
6. **Đo lường + bidding + tối ưu + scaling** — attribution, Conversion Lift, 3 lớp bidding, ngân sách, nguyên tắc tối ưu 7-14 ngày, scaling dọc/ngang, **chính sách Health/YMYL**.
7. **Benchmark + dashboard + công cụ + lộ trình 30/60/90** — WordStream + Triple Whale benchmark, 5 tab dashboard, UTM, automated rules, Apps Script alerts.

## 🧱 Phần 1+2 — Tư duy + Nền tảng

### 6 objective Meta hiện tại
**Awareness**, **Traffic**, **Engagement**, **Leads**, **App Promotion**, **Sales**.

### Chuỗi logic 8 bước (gốc dòng 3)
Mục tiêu kinh doanh → objective → conversion location → performance goal → event → creative → landing page → đo lường.

### Bảng chọn objective theo bài toán

| Bài toán | Objective | Performance goal / Event |
|---|---|---|
| Phủ nhận biết | Awareness | Reach, impressions, ThruPlay |
| Kéo người vào web (web chưa đủ data) | Traffic | Website + LPV |
| Social proof, video | Engagement | Post engagement, video views, messages |
| Cần lead | Leads | Website, instant form, calls, messages |
| Bán hàng | Sales | Website/App/Shop + Purchase/Value |
| Cài app | App Promotion | App install/in-app event |

### 5 nguyên tắc tư duy người mới (gốc dòng 48-53)
1. Bắt đầu bằng **kết quả kinh doanh muốn mua**, không phải target.
2. Bắt đầu bằng **tracking sạch**, không phải scale.
3. **Không tối ưu click** nếu cần lead/sale.
4. **Không chia nhỏ** cấu trúc quá sớm.
5. **First-party data + remarketing > interest**.

### Quy tắc 50 events/tuần
- Mốc thoát Learning Phase mỗi ad set.
- Không đạt → **learning limited** → tối ưu kém.
- Cách xử lý đúng khi thiếu volume: **lùi lên event gần hơn** (Purchase → AddToCart → ViewContent), không phải mở target rộng vô tội vạ.

→ Chi tiết: [[Learning Phase (50 events tuần)]].

## 🏗️ Phần 3 — Hạ tầng tài khoản & đo lường

### Cấu trúc tài khoản (gốc dòng 55)
- **Business Portfolio** (BM cũ đổi tên) = "công ty mẹ" của tài sản.
- **Ad Account** = nơi tiêu tiền.
- **Dataset/Pixel** = nơi ghi nhận hành vi web.
- **GA4** = nơi đối chiếu đa kênh.
- **CAPI (Conversions API)** = đường gửi dữ liệu từ máy chủ.
- **Catalog** = kho sản phẩm cho quảng cáo động.

### Checklist kỹ thuật trước chiến dịch đầu tiên — 9 bước

1. ☐ Tạo Business Portfolio + thêm Page + ad account + đối tác + phân quyền tối thiểu.
2. ☐ Bật **2FA** cho mọi người có quyền vào tài sản.
3. ☐ **Verify business + verify domain** ngay từ đầu.
4. ☐ Tạo dataset/Pixel + gắn vào web + kết nối ad account.
5. ☐ Set up **Standard Events**: ViewContent, AddToCart, InitiateCheckout, Lead, Purchase, CompleteRegistration.
6. ☐ Bật **CAPI**, **dedup pixel + CAPI bằng event_id/event name**, test bằng **Test Events Tool**.
7. ☐ Theo dõi **Event Match Quality (EMQ)**, diagnostics, event coverage ratio.
8. ☐ Cài **GA4** song song.
9. ☐ Offline events nếu có gọi điện/chốt cửa hàng/CRM.

→ Chi tiết: [[Pixel + CAPI + Event Deduplication]].

### Event mapping Meta ↔ GA4

| Meta event | GA4 event |
|---|---|
| PageView | page_view |
| ViewContent | view_item |
| AddToCart | add_to_cart |
| InitiateCheckout | begin_checkout |
| Lead | generate_lead |
| Purchase | purchase |
| AddPaymentInfo | add_payment_info |
| CompleteRegistration | sign_up |

### 2 lưu ý quan trọng hiện tại
- Từ **2024**, Meta chuyển offline events từ "offline event sets" sang **datasets**.
- ⚠️ Tài liệu gốc nói "từ 4/2026 conversion leads performance goal không còn khả dụng cho chiến dịch mới nếu không có CAPI" — mốc đã qua. Phải kiểm chứng lại trong Events Manager khi triển khai.

## 🎯 Phần 4 — Funnel + Audience + Remarketing

### Sơ đồ TOF/MOF/BOF (gốc dòng 103)

```
TOF (Người lạ): Video view, LPV, Engaged users
  → Audience: Broad / Advantage+ / Lookalike

MOF (Người quan tâm): ViewContent, Lead form opened, Messenger started
  → Audience: Website 30-180d, Video engagers 30-90d, IG-FB engagers 30-365d

BOF (Ý định cao): AddToCart, InitiateCheckout, Qualified Lead
  → Audience: ATC 1-14d, IC 1-14d, Form opened, Message started

Sau Purchase: Upsell / Cross-sell / Reactivation
Loại trừ: người đã mua / đã chốt
```

→ Chi tiết: [[TOF-MOF-BOF Funnel + Audience Layers]].

### 4 lớp audience (gốc dòng 105)

- **Custom audience** = vàng (remarketing).
- **Lookalike** = bạc (prospecting).
- **Detailed targeting** = bổ trợ.
- **Broad/Advantage+** = ngày càng đáng tin khi pixel + creative tốt.

### Retention windows (gốc dòng 106)

| Loại | Tối đa | Khuyến nghị seed |
|---|---|---|
| Website custom audience | **180 ngày** | — |
| Page/Instagram engagement | **365 ngày** | — |
| Lookalike | — | Tối thiểu **100 người** seed; khuyến nghị **1.000-5.000** |

**Chia tệp theo nhiệt độ**: 1-7d nóng, 8-30d ấm, 31-180d nguội.

### Dynamic Ads / Catalog Ads
- Đòn bẩy lớn nhất e-commerce hay bỏ qua.
- Cần catalog + feed sạch + pixel/SDK với ViewContent, AddToCart, Purchase.

### 4 case study (gốc dòng 108-109)

| Case | Kết quả | Insight |
|---|---|---|
| **VistaPrint** | **2.5× incremental purchases** với Advantage+ catalog ad | Catalog match rate cao hơn |
| **Europcar** | **2.9× bookings** với Advantage+ shopping tự động vs thủ công | Tự động hoá thắng thủ công khi có data |
| **DIVA Beauty Center** | Reels đa dạng cho ads click-to-Messenger | Format đa dạng → reach + chuyển đổi |
| **CỎ MỀM HomeLab** | Thử value optimization cho ads click-to-Messenger | Value optimization phù hợp lead-via-chat |

### Bảng chiến lược theo ngành (gốc dòng 110-152)

| Ngành | Objective | Funnel split | Audience ưu tiên | Creative | KPI |
|---|---|---|---|---|---|
| **E-commerce có catalog** | Sales | 50/20/30 | Broad + lookalike + website + purchasers exclude | Video demo, carousel, catalog, UGC | CPA, ROAS, AOV |
| **Dịch vụ địa phương/clinic** | Leads/Calls | 50/20/30 | Geo + engagers + website + call starters | Proof, testimonial, quy trình, ưu đãi tư vấn | CPL, booking rate |
| **Giáo dục/khoá học** | Leads | 60/25/15 | Broad + engagers 365d + website 180d + lead lookalike | Case study học viên, syllabus, hook nghề nghiệp | CPL, show-up, close |
| **Real estate/tài chính** | Leads + Special Ad Category | 40/20/40 | First-party + special ad audience | Trust, hàng có, lịch hẹn | Qualified lead, appointment |
| **B2B** | Leads | 55/30/15 | Customer list, website, video engagers | ROI, case study, demo, checklist | CPL, MQL, SQL |
| **App** | App Promotion | 60/20/20 | Broad + app events custom | Video dọc, incentive, demo | CPI, cost per in-app event |

📎 *Em (agent) thêm — TPCN nên tham chiếu*:
- TPCN bán online qua web/Shopee/Tiki → mô hình **e-commerce có catalog** (50/20/30, Sales, KPI: CPA/ROAS/AOV).
- TPCN bán qua tư vấn dược sĩ/bác sĩ → mô hình **dịch vụ địa phương/clinic** (50/20/30, Leads/Calls).
- TPCN bán qua phễu seminar/khoá sức khoẻ → mô hình **giáo dục** (60/25/15, Leads).

## ✍️ Phần 5 — Creative + Landing Page + A/B Testing

### 4 format cơ bản cho người mới
Single image, **video**, carousel, collection. **Collection** = thiết kế chuyển từ discovery → mua trên mobile.

### Advantage+ Placements > Manual
Thí nghiệm Meta: Advantage+ placements cho **CPA thấp hơn trung bình 11.7%** vs manual (gốc dòng 157).

### Công thức copy 6 bước (gốc dòng 158)

```
Hook → Problem/Desire → Proof → Offer → Risk reversal → CTA
```

### CTA theo tầng funnel (gốc dòng 159)

| Tầng | CTA mẫu |
|---|---|
| TOF (mềm) | "Xem thêm", "Xem cách hoạt động", "Nhận checklist" |
| MOF (vừa) | "Xem giá", "Xem feedback", "So sánh mẫu" |
| BOF (mạnh) | "Mua ngay", "Đặt lịch tư vấn", "Nhận báo giá", "Đăng ký học thử" |

### Landing page — 3 việc + 8 checklist

**3 việc**: khớp thông điệp với ad, giảm ma sát, tăng tin cậy.

**Số liệu Google**: trang mobile nhanh hơn **1 giây** có thể tăng conversion rate đến **27%** (gốc dòng 160).

**Checklist 8 mục**:
1. ☐ Phần đầu khớp lời hứa ad.
2. ☐ Một CTA chính.
3. ☐ Proof càng sớm càng tốt.
4. ☐ Form ngắn nhất.
5. ☐ Mobile CTA luôn nhìn thấy sớm.
6. ☐ Tốc độ > hiệu ứng.
7. ☐ Có FAQ.
8. ☐ UTM nhất quán.

### 5 kịch bản A/B test (gốc dòng 171-201)

1. **Hook đau vs Hook ham muốn** (biến: 3 giây đầu).
2. **UGC vs Demo kỹ thuật** (biến: loại video).
3. **CTA mềm vs CTA cứng** (biến: câu CTA).
4. **Broad vs Lookalike** (biến: audience).
5. **Trang ngắn vs Trang proof dày** (biến: landing page).

### Ad Relevance Diagnostics (gốc dòng 202)
3 chỉ số: **quality ranking + engagement rate ranking + conversion rate ranking**.
→ **Là công cụ chẩn đoán, KHÔNG phải KPI tối thượng**.

⚠️ Lưu ý: 3 ranking này hiện chỉ hiển thị dạng **above/at/below average** chứ không phải điểm số cụ thể.

## 📊 Phần 6 — Đo lường + Bidding + Tối ưu + Scaling

### Attribution Settings
1-day view, 1-day click, 7-day click, 28-day click. Một số metrics là **ước tính/mô hình hoá**.

### Conversion Lift + Brand Lift (Experiments)
Đo **incremental effect thực sự** — dữ liệu nền tảng không có holdout/control phù hợp → dễ suy luận nhân quả sai.

### 3 lớp bidding (gốc dòng 206)

1. **Lớp 1**: highest volume / lowest cost (an toàn, điểm bắt đầu).
2. **Lớp 2**: cost per result goal hoặc ROAS goal (khi đã biết ngưỡng).
3. **Lớp 3**: bid cap (dao sắc, người mới hay cầm ngược).

### Ngân sách

| Loại | Mô tả |
|---|---|
| **Advantage+ campaign budget** | Tự phân bổ giữa ad sets |
| **Ad set budget** | Khi cần lịch/bid/nhịp riêng |
| **Daily budget** | Trung bình ngày (có thể chi cao hơn vào ngày tốt) |
| **Lifetime budget** | Trần toàn chiến dịch |

### Nguyên tắc tối ưu 7-14 ngày đầu (gốc dòng 208-215)

**72h đầu**: chỉ nhìn lỗi kỹ thuật, phân phối, CTR, LPV rate, CPM bất thường, reject, learning limited.

**Sau khi đủ data**: đọc theo thứ tự **CPM → CTR → LPV rate → CVR → CPA/CPL/ROAS**.

| Tầng | Triệu chứng | Vấn đề ở đâu |
|---|---|---|
| CPM cao | Audience cạnh tranh hoặc creative thiếu hấp dẫn |
| CTR thấp | Hook/offer/creative |
| CTR tốt + LPV thấp | Landing page chậm/mismatch |
| LPV tốt + CVR thấp | Offer/proof/giá/UX form |
| CVR tốt + CPA cao | Objective/bid/audience/placements/frequency |

→ Chi tiết: [[Khung diagnose phễu]].

### Scaling 2 kiểu

- **Vertical**: tăng ngân sách campaign/ad set thắng.
- **Horizontal**: nhân thêm góc creative, audience, thị trường, placement, funnel.

**Sai lầm**:
- Tăng ngân sách quá mạnh → quay lại Learning Phase.
- Nhân bản nhiều ad set giống nhau → auction overlap.

### 5 advanced tricks (gốc dòng 218-223)

1. **Advantage+ placements** trước manual.
2. **Pixel + CAPI dedup chuẩn** + Event Match Quality.
3. **Catalog ads** khi feed đủ sạch.
4. **Value optimization** / maximize value khi đo được giá trị đơn hàng.
5. **Automated rules** để giữ kỷ luật.

→ Chi tiết: [[Advantage+ Family]].

### Chính sách Meta cho Health (TPCN) — QUAN TRỌNG (gốc dòng 224)

Meta **CẤM/SIẾT** quảng cáo (theo gốc PTL liệt kê):
- Gợi nhắc **personal attributes**: "Bạn đang béo?", "Bạn bị mụn nặng?" — cấm.
- Có chính sách riêng cho **health, sensitive content, sensational content, housing/employment/financial, gambling, crypto**.
- **Special Ad Category** bị giới hạn audience selection.

🚨 **Sửa sau QA round 2 — phân biệt rõ**:
- **Special Ad Category** (theo policy Meta hiện tại) chỉ gồm 4 nhóm: **Credit, Employment, Housing, Social Issues/Elections**.
- **Health/TPCN KHÔNG nằm trong Special Ad Category** — chịu chính sách RIÊNG (Personal Health Ads, Drugs & Pharmaceuticals, Sensational Content).
- Cả 2 nhóm đều **kiểm duyệt nghiêm**, nhưng **mechanism khác nhau** — không nhầm lẫn khi setup audience.

→ TPCN đọc bắt buộc [[Special Ad Category + chính sách Health-YMYL]] + [[Khối 14f - Từ cấm FB Ads (cảnh báo nhân viên)]].

### Checklist an toàn tài khoản — 6 mục

1. ☐ Không chạm "nỗi xấu hổ" của user.
2. ☐ Không **before/after** dễ hiểu nhầm (đặc biệt TPCN).
3. ☐ Domain + Page + ad + LP cùng câu chuyện.
4. ☐ Theo dõi **Account Quality**.
5. ☐ Chấp nhận Lead Ads Terms.
6. ☐ Lịch sử thanh toán sạch + 2FA.

## 📈 Phần 7 — Benchmark + Dashboard + Công cụ + Lộ trình 30/60/90

### Benchmark cảnh báo
**Benchmark VN công khai chuẩn hoá: KHÔNG xác định** (gốc tự thừa nhận, dòng 233). Dùng để **đặt câu hỏi**, không phải tự ám thị.

### Bảng WordStream lead-gen 2025 (>1.000 chiến dịch)

| Ngành | CTR | CPC | CVR | CPL |
|---|---|---|---|---|
| Real Estate | 3.75% | $1.57 | 9.53% | $16.61 |
| Education | 1.86% | $1.65 | 10.08% | $28.22 |
| Legal | 2.11% | $4.10 | 10.53% | $18.17 |
| Restaurants | 2.97% | $0.74 | 18.25% | $3.16 |
| Dentists | 1.05% | $9.78 | 6.38% | $76.71 |

### Bảng Triple Whale e-commerce 2026 (~35.000 brands, 2025)

| Ngành | CTR | CVR | CPA | ROAS |
|---|---|---|---|---|
| Apparel | 2.25% | 1.46% | $36.76 | 2.18 |
| Beauty | 2.27% | 1.94% | $37.92 | 1.57 |
| Electronics | 2.19% | 1.20% | $49.48 | 1.92 |
| **Health & Wellness** | **2.70%** | **1.72%** | **$38.55** | **1.50** |
| Automotive | 2.22% | 1.30% | $34.15 | 2.54 |
| **Tổng quan** | 2.19% | 1.57% | $38.17 | 1.93 (CPM $13.48) |

→ TPCN ≈ Health & Wellness — ROAS benchmark 1.50 là **quá thấp** với biên LN TPCN 60-80%; mục tiêu của anh nên ≥3.0.

### 5 tab dashboard chuẩn (gốc dòng 297-302)

1. **Executive view**: spend, revenue, leads, CPL/CPA, ROAS, top winners, top issues.
2. **Funnel view**: impression, CPM, CTR, LPV, CVR, CPA theo TOF/MOF/BOF.
3. **Creative view**: format, hook, angle, ad ID, CTR, CVR, CPA, rankings.
4. **Audience view**: broad vs lookalike vs remarketing vs địa lý.
5. **Diagnostics view**: learning limited, frequency, reject, event coverage, match quality.

### UTM template (gốc dòng 305-306)

```
utm_source=meta
utm_medium=paid_social
utm_campaign={{brand}}_{{objective}}_{{country}}_{{offer}}_{{funnel}}
utm_content={{angle}}_{{format}}_{{hook}}_{{adid}}
utm_term={{audience}}
```

→ Chi tiết: [[UTM template chuẩn 4 nền tảng]].

### 5 Automated Rules đề xuất (gốc dòng 307-325)

1. **Kill ad yếu**: spend > 2× target CPA + 0 result trong 3 ngày → tắt.
2. **Tăng budget ad thắng**: results ≥ 3 + CPA < 80% target trong 3 ngày → tăng 10-15%.
3. **Báo fatigue**: frequency > 3 + CTR giảm > 30% so với 7 ngày trước → cảnh báo + duplicate angle mới.
4. **Báo lỗi tracking**: spend có nhưng results = 0 toàn campaign bất thường → cảnh báo.
5. **Báo rủi ro lead quality**: CPL rẻ nhưng close rate giảm mạnh CRM → gắn cờ, không scale.

### Apps Script `metaDailyAlerts()` (gốc dòng 326-327)

Đọc sheet `meta_daily`, gửi mail cảnh báo khi:
- spend ≥ 2.000.000đ + results = 0 → STOP xem xét.
- cpa > 250.000đ + results > 0 → CPA cao.
- 0 < roas < 1.5 → ROAS thấp.
- frequency > 3 + ctr < 1% → creative cũ.

### Lộ trình 30/60/90 ngày

| Giai đoạn | Mục tiêu | Việc | Dấu hiệu đạt |
|---|---|---|---|
| **30 ngày** | Hạ tầng + baseline | BP, quyền, 2FA, domain, pixel, CAPI, GA4, dashboard, 2-3 campaign, 3-5 góc creative | Event đúng, đọc số được, có baseline |
| **60 ngày** | Máy test có kỷ luật | TOF/MOF/BOF, custom audiences, lookalike, A/B test tuần, automated rules, lead quality từ CRM | Biết ad thắng vì sao, biết nút thắt |
| **90 ngày** | Scale có kiểm soát | Catalog/dynamic, budget strategy, value optimization, offline events, Conversion Lift/MMM | Scale + số liệu sạch, không phụ thuộc 1 ad |

## 💬 Trích dẫn

> "Đưa đúng tín hiệu để hệ thống tự tìm đúng người." *(gốc dòng 7)*

> "Đừng bắt đầu bằng target — bắt đầu bằng kết quả kinh doanh muốn mua." *(dòng 49)*

> "First-party data và remarketing có giá trị cao hơn." *(dòng 53)*

> "Bid cap là dao sắc; người mới thường cầm ngược." *(dòng 206)*

## 🔗 Liên kết

- [[Khối 14 - ADS Các nền tảng]] — page mẹ
- [[Learning Phase (50 events tuần)]] — concept nền
- [[Pixel + CAPI + Event Deduplication]] — hạ tầng tracking
- [[Advantage+ Family]] — trụ cột AI hoá Meta
- [[TOF-MOF-BOF Funnel + Audience Layers]] — funnel
- [[Special Ad Category + chính sách Health-YMYL]] — bắt buộc cho TPCN
- [[Khối 14f - Từ cấm FB Ads (cảnh báo nhân viên)]] — checklist từ tránh
