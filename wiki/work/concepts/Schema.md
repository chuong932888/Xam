---
type: concept
tags: [seo, schema, structured-data, technical-seo, blog, ips, khoi-9]
created: 2026-05-09
updated: 2026-05-09
sources: ["[[Khối 9 - SEO Blog 2026]]"]
---

# Schema — Đánh dấu dữ liệu có cấu trúc cho máy đọc

> **Định nghĩa thẳng** *(theo PTL gốc dòng 81-82)*: Schema là một đoạn mã ngắn nhúng vào trang web để "nói" cho Google và AI biết: đây là bài viết, tác giả là ai, ngày đăng khi nào, có FAQ ở đoạn nào… Người đọc **không nhìn thấy** đoạn mã, nhưng máy đọc rất nhanh.

> ⚠️ **Phân biệt nguồn — quan trọng**:
> - ✅ **PTL gốc nói**: định nghĩa Schema, "có Schema = máy hiểu nhanh hơn", **chỉ nhắc 2 loại Schema cụ thể là `Article` + `FAQPage`** (gốc dòng 112, 192, 232), test bằng **Rich Results Test** (gốc dòng 393), plugin Yoast/Rank Math tự cài.
> - 📎 **Em (agent) thêm**: thuật ngữ "JSON-LD", các @type chuyên ngành (`MedicalScholarlyArticle`, `Physician`, `DietarySupplement`, `Person`, `Organization`, `Product`), chi tiết các trường (`headline`, `datePublished`, `sameAs`, `aggregateRating`…), khái niệm "Knowledge Panel", Schema.org Validator, "7 lỗi Schema phổ biến". Đây đều là kiến thức SEO industry chuẩn từ schema.org, **đúng kỹ thuật** nhưng **không có trong tài liệu PTL** — anh xác minh độc lập trước khi giao team triển khai.
> - 🚫 **Em đã bỏ con số "CTR tăng 30-50%"** — không có trong gốc, không xác minh được, dễ thành con số trôi nổi.

## 🎯 Vì sao Schema = lợi thế

Google hiển thị **rich snippet** (đoạn highlight đặc biệt) cho bài có Schema. Bài có Schema FAQ → câu hỏi-đáp hiển thị NGAY trên trang kết quả Google.

→ Đặc biệt quan trọng cho TPCN vì câu hỏi sức khoẻ rất nhiều, người dùng thường lướt nhanh chọn bài có FAQ rõ ràng.

## 📋 5 loại Schema khuyến nghị cho website TPCN

> 📎 *Trong 5 loại dưới đây, **chỉ Article + FAQPage là PTL gốc nhắc đến**. 3 loại còn lại (Person, Organization, Product/DietarySupplement) là em đề xuất thêm — chuẩn schema.org, dùng phổ biến cho thương hiệu y tế/TPCN.*

### 1. Article (cho mọi bài blog) — ✅ PTL gốc nhắc trực tiếp

**Đánh dấu**: bài viết, tác giả, ngày đăng, ngày sửa, ảnh đại diện, mô tả ngắn.

**Lợi ích**: Google hiển thị tên tác giả + ngày đăng dưới tiêu đề → tăng độ tin cậy.

**Trường bắt buộc**:
- `@type: Article` (hoặc `MedicalScholarlyArticle` cho bài y khoa chuyên sâu)
- `headline` — tiêu đề
- `author` — tên tác giả + link tới trang Author
- `datePublished` — ngày đăng
- `dateModified` — ngày cập nhật (Google ưu tiên bài "tươi")
- `image` — ảnh đại diện
- `publisher` — tên brand + logo

### 2. FAQPage (cho phần FAQ cuối bài) — ✅ PTL gốc nhắc trực tiếp, "PHẦN AI HAY TRÍCH NHẤT"

**Đánh dấu**: từng cặp câu hỏi-đáp.

**Lợi ích**: 
- Google hiển thị **5-10 câu FAQ** ngay trên SERP (rich snippet).
- AI (ChatGPT, Perplexity) **dễ trích nhất** từ phần này.

**Trường bắt buộc**:
- `@type: FAQPage`
- Danh sách `mainEntity` — mỗi item:
  - `@type: Question`
  - `name` — câu hỏi
  - `acceptedAnswer` → `text` — câu trả lời

### 3. Person (cho trang tác giả) — 📎 em đề xuất, chuẩn schema.org

**Đánh dấu**: thông tin tác giả/bác sĩ.

**Lợi ích**: gắn tác giả thành **[[Entity]]** rõ ràng → tăng [[E-E-A-T]] mạnh.

**Trường bắt buộc**:
- `@type: Person` (hoặc `Physician` cho bác sĩ)
- `name`, `jobTitle`
- `image` — ảnh chân dung thật
- `sameAs` — danh sách link: LinkedIn, trang bệnh viện, các bài báo nhắc tới...
- `description` — tiểu sử ngắn
- `affiliation` — bệnh viện/trường ĐH

### 4. Organization (cho brand) — 📎 em đề xuất, chuẩn schema.org

**Đánh dấu**: thông tin công ty.

**Lợi ích**: brand thành [[Entity]] rõ ràng, hiển thị Knowledge Panel khi Google đủ tin.

**Trường bắt buộc**:
- `@type: Organization`
- `name`, `legalName`, `url`
- `logo`
- `sameAs` — fanpage, LinkedIn company, Twitter/X, YouTube channel...
- `address`, `telephone`, `email`
- `contactPoint`

### 5. Product (cho trang sản phẩm TPCN) — 📎 em đề xuất, chuẩn schema.org

**Đánh dấu**: tên sản phẩm, giá, đánh giá, mô tả.

**Lợi ích**: Google hiển thị **giá + sao đánh giá** ngay trên SERP → CTR cao.

**Trường bắt buộc**:
- `@type: Product`
- `name`, `description`, `image`
- `brand`, `sku`, `gtin` (nếu có)
- `offers` → `price`, `priceCurrency`, `availability`
- `aggregateRating` (nếu có ≥ 5 đánh giá thật)
- **TPCN cụ thể**: nên dùng `@type: DietarySupplement` (subtype của Product) — Google nhận diện đúng ngành.

## 🛠️ 4 cách cài Schema (chọn cách phù hợp)

| Cách | Phù hợp | Khó | Chi phí |
|---|---|---|---|
| **Plugin Yoast SEO / Rank Math** (WordPress) | Người mới, không code | Dễ | Miễn phí (bản free đủ dùng) |
| **Plugin Schema Pro / WP Schema Pro** | WP, cần Schema sâu hơn | Vừa | $79/năm |
| **Tag Manager + JSON-LD tự viết** | Web custom, có dev | Khó | Miễn phí (cần dev) |
| **Hardcode trong template** | Cần kiểm soát 100% | Khó | Cần dev |

→ **Khuyến nghị cho anh Chương**: WordPress + **Rank Math (free)** — đủ làm Article + FAQPage + Person + Organization. Khi cần Product/Review thì lên Schema Pro.

## ✅ Cách kiểm tra Schema đã đúng chưa

### Tool 1: Rich Results Test (chính thức của Google)
🔗 https://search.google.com/test/rich-results

- Dán URL → bấm Test.
- Phải báo "✅ Page is eligible for rich results" + liệt kê các Schema phát hiện.
- Nếu báo lỗi → đọc lỗi, sửa.

### Tool 2: Schema.org Validator
🔗 https://validator.schema.org/

- Validate cú pháp JSON-LD chuẩn theo schema.org.
- Bắt được lỗi structure mà Google Rich Results không bắt.

### Tool 3: Google Search Console
- Vào tab "Enhancements" → xem báo cáo FAQ, Article...
- Theo dõi **Valid items** vs **Errors**.
- Hàng tuần check 1 lần.

## 🚨 7 lỗi Schema phổ biến *(em biên soạn — không có trong PTL gốc, là kiến thức SEO chung)*

1. **Có Schema FAQPage nhưng nội dung FAQ ẩn (collapse mặc định)** — Google năm 2024+ phạt: FAQ phải hiển thị trên trang, không được dưới accordion ẩn.
2. **Schema Article không có `dateModified`** — bài cũ không được làm "tươi" → tụt rank.
3. **Tên Author trong Schema khác tên hiển thị trên bài** — Google không nối được entity → mất E-E-A-T.
4. **Image quá nhỏ trong Schema** — Google yêu cầu ≥ 1200px chiều rộng cho Article.
5. **`sameAs` rỗng** — không link tới LinkedIn/trang bệnh viện → tác giả không được công nhận entity.
6. **Schema Product không có `brand` hoặc `offers.priceCurrency`** — không hiển thị rich snippet.
7. **Multiple Schema cùng loại** — vd: 2 Article schema trên 1 trang → Google bỏ qua cả 2.

## 📅 Quy trình áp Schema cho mỗi bài blog (5 phút/bài)

1. ☐ Cài plugin Rank Math (làm 1 lần cho cả website).
2. ☐ Bật **Article schema** mặc định cho mọi post.
3. ☐ Tạo trang Author với đủ thông tin → Rank Math tự sinh **Person schema**.
4. ☐ Khi viết bài, đến phần FAQ → dùng block "FAQ" trong Gutenberg → Rank Math tự sinh **FAQPage schema**.
5. ☐ Sau khi đăng — copy URL → test bằng [[Rich Results Test]] → fix nếu có lỗi.
6. ☐ Submit URL lên Google Search Console để index nhanh.

## 🎯 Hành động cho anh Chương

1. **Tuần 1 sau khi có website** — cài Rank Math + tạo Author profile cho bác sĩ chính + cấu hình Organization schema.
2. **Mỗi bài đăng** — bắt buộc qua Rich Results Test trước khi public.
3. **Hàng tháng** — vào Google Search Console tab Enhancements check số valid items vs errors.

## 🔗 Liên quan

- [[Khối 9 - SEO Blog 2026]] — page mẹ
- [[E-E-A-T]] — Person schema + sameAs nâng E-E-A-T
- [[AEO-GEO]] — FAQPage schema = phần AI hay trích nhất
- [[Topic Cluster]] — mỗi bài trong cluster phải có Schema đầy đủ
