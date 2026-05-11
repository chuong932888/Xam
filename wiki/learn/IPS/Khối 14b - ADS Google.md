---
type: source
tags: [ips, khoi-14, ads, google, ptl]
created: 2026-05-09
updated: 2026-05-09
sources: ["[[raw/Đặc sản của Phạm Thành Long/IPS - 19 khối công việc/14_ ADS Các nền tảng/ADS GOOGLE.docx]]"]
khoi: 14
---

# Khối 14b — ADS Google

> Sub-page của [[Khối 14 - ADS Các nền tảng]]. File gốc 477 dòng, 9 phần + 55 footnote.

## ⚠️ Lỗi phát hiện trong gốc — đã hiệu chỉnh

- **6 footnote citation gắn SAI** ([33], [35], [37], [39], [41], [43]) — lệch 1 đơn vị so với link thực. Lỗi formatting nghiêm trọng từ docx gốc. **Khi anh xem case study Samsung/1STOPlighting/Traveloka/David Jones/Campmor — đừng tin số footnote**, kết quả con số vẫn đúng nhưng URL trỏ sai chỗ. Anh muốn tra cứu nguồn → search Google Ads case studies trực tiếp.
- **Mermaid diagram** (gốc dòng 165) bị nén thành 1 dòng dài — em đã giãn ra format đọc được.
- **Bảng bị flatten thành text** — em đã dựng lại bảng markdown.
- **Naming convention ví dụ** trong gốc dùng "MayXam"/"may_xam" — em thay bằng ví dụ TPCN trung tính.

## 🎯 TL;DR

Báo cáo dạy người mới chạy Google Ads + remarketing **đúng thứ tự**: mục tiêu kinh doanh → conversion goal → tracking → loại chiến dịch → cấu trúc tài khoản → ad/asset → landing page → bidding → tối ưu. **Đảo ngược thứ tự = data bẩn, bid học sai, remarketing yếu.**

**Default an toàn cho người mới**:
- Bắt đầu **Search ý định mua cao** → thêm remarketing.
- E-commerce có feed sạch + value tracking → cân nhắc Shopping/Performance Max ở giai đoạn sau.
- **Smart Bidding KHÔNG chữa được tracking sai.**

**Cách hỏi ngân sách đúng**:
- KHÔNG hỏi "đốt bao nhiêu tiền".
- HỎI "mỗi ngày đủ ngân sách mua bao nhiêu conversion ở CPA mục tiêu?".

**Lộ trình 30 ngày**: khoá tracking trước khi scale bidding.

## 🧭 Mục lục 9 phần (theo gốc)

1. **Executive summary** — đúng thứ tự, default an toàn, remarketing 4 điều kiện, cách hỏi ngân sách.
2. **Tư duy gốc + bản đồ yếu tố** — 16 yếu tố + Quality Score vs Ad Rank.
3. **So sánh 5 loại campaign** — Search/Display/Video/Shopping/PMax.
4. **Quy trình 11 bước** + sơ đồ Mermaid + timeline 30 ngày.
5. **Công thức + checklist + templates** — KPI, kịch bản ngân sách, naming, landing page 8 khối, tracking plan 9 events.
6. **Remarketing + kỹ thuật nâng cao** — basic, layering, RLSA, dynamic, Customer Match, Smart Bidding tips, PMax, scripts/rules/API, offline conversion, cross-device, budget allocation, anomaly detection.
7. **11 lỗi phổ biến + 5 case studies** — Samsung, 1STOPlighting, Traveloka, David Jones, Campmor.
8. **Tài nguyên + lộ trình 3/6/12 tháng** — 8 nguồn chính thức + 3 việc làm ngay.
9. **References** — 55 footnote (đã cảnh báo lỗi gắn sai).

## 🧱 Phần 1+2 — Tư duy gốc + Bản đồ yếu tố

### Đúng thứ tự bắt buộc (gốc dòng 3)

```
Mục tiêu kinh doanh → conversion goal → tracking 
→ loại chiến dịch → cấu trúc tài khoản 
→ quảng cáo/tài sản → landing page → bidding → tối ưu
```

### Sai lầm lớn nhất (gốc dòng 9)
Coi Google Ads là công cụ **mua traffic**.
**Đúng**: mua **xác suất chuyển đổi có lợi nhuận**. Campaign tốt KHÔNG phải campaign CTR cao nhất, mà là campaign đưa được **conversion / conversion value đúng mục tiêu** với CPA/ROAS phù hợp.

### Cấu trúc 3 lớp (gốc dòng 10)
**Account → Campaign → Ad group**. Cấu trúc Search hiện đại nên **ĐƠN GIẢN, gộp theo chủ đề chặt**. Cấu trúc vụn = báo cáo mờ, khó học máy, dễ sai sót.

**Performance Max** thêm khái niệm **asset group** — ghép headline, description, image, logo, video, audience signals thành nhiều tổ hợp ad.

### Bản đồ 16 yếu tố (gốc dòng 11-68)

| # | Yếu tố | Câu hỏi | Quy tắc người mới |
|---|---|---|---|
| 1 | Mục tiêu chiến dịch | Sale/lead/traffic/awareness? | Mỗi campaign chỉ 1 mục tiêu chính |
| 2 | Conversion goals | Hệ thống bid cho hành động nào? | Chỉ đặt Primary cho hành động thật sự có giá trị kinh doanh |
| 3 | Loại chiến dịch | Search/Display/Video/Shopping/PMax? | Chọn theo nguồn cầu + mức sẵn sàng mua |
| 4 | Cấu trúc tài khoản | Tách campaign theo gì? | Theo mục tiêu/ngân sách/địa lý/intent — không tách vô tội vạ |
| 5 | Keywords | Người dùng gõ gì? | Bắt đầu nhóm từ khoá ý định cao, bổ sung broad match có kiểm soát sau |
| 6 | Negative keywords | Loại bỏ truy vấn nào? | Review search terms đều đặn; negative KHÔNG tự loại synonym/plural như positive |
| 7 | Audiences | Người lạ hay đã biết? | Search lạnh dùng keyword; remarketing dùng data segments, Customer Match, RLSA |
| 8 | Targeting / Observation | Nhắm thật hay quan sát? | Search/Shopping người mới nên dùng Observation trước để học |
| 9 | Bidding | Tối ưu click/conversion/value? | Có tracking sạch → Smart Bidding; chưa sạch → sửa tracking trước |
| 10 | Ngân sách | Mỗi ngày bao nhiêu? | Ngân sách = "nhiên liệu"; bid strategy = "hộp số". Đừng đổi cả hai liên tục |
| 11 | Lịch chạy | Chạy giờ nào? | Dùng ad schedule khi có lý do vận hành/dữ liệu rõ |
| 12 | Creatives & assets | Ad đủ mạnh? | Search ≥ 2 RSA/ad group; thêm assets đầy đủ, đặc biệt sitelinks |
| 13 | Landing page | Trang đích khớp thông điệp? | Ad nói gì, landing page cho thấy đúng đó + CTA rõ |
| 14 | Tracking | Đo đúng? | Đo sai → mọi báo cáo sau đều không đáng tin |
| 15 | Privacy/consent | Có quyền dùng data? | Consent mode chỉ truyền tín hiệu đồng ý; KHÔNG tự tạo banner xin đồng ý |
| 16 | Remarketing | Đủ data bám đuổi? | Tag mọi trang, audience logic đúng, kiểm tra list size + reach |

### Quality Score vs Ad Rank (gốc dòng 69)

| Khái niệm | Định nghĩa | Cấu thành |
|---|---|---|
| **Quality Score** (Search) | Điểm chất lượng cho từng từ khoá, thang **1-10** | Expected CTR + Ad Relevance + Landing Page Experience |
| **Ad Rank** | Cơ chế quyết ad có hiển thị + đứng đâu | Bid + chất lượng ad/landing + thresholds + cạnh tranh auction + ngữ cảnh truy vấn + impact assets/formats |

**Chất lượng tốt hơn không chỉ tăng vị trí** — còn có thể **giảm CPC thực tế** + **tăng khả năng hiển thị assets**.

→ Chi tiết: [[Quality Score vs Ad Rank]].

## 🎯 Phần 3 — So sánh 5 loại campaign

### Bảng đầy đủ (gốc dòng 70-107)

| Loại | Phù hợp khi | Tín hiệu chính | Điểm mạnh | Điểm yếu | Vai trò remarketing |
|---|---|---|---|---|---|
| **Search** | Bắt nhu cầu có sẵn | Keywords, ads, landing page, bids | Ý định cao, đo lường rõ, mạnh cho lead/sale | Volume phụ thuộc nhu cầu tìm; lãng phí nếu keyword rộng + thiếu negatives | Rất mạnh với RLSA + brand protection |
| **Display** | Mở rộng reach hoặc bám đuổi | Audiences, placements, images, copy | CPM/CPC thường rẻ, tốt cho remarketing + awareness | Ý định lạnh; creative kém → đốt tiền nhanh | Kênh remarketing rất hữu ích |
| **Video** | Kể chuyện, tăng nhớ thương hiệu | Video asset, audience, YouTube inventory | Thuyết phục tốt, mạnh ở mid-funnel + retargeting | Cần asset video đủ tốt; direct response lạnh thường khó hơn Search | Tốt để nuôi nóng audience + bám đuổi YouTube |
| **Shopping** | Bán sản phẩm có feed | Merchant Center feed, giá, ảnh, title, bids | Click "chất" hơn vì người dùng thấy giá/ảnh trước khi click | Feed kém = campaign kém; title/attributes sai → mất hiển thị | Là nền để làm dynamic remarketing retail |
| **Performance Max** | Scale conversion/value đa kênh | Conversion goals, assets, audience signals, feed (nếu có) | Phủ đa inventory từ 1 campaign, tận dụng Google AI mạnh | Ít đòn bẩy thủ công hơn; tracking, values, assets phải sạch | Rất mạnh cho remarketing mở rộng + retail |

### Khuyến nghị thực chiến (gốc dòng 108)

- **Lead gen + ngân sách hạn chế** → Search non-brand high intent trước → thêm remarketing Search/Display/Video.
- **E-commerce** → ưu tiên **Shopping hoặc Performance Max** có feed sạch, NHƯNG vẫn giữ Search brand/non-brand để kiểm soát nhu cầu ý định rõ.
- **Awareness** → Video + Display vai trò lớn hơn, nhưng muốn bán hàng ngay vẫn nên có Search hoặc feed-based campaigns làm trục chính.

→ Tác giả nói rõ: **"đây là khuyến nghị suy luận, KHÔNG phải luật cứng cho mọi ngành"**.

## 📋 Phần 4 — Quy trình 11 bước cho người mới

| Bước | Việc | Xong khi nào | Sai thường gặp |
|---|---|---|---|
| 1 | Tạo Google Ads, chọn múi giờ/tiền tệ/billing | Time zone/currency đúng từ đầu | Đặt sai múi giờ → báo cáo lệch |
| 2 | Tạo GA4 property + web data stream | Có Measurement ID + data vào Realtime | Tạo xong nhưng chưa gắn code |
| 3 | Cài tag (GTM hoặc Google tag) toàn site | Tag Assistant/GTM Preview thấy tag bắn đúng | Chỉ gắn ở homepage |
| 4 | Liên kết Ads–GA4 | Data Ads xuất hiện trong GA4 | Link sai property/account |
| 5 | Định nghĩa conversions từ Google tag/GA4 events | ≥1 primary conversion đúng business goal | Đẩy "view page", "scroll" vào primary |
| 6 | Consent banner + consent mode | Tín hiệu consent gửi hợp lệ | Nghĩ consent mode tự tạo banner |
| 7 | Theo dõi hành vi (view_item, ATC, begin_checkout, purchase, lead) | Event map đúng logic funnel | Thiếu value, currency, item IDs |
| 8 | Nghiên cứu từ khoá + negative list | Có bộ keyword cốt lõi + loại trừ rõ | Trộn brand + non-brand cùng nhóm |
| 9 | Viết ads/assets — RSA, sitelinks, callouts, hình/video | Search có **2 RSA/ad group, ≥4 sitelinks** | Copy chung chung, không bám landing |
| 10 | Tạo audience remarketing — Website visitor lists, GA4 audiences, Customer Match | Audience Manager xuất hiện list + có size | List quá nhỏ hoặc logic sai |
| 11 | Launch + QA — bid strategy, budget, ad schedule | Campaign eligible + bắt đầu nhận data | Bật mọi network/campaign cùng lúc |

### Ghi chú quan trọng — "Conversion API" cho Google (gốc dòng 163)

⚠️ **KHÔNG có 1 tính năng tên "Conversion API" như Meta**. Triển khai tương đương Google = tổ hợp:
- Google tag/GTM
- Server-side tagging
- Enhanced Conversions
- Google Ads API/Data Manager

→ "Cài Conversion API cho Google" phải DỊCH thành hành động kỹ thuật cụ thể, không chạy theo cái tên.

### Sơ đồ luồng đo lường + remarketing chuẩn (gốc dòng 164-165)

```
Banner xin đồng ý → Consent mode → GTM/Google tag → 
GA4 events + Google Ads conversions

GA4 events → GA4 audiences → Publish sang Google Ads
Google Ads conversions → Data segments trong Google Ads
CRM/offline sales → Data Manager hoặc Google Ads API → Google Ads conversions
Merchant Center/feed → Dynamic remarketing

Audiences + Data segments + Feed → Dynamic remarketing → 
Search/Display/Video/PMax remarketing
```

### Timeline 30 ngày (gốc dòng 166-184)

| Giai đoạn | Trọng tâm | Output |
|---|---|---|
| **Ngày đầu** | Tạo account, GA4, GTM/tag, link Ads-GA4 | Hệ đo lường chạy được, data có vào |
| **Tuần đầu** | Conversions, consent mode, cross-domain (nếu cần), QA tag | 1 primary conversion sạch, KHÔNG duplicate |
| **Tuần 2** | Keyword research, landing page, viết ads/assets, mở Search cốt lõi | Campaign đầu live, có traffic đúng intent |
| **Tuần 3** | Soát search terms, thêm negatives, sửa ads + landing, tạo audiences | CTR/CVR/CPA bắt đầu có tín hiệu |
| **Tuần cuối** | Mở remarketing, thêm experiments/automation đơn giản, chuẩn hoá báo cáo KPI | Có baseline so sánh tuần/tháng sau |

→ Logic timeline: **buộc khoá tracking trước khi scale bidding**.

## 🧮 Phần 5 — Công thức + Checklist + Templates

### 9 công thức KPI (gốc dòng 185-216)

| Chỉ số | Công thức |
|---|---|
| **CTR** (chuẩn Google) | Clicks / Impressions |
| **Conversion rate** | Conversions / Interactions |
| **CPA** | Cost / Conversions |
| **ROAS** | Conversion value / Ad spend × 100% |
| **LTV/CLV heuristic** | AOV × Purchase frequency × Gross margin × Customer lifespan |
| **Break-even ROAS** | 1 / Biên LN gộp × 100% |
| **Break-even CPA lead gen** | Lợi nhuận gộp/sale × Tỷ lệ chốt lead→sale × Tỷ lệ ngân sách marketing cho phép |
| **Trần CPC thủ công** | Target CPA × Conversion rate × hệ số an toàn |
| **Ngân sách ngày** | CPA mục tiêu × số conversion mong muốn mỗi ngày |

⚠️ **4 công thức đầu là CHUẨN GOOGLE chính thức**; các công thức sau là **heuristic của báo cáo** — không phải con số chính thức Google ban hành.

### 3 kịch bản ngân sách (gốc dòng 217-229)

| Kịch bản | Dấu hiệu | Cách triển khai |
|---|---|---|
| **Thấp** | Daily < 3× CPA mục tiêu HOẶC click volume còn ít | Search intent cao, structure đơn giản, chưa mở quá nhiều network |
| **Trung** | Daily ~ 3-10× CPA mục tiêu | Thêm remarketing, broad match có kiểm soát, Smart Bidding rõ mục tiêu |
| **Bão hoà** | Budget bắt đầu limit campaign thắng, impression share gần trần | Experiments, PMax/Shopping mạnh hơn, value-based bidding, feed segmentation, creative rotation |

⚠️ Đây là **quy ước thực hành của báo cáo**, KHÔNG phải ngưỡng chính thức Google.

### Naming convention campaign

| Cấp | Template | Ví dụ TPCN *(em — agent — chỉnh từ ví dụ ngành xăm gốc)* |
|---|---|---|
| Campaign | `[QuốcGia]_[Network]_[Intent/Offer]_[Goal]_[Geo]` | `VN_Search_NonBrand_Collagen_Lead_HN` |
| Ad group | `[Theme]_[Subtype]` | `collagen_phu_nu_35` |
| Remarketing | `[QuốcGia]_RMKT_[Network]_[Audience]_[Goal]` | `VN_RMKT_Display_CartAbandon_Purchase` |
| Shopping/PMax | `[QuốcGia]_[Type]_[Feed/Portfolio]_[Goal]` | `VN_PMax_Feed_FullCatalog_Purchase` |

### Mẫu landing page — 8 khối theo thứ tự (gốc dòng 246-264)

1. **Hero** — Headline bám đúng từ khoá/nhu cầu.
2. **Proof** — Review, chứng chỉ, con số tin cậy.
3. **Offer** — Giá, quà, USP rõ.
4. **Fit** — Sản phẩm/dịch vụ phù hợp cho ai.
5. **Friction-killers** — Giao hàng, bảo hành, đổi trả, hỗ trợ.
6. **CTA** — Form, call, chat, mua ngay.
7. **FAQ** — Xử lý phản đối trước khi rời trang.
8. **Technical trust** — Chính sách, bảo mật, tốc độ, mobile-friendly.

→ Ghi chú PTL: landing page phải phản ánh đúng thông điệp ad, có CTA rõ, đưa người dùng đến đúng trang liên quan.

### Mẫu tracking plan tối thiểu — 9 events (gốc dòng 265-315)

| Event | Nền tảng | Tham số tối thiểu | Dùng cho | Primary/Secondary |
|---|---|---|---|---|
| `page_view` | GA4 | `page_location` | QA traffic | Secondary |
| `view_item` | GA4 / Ads | `item_id, value, currency` | Remarketing động, funnel | Secondary |
| `add_to_cart` | GA4 / Ads | `item_id, value, currency` | Mid-funnel, audience nóng | Secondary |
| `begin_checkout` | GA4 / Ads | `value, currency, items` | Remarketing checkout | Secondary |
| `purchase` | GA4 / Ads | `transaction_id, value, currency, items` | Doanh thu thật | **Primary** |
| `generate_lead` | GA4 / Ads | `form_id, lead_type, value` | Lead online | **Primary** |
| `phone_click` | GA4 | `link_url, page_location` | Phụ trợ | Secondary |
| `qualified_lead` | Ads import/API | `gclid` hoặc hashed user data | Offline quality signal | **Primary** |
| `closed_sale` | Ads import/API | `value thật, order_id, timestamp` | Bidding theo giá trị thật | **Primary** |

## 🔁 Phần 6 — Remarketing + Kỹ thuật nâng cao

### Basic remarketing (gốc dòng 317)

- Đặt **Google tag toàn trang** → đưa user vào data segments → dùng segment trên Search/Display/Video.
- **Điều kiện phục vụ tối thiểu: 100 active users trong 30 ngày gần nhất** (Display, Search, YouTube).
- **Customer Match** cùng điều kiện cơ bản này.
- → Remarketing KHÔNG nên là campaign đầu tiên duy nhất của site mới.

### Audience layering — Targeting vs Observation (gốc dòng 318)

- **Observation**: xem audience nào đang chuyển đổi tốt mà KHÔNG bó hẹp reach.
- **Targeting**: chỉ phục vụ nhóm đó.
- Search/Shopping người mới → dùng **Observation** trước.
- Data segments trên Search có thể: tăng bid, đổi ad copy, chọn keyword phù hợp với người đã ghé site.

### RLSA — Remarketing Lists for Search Ads (gốc dòng 319)

- Giữ campaign Search chính bắt nhu cầu lạnh → thêm audience chế độ Observation để học → đủ data thì tạo campaign/ad group riêng cho user quay lại, tăng bid hoặc nới keyword.
- **RLSA KHÔNG thay Search bằng audience** — nó **ghép ý định hiện tại với hành vi quá khứ**.

### Dynamic Remarketing (gốc dòng 320)

- Mạnh nhất khi có nhiều SKU/dịch vụ + người dùng thường bỏ dở.
- Yêu cầu feed sản phẩm chứa **ID, giá, ảnh, thuộc tính**.
- Retail → feed ở **Merchant Center**; non-retail → feed ở **Business data**.
- **Feed sai = dynamic remarketing vô dụng.**

### Customer Match (gốc dòng 321)

- Vũ khí mạnh nhưng phải có **consent + policy**.
- Google áp chính sách riêng + yêu cầu consent cho ad personalization ở thị trường liên quan.
- Pháp lý + lịch sử tuân thủ tài khoản ảnh hưởng quyền dùng.
- **Không chắc nguồn CRM đủ đồng ý quảng cáo → đừng upload.**

### Smart Bidding — 4 tips (gốc dòng 322)

1. Dùng cùng **account-default goals** ở phần lớn campaign → cross-campaign learning.
2. Tối ưu cho conversion value → truyền **value thật**, không chỉ đếm số.
3. Đổi bid strategy/goal → đừng đánh giá sau **2-3 ngày**. Cần ít nhất vài chu kỳ chuyển đổi.
4. **Seasonality adjustments** chỉ dành biến động ngắn hạn dự đoán trước (vd sale 3 ngày). KHÔNG dùng để sửa vấn đề cấu trúc dài hạn.

→ Chi tiết: [[Smart Bidding (Google)]].

### Performance Max (gốc dòng 323) — 6 đòn bẩy

- Phải "steer" bằng dữ liệu đầu vào, không ép bằng tay.
- **Audience signals = tín hiệu gợi ý**, KHÔNG phải khoá cứng.

**6 đòn bẩy thật cho PMax**:
1. Goal đúng
2. Value đúng
3. Asset group theo chủ đề rõ
4. Feed sạch
5. Custom labels tốt
6. Audience signals bám first-party data chất lượng

### Scripts/rules/API theo tầng (gốc dòng 324)

- **Automated rules** → điều kiện đơn giản (pause ad, chỉnh budget/bid theo ngưỡng).
- **Scripts** → logic tuỳ chỉnh bằng JavaScript (pause ad groups, thêm keywords, gửi alert).
- **Google Ads API** → quy mô lớn, đồng bộ CRM, upload conversion, tự động hoá sâu.
- ⚠️ **Rule sai dễ sửa, script sai có thể phá cả account nhanh hơn**.

### Offline Conversion Import (gốc dòng 325) — BẮT BUỘC cho lead gen

- Mô hình lead có doanh thu thật xảy ra sau điện thoại, tư vấn, chốt hợp đồng.
- Google hỗ trợ import bằng **GCLID**.
- Khuyến nghị nâng cấp lên **Enhanced Conversions for Leads** vì:
  - Dùng first-party data đã hash, bền hơn về privacy.
  - Hỗ trợ tốt hơn cho reporting, engaged-view, cross-device conversions.
- KHÔNG mang offline data về Google Ads = đang tối ưu cho **lead số lượng**, không phải **lead chất lượng**.

### Cross-device + Cross-domain (gốc dòng 326)

- User đi từ domain bán hàng sang domain thanh toán khác → phải cấu hình **cross-domain trong GA4**.
- Bật **Google signals** để nhận diện đa thiết bị.

### Budget allocation (gốc dòng 327)

- **Performance Planner** → mô hình hoá phân bổ bid/budget.
- **Shared budgets + Portfolio bid strategies** = best practice khi nhiều campaign cùng mục tiêu.
- Campaign liên tục **"Limited by budget"** → tín hiệu xem lại phân bổ, KHÔNG phải cứ ép bid lên.

### Anomaly Detection (gốc dòng 328)

- Bật sớm ở **GA4**.
- GA4 hỗ trợ **anomaly detection, automated insights, custom insights** — gửi email alert.
- Cách rẻ nhất phát hiện sớm rớt conversion, mất traffic, tracking lỗi.

## 🚨 Phần 7 — 11 lỗi phổ biến + 5 case studies

### 11 lỗi phổ biến (gốc dòng 329-363)

| Lỗi | Sai ở đâu | Sửa |
|---|---|---|
| Mở ads trước khi cài tracking | Không biết cái gì tạo ra tiền | Khoá 1 primary conversion thật rồi mới scale |
| Để micro-conversions làm Primary | Hệ thống học sai mục tiêu | Chuyển micro thành Secondary |
| Tách account quá vụn | Dữ liệu loãng, quản trị rối | Gộp theo theme chặt, mục tiêu rõ |
| Trộn brand và non-brand | KPI bị đẹp giả | Tách riêng để đọc intent thật |
| Không thêm negatives | Click rác tăng | Review search terms theo lịch cố định |
| Ad nói 1 đằng, landing page 1 nẻo | Quality Score thấp, CVR thấp | Đồng bộ headline–offer–CTA |
| Remarketing list quá nhỏ | Ads không serve được | Mở Search trước nuôi list |
| Đổi bid, budget, ad, landing cùng lúc | Không biết cái gì gây thay đổi | Mỗi lần đổi 1 biến chính |
| Feed sản phẩm nghèo nàn | Shopping/PMax học sai | Sửa title, image, price, custom labels |
| Sốt ruột với Smart Bidding | Chưa qua conversion cycle đã kết luận | Chờ đủ chu kỳ + đủ data |

### 5 case studies (gốc dòng 365-369)

| Case | Setup | Kết quả | Bài học |
|---|---|---|---|
| **Samsung Electronics** | Test "Display+Discovery" vs "Display+Discovery+PMax" | **2.5× conversions, -60% cost/conversion, CTR ×2** | PMax mạnh khi đi trên nền campaign đang chạy tốt — không phải "viên đạn bạc" cho account còn non |
| **1STOPlighting** | Chuyển toàn bộ Shopping → **Target ROAS** | **Profit +214%** | Mỗi conversion có value khác — tối ưu theo value đúng bản chất hơn theo count |
| **Traveloka** | A/B test "DSA + Target CPA" vs "DSA + Target ROAS + first-party profile" | **ROAS +11%, AOV booking +14%, cost/booking -5%** | Search automation mạnh hơn nhiều khi nuôi bằng first-party data + conversion value |
| **David Jones** | Triển khai **RLSA + GDN dynamic + Shopping RLSA** | **ROAS +286%, CVR +642%**; riêng Shopping RLSA: **CVR +97%, ROAS +72%** | Remarketing mạnh nhất khi chia theo tầng trong funnel |
| **Campmor** *(bonus)* | Dynamic Remarketing vs static | **CTR +300%, cost/conv -37%**; mở rộng ~100 list mới mùa sale | Dynamic remarketing chỉ thật sự bùng nổ khi feed, tag, audience logic chuẩn hoá sớm |

⚠️ **Footnote citation cho 5 case này gắn SAI trong gốc** ([34], [36], [38], [40], [42] đúng — không phải [33]/[35]/[37]/[39]/[41]). Anh muốn tra cứu nguồn → search "Samsung Performance Max case study Google Ads" trực tiếp.

## 🎓 Phần 8 — Tài nguyên + Lộ trình + 3 việc làm ngay

### 8 nguồn ưu tiên chính thức

1. **Skillshop tiếng Việt** — Google Ads + chứng chỉ.
2. **Google Ads Help** — chọn loại campaign.
3. **Google Ads Help** — conversions, goals, Smart Bidding, experiments.
4. **GA4 Help** — link Ads-Analytics, attribution, Google signals, cross-domain.
5. **Tag Manager Help** — GTM, preview/debug, consent mode, server-side.
6. **Merchant Center Help** — product data + feed setup.
7. **Advertising Policies Help** — destination, personalized ads, Customer Match.
8. **Case studies chính thức** — học cấu trúc + logic, không chỉ nhìn con số.

### Lộ trình 0 → chuyên gia 12 tháng

| Giai đoạn | Mục tiêu | Milestones | Bài tập |
|---|---|---|---|
| **3 tháng** | Hiểu nền tảng + launch 1 hệ Search + tracking sạch | Tự cài GA4 + GTM + conversions; tách brand/non-brand; báo cáo CPA/ROAS cơ bản | 1 account demo: 1 Search campaign + 1 remarketing + 1 landing page |
| **6 tháng** | Tối ưu lợi nhuận, không chỉ traffic | Primary/secondary đúng; remarketing; đọc search terms, auction insights, experiments | Test ad copy hoặc landing; thêm dynamic remarketing/Shopping/PMax (nếu có feed) |
| **12 tháng** | Làm chủ automation + measurement nâng cao | Scripts/rules/API; offline import; value-based bidding, seasonality, anomaly alerts | Tracking plan đầy đủ + nối CRM offline + 1 experiment có đối chứng |

### 3 việc làm ngay (gốc dòng 397-400)

1. **Khoá hệ đo lường trước khi khoá ngân sách**:
   - **Đúng**: 1 primary conversion duy nhất, tag bắn 1 lần cho 1 hành động, GA4-Ads link, consent signals hợp lệ.
   - **Sai**: thấy có click là chạy.
2. **Mở cấu trúc đơn giản nhưng đọc được**:
   - **Đúng**: tách brand/non-brand, 1-3 campaign theo mục tiêu, mỗi ad group 1 theme chặt, 2 RSA/ad group + ≥4 sitelinks.
   - **Sai**: gom mọi thứ vào 1 campaign hoặc tách vụn quá mức.
3. **Sau 7-14 ngày, tối ưu theo dữ liệu**:
   - **Đúng**: search terms, thêm negatives, kiểm landing match, audience reach, anomaly, **chỉ đổi 1 biến lớn mỗi lần**.
   - **Sai**: đổi bid + ngân sách + ad + geo + landing cùng lúc.

## 💬 Trích dẫn

> "Smart Bidding không chữa được tracking sai." *(dòng 6)*

> "Bid sai còn dễ sửa, script sai có thể phá cả account." *(dòng 324)*

> "Ngân sách là nhiên liệu; bid strategy là hộp số." *(dòng 44)*

> "Feed kém là campaign kém." *(dòng 100)*

> "Mỗi campaign chỉ nên có một mục tiêu chính." *(dòng 17)*

## 🔗 Liên kết

- [[Khối 14 - ADS Các nền tảng]] — page mẹ
- [[Smart Bidding (Google)]] — concept đặc thù
- [[Quality Score vs Ad Rank]] — nền tảng Google
- [[3 loại Conversion Click-Engaged-View-View-Through]] — quan trọng cho Display/Video
- [[Khung diagnose phễu]] — debug
- [[Khối 13 - SEO sản phẩm Website]] — feed Merchant Center cho Shopping
- [[UTM template chuẩn 4 nền tảng]]
