---
type: concept
tags: [seo, website, san-pham, schema, cro, product-page, on-page, ptl]
created: 2026-05-09
updated: 2026-05-09
sources: ["[[Khối 13 - SEO sản phẩm Website]]"]
---

# Cấu trúc trang sản phẩm chuẩn SEO + CRO

> Nguồn: [[Khối 13 - SEO sản phẩm Website]] — thầy [[Phạm Thành Long]], khoá IPS.

> ⚠️ **Phân biệt nguồn**:
> - ✅ **PTL gốc**: Bảng 13 thành phần (mục 4 Khối 13), ví dụ trước/sau tối ưu, logic intent-matching, ProductGroup schema, Merchant Center, chiến lược từ khóa 4 tầng.
> - 📎 **Em thêm**: phần ánh xạ vào TPCN, ví dụ cụ thể về sản phẩm sức khoẻ, ghi chú về YMYL.

---

## 🎯 Vì sao trang sản phẩm khác blog về SEO?

✅ PTL — Khối 13 phân biệt rõ:
- **Blog (Khối 9)**: tối ưu để Google và AI tin tưởng + trích dẫn → mục tiêu là authority và awareness.
- **Trang sản phẩm (Khối 13)**: tối ưu để **match intent mua hàng + làm rõ thông tin quyết định mua + tăng trust + giảm ma sát** → mục tiêu là conversion.

Trang sản phẩm cần đồng thời thuyết phục 2 đối tượng:
1. **Google/bot**: hiểu đây là trang gì, sản phẩm gì, giá bao nhiêu, còn hàng không, đáng tin không.
2. **Người mua**: thấy đủ lý do để ấn "mua ngay" và không rời đi.

---

## 📋 13 thành phần bắt buộc của trang sản phẩm chuẩn

✅ PTL:

### 1. URL
- **Chuẩn**: ngắn, mô tả sản phẩm, ổn định, không chứa session ID hoặc tracking parameter.
- **Sai lầm**: URL dài với tham số rác, đổi URL liên tục (mất link equity).
- Ví dụ tốt: `/thuc-pham-chuc-nang-tang-de-khang-vitamin-c-1000mg`
- Ví dụ xấu: `/san-pham?id=48291&color=red&utm=abc&session=xyz`

### 2. Title (thẻ `<title>`)
- **Chuẩn**: Tên sản phẩm + thuộc tính chính + lợi ích/brand.
- **Sai lầm**: nhồi từ khóa, trùng lặp giữa nhiều sản phẩm trong cùng danh mục.
- Format gợi ý: `[Tên SP] — [Công dụng chính/Spec nổi bật] | [Brand]`

### 3. H1
- **Chuẩn**: khớp tên thương mại và intent tìm kiếm.
- **Sai lầm**: H1 khác hẳn title (gây mâu thuẫn tín hiệu) hoặc quá chung chung.
- H1 và Title nên gần giống nhau, không cần trùng 100%.

### 4. Above the fold (màn hình đầu tiên khi load trang)
- **Chuẩn**: ảnh tốt + giá + tồn kho rõ ràng + CTA + chính sách giao/đổi trả.
- **Sai lầm**: đưa quá nhiều text, thiếu CTA, không rõ còn hàng không.
- Nguyên tắc: người mua phải thấy lý do mua và nút mua mà không cần scroll.

### 5. Mô tả ngắn (short description)
- **Chuẩn**: nêu 3–5 lợi ích mua hàng chính, súc tích, hướng đến quyết định.
- **Sai lầm**: viết chung chung như brochure thương hiệu.

### 6. Mô tả sâu (long description)
- **Chuẩn**: specs kỹ thuật, chất liệu/thành phần, đối tượng phù hợp, lưu ý khi dùng, bảo hành, câu hỏi thường gặp về sản phẩm.
- **Sai lầm**: thin content (quá ít), copy từ nhà sản xuất (duplicate content).
- Độ dài: đủ để thuyết phục — thường 600–1.200 từ tùy độ phức tạp của sản phẩm.

### 7. Media (ảnh + video)
- **Chuẩn ảnh** (6–10 ảnh): nền trắng / góc nghiêng / cận chi tiết / kích thước quy cách / thực tế khi dùng / bao bì phụ kiện / ảnh trust (tem, chứng nhận).
- **Chuẩn video** (ít nhất 1): chia 3 loại — unboxing/overview, demo cách dùng, so sánh nhanh với mẫu gần nhất.
- **Sai lầm**: chỉ có 1–2 ảnh nhỏ, không có video.
- Yêu cầu kỹ thuật: tên file mô tả + alt text mô tả + URL video ổn định để Google fetch được.

### 8. Review
- **Chuẩn**: điểm trung bình + số lượng review + nội dung review có ích (có ảnh/video nếu được).
- **Sai lầm**: không có review, hoặc review rỗng không có nội dung.
- Kết nối với schema: AggregateRating trong Product schema.

### 9. FAQ
- **Chuẩn**: trả lời đúng cản trở mua hàng thật (giao hàng, bảo hành, tương thích, cách dùng).
- **Sai lầm**: FAQ spam hoặc copy y hệt ở mọi trang sản phẩm.
- Lưu ý PTL: FAQ schema hiện **không còn cho rich result** với e-commerce — nhưng vẫn cần cho UX và text relevance.

### 10. Schema sản phẩm
- **Chuẩn**: Product + Offer + Review/AggregateRating nếu đủ điều kiện.
- **Biến thể**: dùng ProductGroup khi có nhiều biến thể (màu, size, hương vị...).
- **Sai lầm**: schema không khớp text hiển thị trên trang.
- Validate: Rich Results Test → URL Inspection → theo dõi báo cáo trong Search Console.

### 11. Internal links
- **Chuẩn**: trang sản phẩm phải nhận link từ — category page, bài review, bài hướng dẫn, sản phẩm liên quan trong cùng nhóm.
- **Sai lầm**: trang sản phẩm mồ côi (chỉ tìm thấy qua search box nội bộ).
- Logic: blog cluster (Khối 9) → dẫn về trang sản phẩm (Khối 13) → tạo vòng traffic + authority.

### 12. Trust signals
- **Chuẩn** ✅ PTL: tên tác giả/chuyên gia review, chính sách rõ ràng, hotline, địa chỉ thực, tên thương hiệu, mạng xã hội.
- **Sai lầm** ✅ PTL: không có bất kỳ dấu hiệu nào cho thấy đây là doanh nghiệp thật.
- 📎 em thêm: Đặc biệt quan trọng cho TPCN vì TPCN thuộc nhóm YMYL (Your Money or Your Life) theo cách phân loại của Google — tiêu chí E-E-A-T bị đánh giá khắt khe hơn. Khái niệm YMYL không được nêu trong file gốc PTL.

### 13. Meta description
- **Chuẩn**: nêu lợi ích mua hàng hoặc thông tin thương mại quan trọng — giá, chất liệu, bảo hành, đối tượng, thời gian giao hàng.
- **Sai lầm**: "Bán [tên sản phẩm] uy tín, chất lượng, giá tốt" — nói không có thông tin.
- Lưu ý: snippet hiển thị có thể lấy từ nội dung trang, không nhất thiết từ meta description.

---

## 🔢 Chiến lược từ khóa 4 tầng (✅ PTL — cột ví dụ TPCN là 📎 em thêm)

> ⚠️ Gốc PTL trình bày 4 tầng dưới dạng văn xuôi (không phải bảng). Cột "Loại từ khóa" và "Trang đích đúng" là ✅ PTL. Cột "Ví dụ TPCN" là 📎 em thêm để ánh xạ vào bối cảnh của anh Chương — KHÔNG có trong tài liệu gốc.

| Tầng | Loại từ khóa (✅ PTL) | Ví dụ TPCN (📎 em thêm) | Trang đích đúng (✅ PTL) |
|---|---|---|---|
| 1 | Short-tail transactional cho category | "thực phẩm chức năng tăng đề kháng" | Category page |
| 2 | Mid-tail thương hiệu/dòng/thuộc tính | "vitamin C 1000mg DHC Nhật" | Category hoặc product page |
| 3 | Long-tail theo use case/vấn đề/đối tượng | "vitamin C cho người hay bị cảm cúm uống loại nào" | Product page hoặc variant |
| 4 | Comparison/review/support content | "nên uống vitamin C 500mg hay 1000mg" | Bài blog → link về product |

> "Từ khóa càng rộng, trang đích càng nên ở cấp danh mục; từ khóa càng cụ thể, trang đích càng nên ở cấp sản phẩm hoặc biến thể." — ✅ PTL

---

## 🔄 ProductGroup Schema cho biến thể sản phẩm (✅ PTL)

Khi 1 sản phẩm có nhiều biến thể (màu, size, hương vị, hàm lượng):
- Mỗi biến thể cần: URL nhận diện riêng + dữ liệu giá/tồn kho/ảnh đúng + preselect được bằng URL.
- **Site single-page** (selector JS): canonical của ProductGroup = URL nền không preselect biến thể.
- **Site multi-page**: không có một canonical duy nhất đại diện cả nhóm.
- Nguy cơ: đổi biến thể bằng JS mà không có URL ổn định → Google không crawl được hết biến thể.

---

## 🏪 Merchant Center — Bắt buộc nếu bán sản phẩm thật (✅ PTL)

- Merchant Center là công cụ **miễn phí** của Google.
- Kết hợp với structured data trên web → Google hiểu và xác minh dữ liệu sản phẩm từ 2 nguồn.
- Sản phẩm sẽ xuất hiện trên: Google Search, Maps, YouTube, Google Images.
- PTL nói thẳng: "Nếu bạn đang bán sản phẩm thật mà không có feed Merchant Center, bạn đang bỏ tiền trên bàn."
- Với TPCN: đặc biệt quan trọng vì người mua thường tìm kiếm sản phẩm qua Google Shopping trước khi vào landing page.

---

## 📎 Áp dụng cho TPCN (📎 em thêm)

> Phần này do agent suy luận — không có trong PTL gốc. Xác nhận với bác sĩ/chuyên gia trước khi triển khai.

**Đặc thù TPCN cần chú ý thêm khi tối ưu trang sản phẩm**:

1. **YMYL — Your Money or Your Life**: Google xếp TPCN vào nhóm có ảnh hưởng đến sức khoẻ → tiêu chí E-E-A-T và trust được đánh giá khắt khe hơn nhiều so với sản phẩm thông thường.

2. **Trust signals bắt buộc cho TPCN**:
   - Số đăng ký lưu hành (nếu có)
   - Ảnh tem/chứng nhận cơ quan quản lý
   - Tên bác sĩ/chuyên gia đứng sau sản phẩm
   - Công ty sản xuất, địa chỉ nhà máy

3. **Meta description TPCN** nên có: công dụng chính + đối tượng dùng + hàm lượng/liều dùng + lưu ý (ai không nên dùng).

4. **FAQ TPCN** quan trọng hơn mức bình thường: "Sản phẩm có kiểm định không?", "Dùng bao lâu thấy hiệu quả?", "Có dùng được khi đang uống thuốc không?", "Phụ nữ mang thai có dùng được không?"

5. **Ảnh trust** cho TPCN: ảnh hộp/lọ thật từ nhiều góc + ảnh tem QR/barcode + ảnh chứng nhận/giấy phép.

---

## 🔗 Wikilink liên quan

- [[Khối 13 - SEO sản phẩm Website]] — source page đầy đủ
- [[Schema]] — structured data (Article, FAQPage từ Khối 9)
- [[E-E-A-T]] — trust và authority (đặc biệt quan trọng với TPCN/YMYL)
- [[Topic Cluster]] — cấu trúc blog cluster link về trang sản phẩm
- [[Khối 9 - SEO Blog 2026]] — SEO blog/content cluster bổ trợ
- [[TOFU-MOFU-BOFU]] — chiến lược từ khóa 4 tầng theo phễu
