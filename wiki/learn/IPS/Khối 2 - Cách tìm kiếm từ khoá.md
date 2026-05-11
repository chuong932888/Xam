---
type: source
tags: [ips, khoi-2, keyword-research, seo, ptl]
created: 2026-05-09
updated: 2026-05-09
sources: ["[[raw/Đặc sản của Phạm Thành Long/IPS - 19 khối công việc/2_ Cách tìm kiếm từ khóa.md]]"]
khoi: 2
---

# Khối 2 — Cách tìm kiếm từ khoá

> Nguồn: thầy [[Phạm Thành Long]], khoá [[index|IPS]]. File gốc 50KB.

## 🎯 TL;DR

Cẩm nang đầy đủ về keyword research: 4 tầng [[Search Intent|intent]], phân tầng [[TOFU-MOFU-BOFU|phễu]], quy trình 7 bước, bộ công cụ free/trả phí/AI, [[Rubric 10 điểm lọc keyword|rubric 10 điểm]] lọc keyword, map vào 7 kênh, 10 lỗi thường gặp, 7 prompt AI, template Google Sheet, lịch review định kỳ. Nguyên tắc xuyên suốt: **30 keyword được lọc kỹ + làm sâu > 300 keyword làng nhàng**.

## 🧭 Mục đích trong IPS

Biết khách đang ở đâu trong hành trình mua + đang dùng ngôn ngữ gì → phân bổ đúng nội dung vào đúng kênh đúng giai đoạn. Không có keyword research chuẩn → khối nội dung, ADS, landing page đều "mù".

## 📋 Quy trình 7 bước

### Bước 1: Hiểu Hồ sơ KH (bắt buộc trước)
Trích từ [[Khối 1 - Hồ sơ khách hàng]]:
- 3-5 pain point lớn nhất
- 10-20 câu khách nói nguyên văn (voice of customer)
- Trigger mua (khoảnh khắc quyết định)
- Rào cản (lý do chần chừ)

Công thức: mỗi pain → 3-5 cách diễn đạt thành câu tìm kiếm; mỗi quote → 1-2 keyword.

### Bước 2: Brainstorm seed keywords (10-30 từ gốc)
4 nguồn:
- Tên dịch vụ chính (3-5 seed)
- Vấn đề khách than (5-10 seed)
- Tên đối thủ (3-5 seed)
- Thuật ngữ ngành (5-10 seed)

### Bước 3: Mở rộng seed (mỗi seed → 20-100 biến thể)
6 sub-bước:
1. Google → ghi 8 autocomplete
2. Cuộn cuối SERP → "Tìm kiếm liên quan"
3. People Also Ask → 4-8 câu
4. AnswerThePublic → ma trận câu hỏi
5. Ahrefs/Ubersuggest → matching terms + questions + also rank for
6. AI (ChatGPT/Claude/Gemini) → prompt mở rộng

### Bước 4: Phân tích SERP và đối thủ ⭐ QUAN TRỌNG NHẤT (80% người bỏ qua)
Với 5-10 keyword tiềm năng, gõ Google và kiểm:
- Domain nào rank? Mạnh/yếu?
- Loại content gì? (Blog, video, sản phẩm)
- Độ dài bao nhiêu?
- SERP feature nào?
- Có "content gap" không?

**Nguyên tắc**: Volume + KD đẹp nhưng top 10 toàn site authority cao + content rất sâu → vô vọng. Volume nhỏ + top 10 yếu → cơ hội vàng.

### Bước 5: Phân loại + Clustering
4 chiều:
- 3 nhóm cơ bản (Chính / Liên quan / Người mua tìm)
- [[Search Intent]] (4 loại)
- [[TOFU-MOFU-BOFU|Funnel stage]]
- Đặc thù (long-tail, local, branded, seasonal)

**Clustering**: gom keyword cùng intent + cùng SERP intent → 1 bài viết. Cách kiểm: 5/10 kết quả top 10 trùng nhau → cùng cluster.

### Bước 6: Đánh giá qua [[Rubric 10 điểm lọc keyword|Rubric 10 điểm]]
- ≥ 8 điểm → ưu tiên cao, làm trong 30 ngày
- 6-7 → làm khi rảnh
- < 6 → bỏ

### Bước 7: Map vào kênh + lập content calendar
Mỗi keyword: kênh / loại nội dung / người phụ trách / ngày đăng / KPI. Đẩy vào Google Sheet master. Review hàng tuần.

## 📊 Phân loại từ khoá — 4 tầng [[Search Intent]]

| Intent | Mô tả | Wording | Loại SERP |
|---|---|---|---|
| **Informational** | Muốn biết, học, hiểu | "là gì", "cách", "tại sao", "có...không" | Featured snippet, PAA, blog dài |
| **Navigational** | Đã biết tên brand | tên thương hiệu, tên app | Sitelinks |
| **Commercial Investigation** | Đang so sánh | "tốt nhất", "review", "so sánh", "vs" | Listicle, review |
| **Transactional** | Sẵn sàng mua | "mua", "giá", "bao nhiêu", "gần đây" | Shopping, ads, Map Pack |

## 🎯 [[TOFU-MOFU-BOFU|Phân tầng phễu]]

| Tầng | % | Đặc điểm | Loại nội dung | KPI |
|---|---|---|---|---|
| TOFU | 60% | Informational, volume cao, KD cao | Blog giáo dục, video giải thích | Traffic, brand awareness, opt-in |
| MOFU | 30% | Commercial investigation, vừa | So sánh, case study, lead magnet | Lead, đặt lịch tư vấn |
| BOFU | 10% | Transactional, volume thấp, conversion cao | Landing page, bảng giá, testimonial | Đơn hàng, ROAS |

## 📏 Metrics đánh giá keyword

| Metric | Ngưỡng |
|---|---|
| **Volume** | Cao >10K/tháng; Vừa 1K-10K; Thấp 100-1K. **TPCN ngách: 200-500 đã đủ ý nghĩa.** |
| **KD (Keyword Difficulty)** | 0-15 dễ; 16-30 vừa; 31-50 khó; 51+ rất khó. **Site mới năm đầu: chỉ KD ≤ 30.** |
| **CPC** | Cao = kiếm tiền được. Thấp = cơ hội hoặc rủi ro. |
| **Trend** | Ưu tiên đang tăng (Google Trends). |
| **CTR theo position** | P1 = 27.6%; P2 = 15.8%; P3 = 11%; Page 2 < 1% |

## 🛠️ Công cụ thầy khuyên

### Free
- **Google Keyword Planner** — volume, CPC. Cần Google Ads account, không cần chạy ads.
- **Google Trends** — xu hướng, mùa.
- **Google Search Console** — keyword thật đang kéo traffic.
- **Google autocomplete + PAA + Related searches** — không cần tool.
- **AnswerThePublic** — ma trận câu hỏi (free 3 lượt/ngày).
- **Keyword Surfer** (extension Chrome) — volume + CPC ngay trên SERP.
- **Ubersuggest** — volume, KD, content ideas (free 3 lượt/ngày).
- **KeywordTool.io** — scrape suggest từ YouTube, Amazon, Bing, TikTok.
- **Reddit & Quora** — câu hỏi nhiều upvote = keyword TOFU tiềm năng.
- **TikTok/YouTube/Instagram search bar** — autocomplete.

### Trả phí
- **Ahrefs** ($99/tháng) — mạnh nhất, recommend nếu có ngân sách. Site Explorer, Keywords Explorer, Content Gap.
- **SEMrush** ($119/tháng) — toàn diện SEO + ads + social.
- **Moz Pro** ($99/tháng) — dữ liệu sạch.
- **KWFinder/Mangools** ($30/tháng) — **rẻ nhất, đủ cho SME — recommend cho anh Chương khởi đầu**.
- **Surfer SEO** ($89/tháng) — kết hợp keyword + content optimization.

### AI
- **ChatGPT / Claude / Gemini** — mở rộng seed, phân loại intent, sinh outline. Lưu ý: AI KHÔNG có volume thật → luôn cross-check Keyword Planner/Ahrefs.

## 🚫 [[Rubric 10 điểm lọc keyword]] — bản rút gọn

| # | Tiêu chí | Câu hỏi |
|---|---|---|
| 1 | Liên quan HSKH | Khớp persona đang nhắm? |
| 2 | Chạm pain | Có chạm pain thật? |
| 3 | Có ý định hành động | Khách muốn xem/đọc/mua, hay tò mò? |
| 4 | Tạo được nội dung | Mình đủ chuyên môn cover? |
| 5 | Phù hợp sản phẩm | Khớp offer? |
| 6 | KD vừa sức | KD ≤ 30 cho site < 2 năm? |
| 7 | Volume đủ to | Đạt ngưỡng có ý nghĩa với ngách? |
| 8 | Intent khớp giai đoạn | Khớp loại content? |
| 9 | Đo được conversion | Track keyword → lead/sale rõ? |
| 10 | Có cửa top 3 | SERP top 10 — realistic? |

## 📊 Số liệu quan trọng

- **Long-tail chiếm 70%** tổng lượng tìm kiếm Google.
- **Featured snippet** kéo traffic gấp 3-5 lần P1 thường.
- Tỷ lệ branded/non-branded lành mạnh: **30/70**.
- Mỗi chiến dịch ads cần ≥ 30 negative keyword, cập nhật hàng tuần.

## 🔬 Phân loại nâng cao (6 chiều)

### Long-tail vs Short-tail
- **Short-tail**: 1-2 từ, volume rất cao, KD rất cao, intent mơ hồ. VD: "collagen", "TPCN".
- **Long-tail**: 4-7 từ, volume thấp, KD thấp, intent rõ. VD: "collagen cho phụ nữ tuổi 35 dạng nước".
- **Quy tắc thực hành:** Brand mới (domain < 2 năm, traffic < 5K/tháng) → tập trung **80% long-tail**. Long-tail mỗi từ ít traffic nhưng cộng dồn 100 từ thì đáng kể, mà dễ rank hơn nhiều.

### Branded vs Non-branded
- **Branded**: chứa tên thương hiệu. Conversion rất cao.
- **Non-branded**: mô tả thuần chức năng/giải pháp. Volume cao hơn, conversion thấp hơn.
- **Tỷ lệ healthy: 30% branded / 70% non-branded.** 90% branded = chỉ thu khách đã biết. 100% non-branded = brand chưa có nhận diện.

### Local Keywords (RẤT QUAN TRỌNG cho TPCN có cửa hàng vật lý)
Cấu trúc:
- `[dịch vụ] + [địa danh]`: "TPCN cao cấp quận 1"
- `[dịch vụ] + gần [địa danh]`: "nhà thuốc TPCN gần Hồ Gươm"
- `[dịch vụ] + gần đây / gần tôi`: "nhà thuốc TPCN gần đây"
- `[dịch vụ] + [quận] + [thành phố]`: "TPCN dạng nước quận Hai Bà Trưng Hà Nội"
- `[dịch vụ] + ở [địa danh]`: "ở Đà Nẵng mua TPCN ở đâu"

→ Đăng ký **Google Business Profile**, lấy review thật, đăng ảnh có geotag, viết bài lồng tự nhiên tên quận/phường.

### Voice Search Keywords
Khách dùng Siri / Google Assistant — câu đầy đủ, dài 8-15 từ:
- "Nhà thuốc TPCN nào uy tín gần tôi mở cửa chủ nhật"
- Bắt đầu bằng "ai", "ở đâu", "khi nào", "bao nhiêu"
- Voice search tăng nhanh ở VN (Gen Z + người lái xe)

→ Nội dung cần dạng câu hỏi rõ + câu trả lời ngắn 1-2 dòng đầu (Google chọn để đọc lên loa).

### Seasonal Keywords (theo mùa)
Volume tăng vọt theo mùa. Ngành TPCN:
- **Tết**: TPCN biếu, vitamin tổng hợp gói quà
- **Hè (T4-7)**: TPCN làm đẹp da chống nắng, giảm cân chuẩn bị bikini
- **Mùa thi (T5-7)**: TPCN tăng trí nhớ cho học sinh, sĩ tử
- **Mùa cúm (T11-2)**: TPCN tăng đề kháng, vitamin C
- **Sau Tết**: TPCN giải rượu, giải độc gan
- **Cuối năm**: TPCN biếu, gói quà sức khoẻ

→ Phát hiện qua **Google Trends** so sánh 12 tháng. Lập kế hoạch nội dung sớm trước peak **4-6 tuần**.

### Negative Keywords (cho ads)
Trong Google Ads, negative keyword = từ KHÔNG MUỐN bid. Bỏ sót → đốt tiền click rác.

Ví dụ TPCN, nếu chạy ads cho TPCN cao cấp, nên loại:
- "miễn phí" (khách không sẵn sàng trả)
- "tự làm tại nhà" (sản phẩm khác)
- "mẹo dân gian" (đi ngược thông điệp khoa học)
- "rẻ nhất" (định vị khác)
- "cho trẻ em dưới 1 tuổi" (đối tượng không khớp)

→ Mỗi chiến dịch cần ≥ 30 negative keyword, cập nhật hàng tuần từ Search Term Report. Xem [[Template Google Sheet Keyword Master#Tab 2 - Negative Keywords]].

## 🚨 10 lỗi thường gặp

1. **Chỉ chọn keyword volume cao** — ngó volume, bỏ qua intent + KD. Hậu quả: rank khó, traffic không chất.
2. **Bỏ qua intent** — làm blog cho keyword transactional, làm landing cho keyword informational. Bounce rate cao, conversion thấp.
3. **Không phân biệt local vs national** — tiệm Hà Nội mà chạy ads "TPCN Việt Nam". Đốt tiền vô ích.
4. **Copy đối thủ mù quáng** — đối thủ DA 60, mình DA 10 mà đụng cùng keyword. Không có cửa.
5. **Không cập nhật theo quý** — danh mục keyword 2 năm trước có thể đã lỗi thời (slang mới, thuật toán mới, đối thủ mới).
6. **Spam keyword (keyword stuffing)** — nhồi keyword 30 lần trong bài 1.000 từ. Google phạt, người đọc khó chịu.
7. **Bỏ qua long-tail** — chỉ săn head term. Bỏ phí 70% cơ hội (long-tail = 70% tổng search Google).
8. **Không map vào funnel** — toàn keyword TOFU → traffic mà không bán. Toàn BOFU → không ai biết tới.
9. **Không track ROI từng cluster** — không biết cluster nào ra tiền, cluster nào tốn công vô ích → không biết cắt cái gì.
10. **Cố rank từ KD quá cao khi site còn yếu** — site mới đụng KD 60+. 12 tháng vẫn page 5. Đáng lẽ nhắm KD 10-25 thì 6 tháng đã có kết quả.

## 📅 Lịch review định kỳ (4 tầng)

| Tần suất | Thời gian | Hoạt động chính |
|---|---|---|
| **Hàng tuần** *(sáng T2, 1-2h)* | Đều đặn | GSC top 10 query mới → quyết định thêm vào master list. Cập nhật position keyword đang theo. |
| **Hàng tháng** *(đầu tháng, 3-4h)* | Đầu tháng | Review tất cả cluster: cluster nào tốt/yếu. Cluster yếu phân tích lý do. Đăng/cập nhật ≥ 4 nội dung. Refresh 1-2 nội dung cũ tụt position. |
| **Hàng quý** *(đầu quý, 1 ngày)* | Đầu Q | Chạy lại keyword research từ đầu cho 1-2 cluster trọng điểm. Audit toàn master list. So sánh đối thủ tìm gap mới. Lập kế hoạch 90 ngày. |
| **Hàng năm** *(tháng 1, 2-3 ngày)* | Đại tu | Đại tu master list. Lập chiến lược content + keyword cả năm. Phân bổ ngân sách công cụ + ads. |

### Khi nào cần thay seed keyword
- Industry có thuật ngữ mới (slang, công nghệ, trend)
- Khách bắt đầu hỏi câu mà keyword cũ không bắt
- Đối thủ chuyển sang positioning mới
- Algorithm Google đổi (vd: ưu tiên video) → cần seed phù hợp định dạng mới

## 🛠️ Tools đầy đủ

> Em đã tách thành 3 trang riêng để vận hành — anh nhớ dùng:
> - [[AI Prompts - Keyword Research]] — 7 prompt mẫu copy-paste
> - [[Template Google Sheet Keyword Master]] — 20 cột + 4 tab + 4 view filter + CSV mẫu
> - [[Checklist Keyword Research]] — 1 trang in tường cho nhân viên
> - [[Map keyword vào 7 kênh]] — bảng map keyword → kênh phân phối

## 📊 SERP Features (đọc kỹ)

SERP ngày nay không chỉ có 10 link xanh. Cần kiểm:

| Feature | Hành động |
|---|---|
| **Featured snippet** | Cố giành — traffic gấp **3-5 lần P1 thường** |
| **People Also Ask (PAA)** | Lấy câu hỏi làm sub-heading |
| **Map Pack** | Local SEO bắt buộc → Google Business Profile |
| **Video carousel** | Làm YouTube |
| **Image pack** | Tối ưu ảnh + alt text |
| **Shopping ads** | Cân nhắc Google Shopping |

## 🎯 Hành động cho anh Chương — Áp dụng để chốt ngách TPCN

1. **2 ngày tới (deadline 11/05/2026):** Dịch 3 persona TPCN sơ bộ (vd: trung niên đau khớp, phụ nữ 30-45 đẹp da, người bận tăng đề kháng) → 30 seed keyword. 5-7 câu/persona theo văn nói thật của họ + 5-10 seed từ tên đối thủ Shopee/TikTok Shop.
2. **Buổi sáng tuần này:** Chạy Google autocomplete + AnswerThePublic cho 5 seed hàng đầu → 80-150 keyword biến thể.
3. **Cuối tuần:** Áp [[Rubric 10 điểm lọc keyword]] → lọc xuống 30 keyword vàng. **Nếu một ngách KHÔNG ra đủ 30 keyword có intent rõ → ngách quá nhỏ, bỏ.**
4. **Trong tuần:** Kiểm tra SERP thực tế top 10 keyword điểm cao nhất → tìm content gap. Để ý Map Pack (→ Google Business) và Video carousel (→ TikTok/YouTube ưu tiên).
5. **Trước hết tháng:** Lập bản đồ 3 cluster đầu tiên → gán: kênh chính, người phụ trách, deadline đăng đầu tiên, KPI 60 ngày.

## 💬 Trích dẫn

> "Từ khoá là suy nghĩ của khách viết ra bằng chữ."
> "30 keyword được lọc kỹ + làm sâu mạnh hơn 300 keyword làng nhàng."
> "Keyword research không phải việc làm 1 lần rồi xong — nó là kỷ luật hàng tuần."
> "Nếu rank top 3, mình có ra được đơn không?"
> "Khi tôi gõ keyword này vào Google, có một con người thật đang gõ giống tôi không?"
> "Volume + KD đẹp nhưng SERP toàn site authority cao → vô vọng."
> "Nếu tiệm chỉ rank được ở BOFU thì cuộc đua khốc liệt và đắt."

## 🎯 3 câu tự kiểm cuối tháng

1. **"Khi tôi gõ keyword này vào Google, có một con người thật đang gõ giống tôi không?"** — Nếu không chắc = keyword chết.
2. **"Nếu rank top 3 cho keyword này, công ty có thêm tiền không?"** — Nếu không = không đáng tốn.
3. **"Trong 100 keyword đang theo, có 30 keyword sẵn sàng đặt cược 6 tháng làm không?"** — Nếu không = cần lọc lại.

## ❓ Câu hỏi mở

- Ngành TPCN VN có bao nhiêu ngách đủ volume (≥ 200/tháng) mà KD ≤ 30?
- Anh Chương có lợi thế chuyên môn ở ngách TPCN nào?
- Bắt đầu bằng kênh nào: blog SEO (bền, chậm 3-9 tháng) hay TikTok/YouTube (nhanh, phụ thuộc algo)?
- Đối thủ TPCN nào đang rank tốt nhất Google VN? (chạy Content Gap Ahrefs)
- Mục tiêu 20 tỷ/tháng cần bao nhiêu organic traffic + conversion rate? (bài toán ngược)
- Có nên ưu tiên local keyword cho 1 số tỉnh/TP trước, hay đánh toàn quốc ngay?
