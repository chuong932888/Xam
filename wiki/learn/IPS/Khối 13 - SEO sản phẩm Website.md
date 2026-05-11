---
type: source
tags: [ips, khoi-13, seo, website, san-pham, on-page, schema, cwv, ptl]
created: 2026-05-09
updated: 2026-05-09
sources: ["[[raw/Đặc sản của Phạm Thành Long/IPS - 19 khối công việc/13_ SEO sản phẩm Website.docx]]"]
khoi: 13
---

# Khối 13 — SEO sản phẩm Website

> Nguồn: thầy [[Phạm Thành Long]], khoá [[index|IPS]]. File gốc: 1 file docx, 113 paragraphs không rỗng (bao gồm footnotes) + 10 bảng (92 rows tổng cộng).

> ⚠️ **Phân biệt nguồn — đọc trước khi dùng**:
> - Page **này** bám sát PTL gốc. Mọi thông tin gắn "✅ PTL" là trực tiếp từ file gốc.
> - Phần **Áp dụng cho TPCN** là do agent suy luận — gắn "📎 em thêm", KHÔNG có trong tài liệu gốc.
> - File gốc **dùng ví dụ ngành dụng cụ xăm** ở Bảng 4 (trước/sau tối ưu) — theo quy tắc 2 CLAUDE.md, bảng này KHÔNG được lưu vào vault. Wiki ghi chú cấu trúc bảng (12 hạng mục: URL/Title/H1/Above fold/Mô tả ngắn/Mô tả sâu/Video/Review/FAQ/Schema/Internal links/Trust) nhưng không lưu nội dung ví dụ xăm cụ thể.
> - File gốc có **10 bảng** (không phải 9): Table 0 Giả định, Table 1 Checklist P0/P1/P2, Table 2 Audit, Table 3 Khung 13 thành phần, Table 4 Trước/Sau (xăm — không lưu), Table 5 Công cụ, Table 6 KPI, Table 7 Vận hành, Table 8 Dashboard, Table 9 Câu hỏi mở.
> - Chiến lược từ khóa 4 tầng trong gốc là **văn xuôi** (paragraph [33]), không phải bảng — wiki chuyển thành bảng để dễ đọc, logic giữ nguyên 100%.
> - File gốc có **39 footnote** trích dẫn URL Google Developers — đầy đủ ở mục "Nguồn trích dẫn" cuối file này.
> - Khối 13 (SEO sản phẩm) khác Khối 9 (SEO Blog): Khối 9 tối ưu bài blog/content cluster; Khối 13 tối ưu trang sản phẩm/category/landing page bán hàng.

---

## 🎯 TL;DR — Đọc 5 phút hiểu toàn bộ

✅ PTL — **Một câu cốt lõi của toàn bộ Khối 13**:

> "Muốn web đạt 10/10 và muốn sản phẩm có cơ hội lên Top 1, bạn phải làm đúng thứ tự: khả năng được crawl và index trước, cấu trúc và dữ liệu trước, rồi mới đến nội dung, UX và tăng trưởng chuyển đổi."

**3 hiểu lầm phổ biến tài liệu PTL phá vỡ**:
1. "Cứ viết nhiều bài là lên Top" → Sai. Phần lớn web thua vì **Google không hiểu đúng trang nào quan trọng**, không phải vì thiếu bài.
2. "Có thể hứa Top 1" → Không. Google tuyên bố chính thức không nhận tiền để crawl nhiều hơn hay xếp hạng cao hơn. Mục tiêu đúng: **tăng xác suất vào Top 3** cho từ khóa giá trị kinh doanh cao nhất, rồi tối ưu CTR và conversion.
3. "SEO 2026 có bí kíp riêng cho AI Overviews" → Không. Google xác nhận: **các thực hành SEO nền tảng vẫn áp dụng cho AI Overviews và AI Mode**. Không có yêu cầu kỹ thuật riêng.

**6 đòn bẩy lớn nhất** (✅ PTL — đây là khoảng trống của hầu hết website bán hàng):
1. Indexation hygiene (vệ sinh lập chỉ mục)
2. Cấu trúc site và internal linking
3. Schema sản phẩm + feed Merchant Center
4. Page speed và Core Web Vitals
5. Media và review (tăng niềm tin)
6. Tối ưu title/snippet để tăng CTR

---

## 1. Giả định và phạm vi tài liệu PTL

✅ PTL — Bảng giả định chuẩn mà tài liệu xây trên đó:

| Hạng mục | Giả định |
|---|---|
| Loại website | Website thương mại điện tử hoặc website bán hàng có trang danh mục và trang sản phẩm |
| Quy mô | 200–5.000 URL indexable, 100–1.000 sản phẩm |
| Thị trường chính | Việt Nam, mobile-first, 1 ngôn ngữ chính; có thể mở rộng đa ngôn ngữ sau |
| Hạ tầng phổ biến | Shopify, WooCommerce, Haravan hoặc web custom có khả năng sửa template |
| Nguồn lực tối thiểu | 1 SEO lead, 1 dev part-time, 1 content, 1 designer/media part-time |
| Ngân sách tham chiếu | Trung bình; ưu tiên stack công cụ tinh gọn trước, chưa giả định enterprise SEO |

> Lưu ý PTL: "Nếu website của bạn không phải e-commerce thuần, hãy thay 'trang sản phẩm' bằng 'trang dịch vụ / offer page / landing page bán hàng'; logic về crawl, index, intent, CTR, trust và CRO vẫn giữ nguyên."

---

## 2. SEO website đạt 10/10 — Nền tảng kỹ thuật

### 2.1 Điều kiện "10/10" là gì?

✅ PTL — Website chỉ đáng gọi "10/10" khi **thỏa đủ 6 điều kiện cùng lúc**:
1. Google crawl được
2. Index đúng
3. Hiểu đúng
4. Người dùng dùng tốt
5. Trang an toàn và nhanh
6. Dữ liệu đo lường đủ sạch để ra quyết định

✅ PTL — **Kỹ thuật tối thiểu** Google nêu rõ: bot không bị chặn + trang trả về HTTP 200 + có nội dung có thể index. Thiếu 1 trong 3 → mọi nỗ lực nội dung phía trên gần như bị vô hiệu hóa.

### 2.2 Crawlability và Indexability (Lớp nền đầu tiên)

✅ PTL:
- **robots.txt** chỉ dùng để hướng dẫn crawler; KHÔNG phải cơ chế để deindex.
- Muốn trang biến khỏi Google → dùng **noindex** hoặc bảo vệ bằng đăng nhập/mật khẩu.
- **Lỗi phổ biến nhất**: vừa block filter trong robots, vừa mong các URL đó tự biến khỏi index — không thể xảy ra vì bot không vào được thì không nhìn thấy chỉ thị noindex.
- **Canonical** là cơ chế hợp nhất tín hiệu giữa các URL trùng hoặc gần trùng — đặc biệt quan trọng cho: biến thể màu/kích cỡ, phân trang, tracking parameter, session ID.
- Với biến thể qua query parameter → Google khuyến nghị dùng URL không có query parameter làm canonical.
- Internal link nên trỏ nhất quán về canonical URL.
- **Hreflang**: chỉ cần khi thật sự có nhiều phiên bản ngôn ngữ/vùng địa lý. Lỗi hay gặp: canonical trỏ chéo ngôn ngữ hoặc thiếu self-reference.
- **Sitemap**: là "hint" gợi ý, không bảo đảm index. Tách ít nhất 4 sitemap logic: danh mục, sản phẩm, bài viết, hình ảnh/video. KHÔNG nhét URL noindex, redirect, 404, canonical không-self vào sitemap.

### 2.3 Cấu trúc site và Internal Linking

✅ PTL — "Đòn bẩy bị đánh giá thấp nhất":
- Google dùng mối quan hệ liên kết để hiểu **cấu trúc site và mức độ quan trọng tương đối** của từng trang.
- Cấu trúc chuẩn: menu → category → subcategory → product. Category phải có đường dẫn tới toàn bộ sản phẩm cần index.
- Googlebot **không tự gõ vào ô tìm kiếm nội bộ** → sản phẩm chỉ tìm thấy qua search box mà không có link danh mục/sitemap/feed → rất dễ bị mồ côi.
- Link phải là thẻ `<a href>` crawlable. Đừng dựa hoàn toàn vào JS event trên button/div.

### 2.4 Phân trang, lọc, sắp xếp

✅ PTL:
- Google chủ yếu crawl URL trong `href` của thẻ `<a>`, **không "click button"** hay kích hoạt tương tác JavaScript như người dùng.
- **Infinite scroll và "load more"** vẫn phải có URL crawlable phía dưới.
- Mỗi trang pagination phải có URL riêng + liên kết tuần tự + canonical của chính nó (không dùng trang đầu làm canonical cho toàn bộ chuỗi).
- Biến thể lọc/sort tạo danh sách trùng → kiểm soát bằng noindex hoặc robots.
- Google **không còn dùng rel=next/prev** để hiểu phân trang.

### 2.5 Mobile-first

✅ PTL:
- Google dùng **phiên bản mobile** của nội dung để index và xếp hạng.
- Nếu mobile thiếu nội dung/metadata/structured data/gắn noindex/chặn ảnh → mất traffic dù desktop ổn.
- Quy tắc: nội dung chính, robots meta, structured data, internal links, tài nguyên quan trọng trên **mobile phải ngang với desktop**.

### 2.6 JavaScript SEO

✅ PTL:
- Google có thể xử lý JavaScript, nhưng qua các pha: crawl → render → index. Render **không tức thời**.
- Google khuyến nghị **server-side rendering hoặc pre-rendering** vẫn là ý tưởng tốt.
- Không thay canonical lung tung bằng script; không lazy-load nội dung chính sau thao tác người dùng; không để rendering phụ thuộc vào CSS/JS bị block.
- File tĩnh dài hạn → nên **fingerprint** để tránh Googlebot dùng nhầm tài nguyên cũ.

### 2.7 Page Experience, Tốc độ và Bảo mật

✅ PTL:
- Không có một "page experience signal" duy nhất. **Core Web Vitals** là phần được dùng trong xếp hạng nhưng không đủ một mình.
- Ngưỡng Core Web Vitals hiện hành:
  - **LCP** ≤ 2,5 giây
  - **INP** ≤ 200 ms
  - **CLS** ≤ 0,1
  - Tại ngưỡng **75th percentile**
- Page experience tốt gồm: CWV tốt + HTTPS + hiển thị tốt trên mobile + không lạm dụng quảng cáo + không dùng interstitial gây khó chịu + bố cục giúp phân biệt nội dung chính với phần phụ.
- **Search Console** báo cáo CWV bằng field data từ người dùng thực (PSI: 28 ngày). Lab data như Lighthouse hữu ích để debug nhưng không thay thế field data.

### 2.8 Structured Data (Schema) — Vai trò đúng

✅ PTL:
- Có schema đúng **không bảo đảm** sẽ hiện rich result. Google nhắc rõ điều này.
- Quy trình đúng: thêm markup → validate bằng Rich Results Test → kiểm tra bằng URL Inspection → theo dõi báo cáo structured data trong Search Console.
- Schema theo cấp trang:
  - Trang chủ: **WebSite**
  - Site navigation: **BreadcrumbList**
  - Category: **ItemList** (nếu hợp lý)
  - Product page: **Product** + dữ liệu offer/review phù hợp

→ Xem chi tiết schema sản phẩm ở mục 3.3 bên dưới và concept [[Schema]].

### 2.9 Đo lường KPI

✅ PTL — Tối thiểu phải có:
- **Search Console**: clicks, impressions, CTR, position theo query/page/device/country.
- **Analytics**: funnel thương mại điện tử đầy đủ.
- **Dashboard**: hợp nhất dữ liệu SEO với dữ liệu chuyển đổi (khuyến nghị dùng Looker Studio).

---

## 3. SEO trang sản phẩm lên Top

### 3.1 Triết lý tối ưu trang sản phẩm

✅ PTL:
- Bỏ tư duy "nhét từ khóa vào title" → chuyển sang: **match đúng intent + làm rõ thông tin mua hàng + tăng mức tin cậy + giảm ma sát quyết định**.
- Google chỉ xếp hạng cao một trang sản phẩm khi trang đó **vừa đủ liên quan với truy vấn, vừa đủ rõ cho máy hiểu, vừa đủ thuyết phục cho người mua ở lại**.
- Trang thiếu giá, thiếu tồn kho, thiếu media, thiếu biến thể, thiếu review, thiếu liên kết nội bộ, thiếu tín hiệu trust → **gần như không đủ lực giữ Top** dù có lên được.

### 3.2 Dữ liệu sản phẩm và Merchant Center

✅ PTL:
- Google khuyến nghị **kết hợp structured data trên web page với feed trong Merchant Center** — giúp Google hiểu và xác minh dữ liệu tốt hơn.
- Merchant Center là công cụ **miễn phí** để đưa sản phẩm xuất hiện trên Search, Maps, YouTube và Images.
- Lời PTL thẳng: "Nếu bạn đang bán sản phẩm thật mà không có feed Merchant Center, bạn đang bỏ tiền trên bàn."

### 3.3 Biến thể sản phẩm và ProductGroup Schema

✅ PTL:
- Google hỗ trợ **ProductGroup** để nhóm các biến thể (màu, size, chất liệu).
- Mỗi biến thể cần: URL nhận diện được + dữ liệu giá/tồn kho/ảnh đúng + cho phép preselect từng biến thể bằng URL riêng.
- Site single-page với selector: canonical của ProductGroup thường là URL nền không preselect biến thể.
- Site multi-page: logic canonical khác — không có một canonical đại diện cho cả nhóm.
- Chỉ đổi màu/size bằng JS mà không có URL ổn định → Google rất dễ hiểu sai hoặc không crawl hết biến thể.

→ Đây là concept chưa có trong vault. Xem concept mới [[Cấu trúc trang sản phẩm chuẩn SEO + CRO]] được tạo kèm Khối 13.

### 3.4 Title, Meta Description và H1

✅ PTL:
- Title hiển thị có thể **khác `<title>`**; snippet hiển thị có thể lấy từ nội dung trang.
- Tối ưu đúng: title rõ ràng + một tiêu đề chính nổi bật + H1 nhất quán với intent + meta description nêu lợi ích mua hàng hoặc thông tin thương mại quan trọng.
- Meta description product page phù hợp để đưa: **giá, chất liệu, bảo hành, đối tượng phù hợp, thương hiệu, thời gian giao hàng**.

### 3.5 Hình ảnh sản phẩm

✅ PTL — Bộ ảnh đúng chuẩn nên có:
1. Ảnh nền trắng
2. Ảnh góc nghiêng
3. Ảnh cận vật liệu/chi tiết
4. Ảnh kích thước/quy cách
5. Ảnh thực tế khi dùng
6. Ảnh bao bì/phụ kiện
7. Ảnh trust (tem, nguồn gốc nếu có)

Yêu cầu kỹ thuật: tên file mô tả + title/alt mô tả nhất quán với chủ đề trang + nằm gần nội dung liên quan.

### 3.6 Video sản phẩm

✅ PTL — Video nên chia 3 loại:
1. Unboxing/overview
2. Demo cách dùng
3. So sánh nhanh với mẫu gần nhất

Yêu cầu kỹ thuật: cho Google fetch được byte thật của file video + URL ổn định + structured data nhất quán + thumbnail/name/description riêng cho từng video.

### 3.7 Reviews và E-E-A-T — 2 lớp riêng biệt

✅ PTL:
- **Lớp 1**: Review của người mua trên product page → tăng trust + hỗ trợ product/review schema.
- **Lớp 2**: Nội dung review/editorial (bài so sánh, đánh giá, "nên mua mẫu nào") → Google ưu tiên trải nghiệm thực, nghiên cứu gốc, bằng chứng trực quan, góc nhìn chuyên gia.
- **Trust là yếu tố quan trọng nhất trong E-E-A-T** (Google nhấn mạnh).
- Nếu là nhà bán hàng/chuyên gia: thể hiện rõ **ai tạo nội dung**, kinh nghiệm sử dụng thật, tiêu chí chấm, ưu/nhược, ảnh/video tự chụp.

→ Concept [[E-E-A-T]] đã có. Wikilink về đó.

### 3.8 FAQ trên trang sản phẩm

✅ PTL:
- FAQ vẫn hữu ích cho UX, giảm cản trở mua hàng và tăng text relevance.
- **Bỏ ảo tưởng**: FAQ rich results hiện chỉ còn dành cho website uy tín, có tính chất chính phủ hoặc y tế. Với e-commerce, **FAQ schema không cho rich result như trước**.
- Kết luận: vẫn nên có FAQ, nhưng đừng đầu tư với kỳ vọng rich result.

### 3.9 Chiến lược từ khóa — 4 tầng

✅ PTL:
| Tầng | Loại từ khóa | Trang đích phù hợp |
|---|---|---|
| 1 | Short-tail transactional cho category chính | Category page |
| 2 | Mid-tail thương hiệu/dòng sản phẩm/thuộc tính | Category hoặc product page |
| 3 | Long-tail mua hàng theo use case, vấn đề, đối tượng | Product page hoặc variant page |
| 4 | Comparison/review/support content | Bài blog hỗ trợ (link về product) |

**Quy tắc PTL**: "Từ khóa càng rộng, trang đích càng nên ở cấp danh mục; từ khóa càng cụ thể, trang đích càng nên ở cấp sản phẩm hoặc biến thể."

**Sai lầm hay gặp**: cố bắt từ khóa đầu ngành trên một product page đơn lẻ, trong khi intent thực tế của SERP nghiêng về category page hoặc bài so sánh.

---

## 4. Khung tối ưu trang sản phẩm chuẩn SEO + CRO

✅ PTL — Bảng 13 thành phần:

| Thành phần | Chuẩn nên có | Sai lầm phổ biến |
|---|---|---|
| URL | Ngắn, mô tả, ổn định, không session/tracking | URL dài, tham số rác, đổi URL liên tục |
| Title | Tên sản phẩm + thuộc tính chính + lợi ích/brand | Nhồi từ khóa, trùng lặp giữa nhiều sản phẩm |
| H1 | Khớp tên thương mại và intent | H1 khác hẳn title hoặc quá chung chung |
| Above the fold | Ảnh tốt, giá, tồn kho, CTA, chính sách giao/đổi trả | Đưa quá nhiều text, thiếu CTA, không rõ tồn kho |
| Mô tả ngắn | Nêu 3–5 lợi ích mua hàng chính | Viết chung chung như brochure |
| Mô tả sâu | Specs, chất liệu, đối tượng dùng, lưu ý, bảo hành | Thin content, copy từ nhà sản xuất |
| Media | 6–10 ảnh đủ góc + ít nhất 1 video demo | Chỉ có 1–2 ảnh nhỏ |
| Review | Điểm trung bình, số review, nội dung review có ích | Không có review hoặc review rỗng |
| FAQ | Cản trở mua hàng thật: giao hàng, bảo hành, tương thích | FAQ spam hoặc copy ở mọi trang |
| Schema | Product + Offer + Review/AggregateRating nếu đủ điều kiện; variant dùng ProductGroup khi cần | Schema không khớp text hiển thị |
| Internal links | Từ category, bài review, bài hướng dẫn, sản phẩm liên quan | Trang sản phẩm mồ côi |
| Trust | Tác giả/chuyên gia, chính sách, hotline, địa chỉ, thương hiệu | Không có dấu hiệu doanh nghiệp thật |

→ Bảng này được mở rộng thành concept riêng [[Cấu trúc trang sản phẩm chuẩn SEO + CRO]].

---

## 5. Checklist ưu tiên kỹ thuật theo P0/P1/P2

✅ PTL:

| Ưu tiên | Việc phải làm | Mục tiêu | Thời gian ước lượng | Nguồn lực tối thiểu |
|---|---|---|---|---|
| P0 | Sửa indexation: robots, noindex, canonical, lỗi 200/3xx/4xx/5xx, sitemap sạch | Không index sai trang; bot vào đúng trang tiền | 1–2 tuần | SEO + dev |
| P0 | Chuẩn hóa cấu trúc menu, category, breadcrumbs, internal links tới trang tiền | Google hiểu thứ bậc và độ ưu tiên | 1–2 tuần | SEO + dev |
| P0 | Thiết lập Search Console, Analytics, dashboard, event funnel | Có dữ liệu ra quyết định | 3–5 ngày | SEO + analytics/dev |
| P1 | Tối ưu mobile-first, CWV, ảnh, JS rendering | Cải thiện trải nghiệm và khả năng crawl/index | 2–6 tuần | Dev + SEO |
| P1 | Thêm/chuẩn hóa schema trọng yếu | Hỗ trợ hiểu nội dung và rich results | 1–3 tuần | SEO + dev |
| P1 | Dọn faceted navigation, pagination, biến thể sản phẩm | Giảm duplicate và lãng phí crawl | 1–3 tuần | SEO + dev |
| P2 | Làm mới nội dung trang danh mục, sản phẩm, trust blocks | Tăng relevance và conversion | 4–12 tuần | Content + SEO + design |
| P2 | Xây cluster nội dung, review/comparison, link earning | Tăng authority và phủ intent | Liên tục | SEO + content + outreach |

---

## 6. Mẫu báo cáo Audit

✅ PTL — Audit report phải có các mục:

| Mục trong audit | Nội dung cần có |
|---|---|
| Executive summary | 5 lỗi nặng nhất, tác động doanh thu, mức độ khẩn cấp |
| Scope | Số URL crawl, URL indexable, template chính, CMS, quốc gia, ngôn ngữ |
| Indexation | URL bị noindex nhầm, canonical sai, redirect chain, orphan pages, mâu thuẫn sitemap/index |
| Crawl & render | robots, JS rendering, link crawlability, blocked resources |
| Site architecture | menu, breadcrumb, depth, category-to-product linking, faceted nav |
| Performance | CWV theo template, ảnh nặng, JS nặng, server bottleneck |
| Structured data | lỗi/thiếu Product, Breadcrumb, Review, Organization/WebSite |
| Content quality | thin pages, duplicate titles/descriptions, cannibalization, missing trust info |
| Measurement | GSC/GA4/dashboard, conversion funnel, event mapping, baseline KPI |
| Action plan | việc gì làm ngay, ai làm, deadline, tác động kỳ vọng |

---

## 7. CRO và A/B Testing cho product SEO

✅ PTL:
- Ưu tiên test vào thành phần ảnh hưởng conversion **ít rủi ro SEO**: hero media, thứ tự block nội dung, CTA, badge trust, cách trình bày giá/khuyến mãi, block giao hàng/đổi trả, block review và FAQ.
- Test bằng URL riêng → Google khuyến nghị: dùng **rel=canonical trên bản test**, dùng **302** thay vì 301, không cloak, **kết thúc test ngay khi đủ dữ liệu**.
- Đừng kéo dài test hàng tháng trên các URL mở công khai.

---

## 8. Theo dõi ranking và xử lý khi thuật toán biến động

✅ PTL:
- Khi ranking giảm → **không phản ứng theo cảm xúc**.
- Dùng Search Console Performance report: kéo range lên **16 tháng** để loại seasonality, tách theo search type, đánh giá mức giảm nhỏ hay lớn trước khi hành động.
- Biến động nhỏ (vị trí 2 → 4): Google thậm chí khuyên **không nên thay đổi quá mạnh** nếu trang vẫn hoạt động tốt.
- Giảm mạnh và dai dẳng → kiểm tra: ranking updates, Page Indexing report, URL Inspection, tự đánh giá lại mức "helpful and reliable".
- **Core updates** là thay đổi rộng, không nhắm vào site riêng lẻ.

---

## 9. Stack công cụ khuyến nghị

✅ PTL — Bảng so sánh công cụ:

| Công cụ | Vai trò chính | Điểm mạnh | Điểm yếu | Chi phí ước tính |
|---|---|---|---|---|
| Screaming Frog SEO Spider | Crawl/audit kỹ thuật | Crawl local mạnh, kiểm tra meta, hreflang, schema, JS render, sitemap | Chạy máy cá nhân; cần người biết đọc dữ liệu | Free tới 500 URL; bản trả phí khoảng €245/năm |
| Sitebulb Cloud | Crawl/audit + cộng tác | Dễ đọc, ưu tiên issue tốt, có cloud cho team | Đắt hơn bản desktop | Cloud từ khoảng £95/tháng |
| Ahrefs | Backlink + keyword + rank tracking + site audit | Mạnh về backlink, keyword, historical data | Chi phí cao | Lite $129/tháng; Standard $249; Advanced $449; Enterprise $1.499 |
| Semrush SEO Toolkit | Rank tracking + keyword + backlink + audit | Bộ công cụ rộng, gap analysis, báo cáo tốt | Học hơi nặng; khá đắt | Pro $139,95/tháng; Guru $249,95; Business $499,95 |
| Google Search Console | Hiệu suất SEO, indexation, URL inspection, CWV | Nguồn chính thức từ Search | Không phải crawler/backlink suite đầy đủ | Miễn phí |
| Google Analytics | Hành vi người dùng, conversion, ecommerce funnel | Miễn phí, mạnh cho đo lường doanh thu | Cần set up event/data layer đúng | Miễn phí |
| Looker Studio | Dashboard điều hành SEO + CRO | Dễ hợp nhất Search Console + Analytics | Cần người dựng dashboard | Free; Pro ~$9/người/tháng |

**Stack theo ngân sách** (✅ PTL):
- **Ngân sách thấp**: Search Console + Analytics + Looker Studio + Screaming Frog
- **Ngân sách trung bình**: thêm Ahrefs hoặc Semrush
- **Ngân sách team/site lớn**: thêm Sitebulb Cloud

---

## 10. KPI cụ thể và cách đo lường

✅ PTL — Mục tiêu thực tế sau 6 tháng:

| KPI | Mục tiêu sau 6 tháng | Cách đo |
|---|---|---|
| Tỷ lệ URL indexable sạch | >90% URL nên index được index đúng; 0 URL tiền bị noindex nhầm | Crawl + Page Indexing report |
| Impressions non-brand | Tăng 30–100% tùy nền hiện tại | Search Console |
| CTR organic trang tiền | Tăng 15–30% trên nhóm query impression cao | Search Console theo page/query |
| Tỷ lệ Top 10 / Top 3 | Tăng đều trên keyword transactional cốt lõi | Rank tracker |
| Organic sessions vào category + product | Tăng 20–80% | Analytics + Search Console |
| Add-to-cart rate từ organic | Tăng 10–25% | Analytics ecommerce funnel |
| Checkout completion rate từ organic | Tăng 5–15% | Analytics |
| Organic revenue / assisted revenue | Tăng theo tốc độ tốt hơn traffic | Analytics + CRM |
| Tỷ lệ URL "Good" trong CWV | >75% phiên hoặc template group đạt chuẩn | Search Console CWV + RUM |
| Referring domains chất lượng | Tăng đều mỗi tháng, không spam | Ahrefs/Semrush |

---

## 11. Checklist vận hành hằng ngày/tuần/tháng

✅ PTL:

| Chu kỳ | Việc bắt buộc |
|---|---|
| Hằng ngày | Kiểm tra lỗi crawl/index lớn, lỗi server, sản phẩm hết hàng lâu ngày, thay đổi giá/tồn kho quan trọng, biến động doanh thu organic |
| Hằng tuần | Xem GSC: query/page tăng giảm mạnh, CTR thấp nhưng impression cao, URL mới index/chưa index, template lỗi schema, sản phẩm mồ côi |
| Hằng tuần | Tối ưu 5–20 title/meta quan trọng, cập nhật 5–10 product pages, thêm internal links từ blog/category tới trang tiền |
| Hằng tháng | Audit mini kỹ thuật, rà CWV theo template, rà cannibalization, cập nhật content plan, đánh giá link growth, họp SEO–content–dev–sales |
| Hằng tháng | Chốt 1 bảng dashboard điều hành: traffic, CTR, ranking, add-to-cart, revenue, top pages thắng/thua, action tháng sau |

---

## 12. Dashboard điều hành tuần

✅ PTL — 7 khối cần nhìn mỗi tuần:

| Khối | Chỉ số |
|---|---|
| Search demand | Impressions, non-brand impressions, số query mới |
| Search efficiency | CTR, tỷ lệ trang có title/snippet tốt, rich result coverage |
| Ranking | Top 3 / Top 10 share, từ khóa mất hạng mạnh |
| Crawl/index | Indexed vs submitted, lỗi canonical, noindex, orphan, CWV |
| Commerce | Product views từ organic, add-to-cart, checkout, purchase, revenue |
| Content ops | Số category/product đã tối ưu, số bài cluster xuất bản, số internal links mới |
| Authority | Referring domains mới, link mất, brand mentions |

---

## 13. Timeline 6 tháng (tổng quan)

✅ PTL — Timeline đề xuất (giả định site 200–5.000 URL, CMS sửa được template):

> Lưu ý: File gốc trình bày timeline dưới dạng **Mermaid Gantt chart** (không phải text). Wiki rút thành bullet point theo nhóm để dễ đọc; logic và phạm vi giống hệt gốc. Nếu cần Gantt đầy đủ, xem raw/...

- **Tháng 1**: Audit kỹ thuật tổng thể + sửa indexation + sitemap + canonical/robots + dashboard SEO/CRO
- **Tháng 2**: Mapping từ khóa & intent + dọn faceted nav/pagination + tối ưu CWV theo template
- **Tháng 2–3**: Thêm schema site/category/product + Merchant Center + feed
- **Tháng 2–4**: Rebuild category pages + bắt đầu tối ưu 20–50 product pages
- **Tháng 3–6**: Review/comparison/how-to content liên tục
- **Tháng 3–6**: Nâng block trust + review + FAQ + CRO A/B test + digital PR / link earning

**Chi tiết Gantt gốc** (✅ PTL — từng task và thời gian chính xác):

| Section | Task | Bắt đầu | Thời lượng |
|---|---|---|---|
| Nền tảng kỹ thuật | Audit kỹ thuật tổng thể | 2026-05-04 | 14 ngày |
| Nền tảng kỹ thuật | Sửa indexation và sitemap | sau audit | 14 ngày |
| Nền tảng kỹ thuật | Chuẩn hóa canonical/robots | sau audit | 21 ngày |
| Nền tảng kỹ thuật | Dọn faceted nav và pagination | 2026-05-25 | 28 ngày |
| Nền tảng kỹ thuật | Mobile-first và JS rendering | 2026-06-01 | 35 ngày |
| Hiệu suất và schema | Tối ưu CWV theo template | 2026-05-25 | 56 ngày |
| Hiệu suất và schema | Thêm schema site/category/product | 2026-06-01 | 35 ngày |
| Hiệu suất và schema | Merchant Center + feed | 2026-06-08 | 21 ngày |
| Nội dung và trang tiền | Mapping từ khóa & intent | 2026-05-18 | 14 ngày |
| Nội dung và trang tiền | Rebuild category pages | 2026-06-01 | 42 ngày |
| Nội dung và trang tiền | Tối ưu 20–50 product pages | 2026-06-08 | 84 ngày |
| Nội dung và trang tiền | Review/comparison/how-to content | 2026-06-15 | 98 ngày |
| CRO và authority | Nâng block trust + review + FAQ | 2026-06-15 | 42 ngày |
| CRO và authority | Thử nghiệm CRO/A-B test | 2026-07-06 | 56 ngày |
| CRO và authority | Digital PR / link earning | 2026-07-06 | 84 ngày |
| Đo lường và điều hành | Dashboard SEO + CRO | 2026-05-11 | 14 ngày |
| Đo lường và điều hành | Review hiệu suất hàng tuần | 2026-05-18 | 154 ngày |

---

## 14. Câu hỏi mở (5 biến số chưa có để plan chính xác hơn)

✅ PTL:

| Câu hỏi mở | Vì sao quan trọng |
|---|---|
| CMS và mức độ sửa template/URL/schema được đến đâu | Quyết định chi phí và tốc độ triển khai kỹ thuật |
| Số lượng sản phẩm, biến thể và faceted nav | Quyết định độ khó về canonical, crawl budget, pagination |
| Thị trường chỉ VN hay đa ngôn ngữ/đa vùng | Quyết định có cần hreflang ngay hay chưa |
| Có feed sản phẩm chuẩn chưa | Quyết định tốc độ triển khai Merchant Center |
| Nguồn review, media và data layer hiện có | Quyết định tốc độ cải thiện trust và CRO |

---

## 15. Kết luận thực chiến (✅ PTL nguyên văn)

> "Nếu phải chọn một thứ để làm trước, hãy làm audit indexation + cấu trúc internal links + category/product template. Đó là đòn bẩy nhỏ nhất tạo ra thay đổi lớn nhất. Sau đó mới nhân lực vào schema, Merchant Center, review/media, và CRO. Website thắng SEO bền không phải website viết nhiều nhất, mà là website ít lỗi kỹ thuật nhất, cấu trúc rõ nhất, trang tiền mạnh nhất, và đo lường kỷ luật nhất."

---

## 📎 Áp dụng cho TPCN (📎 em thêm — không có trong file gốc)

> ⚠️ Phần này hoàn toàn do agent suy luận từ khung PTL gốc, áp vào bối cảnh TPCN của anh Chương. KHÔNG phải PTL nói.

**6 đòn bẩy PTL ánh xạ vào website TPCN anh đang xây**:

1. **Indexation hygiene**: Khi website TPCN mới lên → P0 là đảm bảo trang sản phẩm/landing bán hàng được crawl & index đúng. Tránh lỗi canonical trên biến thể (vd: cùng 1 sản phẩm nhưng nhiều URL theo dạng combo/đơn lẻ/size khác nhau).

2. **Cấu trúc site**: Nên có cấu trúc rõ từ đầu: trang chủ → danh mục (theo công dụng: giảm cân, tăng đề kháng, hỗ trợ tiêu hóa...) → trang sản phẩm → bài blog hỗ trợ → internal link ngược lại. Tránh tình trạng sản phẩm mồ côi.

3. **Schema sản phẩm + Merchant Center**: Với TPCN, schema Product phải có đầy đủ: tên, mô tả, giá, tình trạng hàng, nhà sản xuất, số lượng đóng gói, hướng dẫn sử dụng. Merchant Center giúp sản phẩm xuất hiện trên Google Shopping miễn phí.

4. **CWV và mobile-first**: Khách TPCN thường mua qua điện thoại sau khi xem video/reels → mobile-first là bắt buộc. LCP ≤ 2,5s đặc biệt quan trọng cho landing page bán hàng.

5. **Media và review**: TPCN cần thêm lớp trust đặc biệt: ảnh sản phẩm thật + ảnh tem/giấy phép + video chuyên gia + review thật (tên, ảnh, trước/sau nếu được). [[E-E-A-T]] cực kỳ quan trọng trong ngành TPCN vì Google xếp TPCN vào YMYL (Your Money or Your Life).

6. **Title/snippet CTR**: Với TPCN, title nên gắn công dụng cụ thể + đối tượng + lợi ích thay vì tên thương mại chung chung. Ví dụ format: "[Tên sản phẩm] — [Công dụng chính] cho [Đối tượng] — [Điểm khác biệt]".

**Liên kết với việc đang làm của anh**:
- Kết nối với [[Khối 9 - SEO Blog 2026]] → blog cluster (Khối 9) và trang sản phẩm (Khối 13) phải link qua lại để hỗ trợ nhau về authority và intent coverage.
- Kết nối với [[Khối 2 - Cách tìm kiếm từ khoá]] → keyword research từ Khối 2 sẽ quyết định từ khóa đặt ở đâu: trang sản phẩm hay bài blog.

---

## 📌 Ghi chú về Bảng 4 — Ví dụ Trước/Sau (✅ PTL — không lưu nội dung cụ thể)

✅ PTL — File gốc có Bảng 4 "Ví dụ mẫu tối ưu một trang sản phẩm trước và sau", với lời giới thiệu: *"Ví dụ minh họa giả định cho một sản phẩm trong ngành dụng cụ xăm."*

Bảng có 12 hạng mục (cột: Hạng mục / Trước tối ưu / Sau tối ưu): URL, Title, H1, Meta description, Above the fold, Mô tả, Video, Review, FAQ, Schema, Internal linking, Trust.

Theo quy tắc 2 CLAUDE.md, nội dung cụ thể của bảng (ví dụ máy xăm) không được lưu vào vault. Logic framework 12 hạng mục đã được capture đầy đủ ở Bảng 13 thành phần (mục 4) và concept [[Cấu trúc trang sản phẩm chuẩn SEO + CRO]].

---

## 📚 Nguồn trích dẫn gốc (✅ PTL — 39 footnote URLs)

File gốc trích dẫn đầy đủ các tài liệu chính thức Google Developers:

| Footnote | URL |
|---|---|
| [1][4][5][33][39] | https://developers.google.com/search/docs/essentials/technical |
| [2] | https://developers.google.com/search/docs/fundamentals/how-search-works |
| [3] | https://developers.google.com/search/docs/appearance/ai-features |
| [6] | https://developers.google.com/search/docs/crawling-indexing/robots/intro |
| [7] | https://developers.google.com/search/docs/crawling-indexing/consolidate-duplicate-urls |
| [8] | https://developers.google.com/search/docs/specialty/international/localized-versions |
| [9] | https://developers.google.com/search/docs/crawling-indexing/sitemaps/build-sitemap |
| [10][31] | https://developers.google.com/search/docs/specialty/ecommerce/help-google-understand-your-ecommerce-site-structure |
| [11] | https://developers.google.com/search/docs/specialty/ecommerce/pagination-and-incremental-page-loading |
| [12][27] | https://developers.google.com/search/docs/crawling-indexing/mobile/mobile-sites-mobile-first-indexing |
| [13] | https://developers.google.com/search/docs/crawling-indexing/javascript/javascript-seo-basics |
| [14] | https://developers.google.com/search/docs/appearance/page-experience |
| [15] | https://developers.google.com/search/docs/appearance/structured-data/intro-structured-data |
| [16] | https://support.google.com/webmasters/answer/9133276?hl=en |
| [17][18] | https://developers.google.com/search/docs/appearance/structured-data/product |
| [19] | https://developers.google.com/search/docs/appearance/structured-data/product-variants |
| [20] | https://developers.google.com/search/docs/appearance/title-link |
| [21] | https://developers.google.com/search/docs/appearance/google-images |
| [22][35] | https://developers.google.com/search/docs/appearance/video |
| [23] | https://developers.google.com/search/docs/appearance/reviews-system |
| [24] | https://developers.google.com/search/docs/appearance/structured-data/faqpage |
| [25] | https://developers.google.com/search/docs/crawling-indexing/website-testing |
| [26] | https://developers.google.com/search/docs/appearance/core-updates |
| [28] | https://www.screamingfrog.co.uk/seo-spider/pricing/ |
| [29][36] | https://search.google.com/search-console/about |
| [30] | https://sitebulb.com/subscriptions/pricing/index |
| [32] | https://ahrefs.com/pricing |
| [34] | https://www.semrush.com/kb/1547-seo-toolkit-pricing-limits |
| [37] | https://marketingplatform.google.com/about/analytics/ |
| [38] | https://cloud.google.com/looker-studio?hl=pt-BR |

---

## 🔗 Wikilink liên quan

- [[Khối 9 - SEO Blog 2026]] — SEO blog/content cluster (Khối 9 ↔ Khối 13 bổ trợ nhau)
- [[Khối 2 - Cách tìm kiếm từ khoá]] — keyword research đầu vào cho cả hai
- [[E-E-A-T]] — trust và authority (đặc biệt quan trọng với TPCN)
- [[Schema]] — structured data nền tảng
- [[Topic Cluster]] — cấu trúc content cluster gắn với internal linking
- [[Search Intent]] — match intent cho từng cấp trang
- [[TOFU-MOFU-BOFU]] — chiến lược từ khóa theo phễu
- [[Cấu trúc trang sản phẩm chuẩn SEO + CRO]] — concept mới tạo từ Khối 13
