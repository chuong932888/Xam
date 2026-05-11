---
type: source
tags: [ips, khoi-14, ads, paid-media, ptl]
created: 2026-05-09
updated: 2026-05-09
sources: ["[[raw/Đặc sản của Phạm Thành Long/IPS - 19 khối công việc/14_ ADS Các nền tảng]]"]
khoi: 14
---

# Khối 14 — ADS Các nền tảng (Tổng quan)

> Nguồn: thầy [[Phạm Thành Long]], khoá [[index|IPS]]. **6 file gốc** trong folder `14_ ADS Các nền tảng/`:
> - ADS FACEBOOK.docx (34KB, 443 dòng) → [[Khối 14a - ADS Facebook]]
> - ADS GOOGLE.docx (31KB, 477 dòng) → [[Khối 14b - ADS Google]]
> - ADS TIKTOK.docx (33KB, 395 dòng) → [[Khối 14c - ADS TikTok]]
> - ADS YOUTUBE.docx (36KB, 391 dòng) → [[Khối 14d - ADS YouTube]]
> - Phân tích chỉ số quảng cáo.docx (30KB, 521 dòng) → [[Khối 14e - Phân tích chỉ số ads]]
> - Từ cấm FB + bí thuật VPCS.docx (12KB, 82 dòng) → [[Khối 14f - Từ cấm FB Ads (cảnh báo nhân viên)]]

> ⚠️ **Tổng quát phân biệt nguồn**:
> - ✅ **PTL gốc nói**: cấu trúc, công thức, số liệu, case study được ghi nguyên trong tài liệu.
> - 📎 **Em (agent) thêm**: ngữ cảnh áp dụng TPCN, một vài cảnh báo pháp lý VN, đánh dấu inline.
> - ⚠️ **Lỗi gốc đã phát hiện** trong QA: footnote citation lệch ở 3/6 file, mốc thời gian "Data Studio" lỗi thời, số "1,8 tỷ DAU FB" lỗi thời (đã sửa hoặc đánh dấu ở từng sub-page).

## 🎯 TL;DR — 1 trang đọc 5 phút

**ADS 2026 không phải trò "vặn target" hay mua click rẻ** — là hệ thống **phân phối xác suất dựa trên dữ liệu, chất lượng quảng cáo và tín hiệu chuyển đổi**. Mỗi nền tảng có cơ chế đặc trưng:

| Nền tảng | Đặc trưng | Điểm mạnh | Khi dùng cho TPCN |
|---|---|---|---|
| **Facebook** | Phân phối xác suất; Advantage+ AI hoá; broad audience > target chi tiết | Remarketing + e-commerce + lead gen | Always-on chính, scale mass-market |
| **Google** | Bắt nhu cầu có sẵn (intent cao); Smart Bidding | Search bắt người chủ động tìm; PMax all-channel | Khi keyword TPCN có volume; ngách rõ |
| **TikTok** | GMV Max mặc định từ 7/2025 cho Shop; creative-first | Bùng nổ doanh số trong Shop + LIVE | Khi có TikTok Shop + creator pipeline |
| **YouTube** | 3 loại conversion (click/engaged-view/view-through); 5s đầu quyết định | Branding + nuôi nóng audience + retargeting | Khi có asset video + cần build nhận biết |

**5 nguyên tắc chung tất cả nền tảng**:
1. **Tracking sạch trước khi scale** — pixel/tag bắn đúng + dedup đúng + event mapping đúng.
2. **Chọn objective đúng theo mục tiêu kinh doanh** — đừng tối ưu click nếu cần lead/sale.
3. **Creative là biến số số một** — đặc biệt TikTok/YouTube/Reels (TPCN ngách bị bóp organic, paid creative càng quan trọng).
4. **First-party data + remarketing > interest** — list KH cũ + visitor 30/180 ngày là vàng.
5. **Đo lường đa lớp** — last click không đủ; cần data-driven attribution + view-through cho video + offline conversion cho lead gen.

**3 sai lầm chết người người mới hay vướng** *(chung cả 4 nền tảng)*:
- Chạy trước khi đo. Tracking lỗi → mọi báo cáo sau đều không đáng tin.
- Chia nhỏ ad set/campaign quá sớm → learning limited (50 events/tuần không đạt).
- Chấm KPI cuối phễu (sale) chỉ bằng last click → đánh giá thấp YouTube/Display/upper funnel.

## 🧭 Mục đích trong IPS — Vai trò Khối 14 với TPCN

- **Khối 14 = đòn bẩy tốc độ**. Khối 1-13 xây nền (hồ sơ KH, keyword, kênh, blog, email, sale page). Khối 14 **đốt nhiên liệu** để máy bán hàng quay nhanh hơn.
- **Roadmap anh Chương**: T3 dựng kênh truyền thông → **T4 chạy quảng cáo → 1 tỷ doanh thu/tháng**. Khối 14 là chìa khoá KPI T4.
- **Đặc thù TPCN ngành YMYL**:
  - Facebook + Google + TikTok đều có chính sách Health/YMYL nghiêm — bài kém duyệt sẽ bị bóp impressions.
  - Cần bác sĩ chuyên môn (xương sống E-E-A-T từ [[Khối 9 - SEO Blog 2026]]) cho creative + landing page tin cậy.
  - "Thực phẩm chức năng" nằm trong từ cấm Facebook → ngách đặc biệt khó (chi tiết: [[Khối 14f - Từ cấm FB Ads (cảnh báo nhân viên)]]).

## 🏗️ Sơ đồ vai trò nhân sự (gộp với roadmap IPS)

Mỗi nền tảng = 1 nhân sự ads chuyên trách → đội ngũ 4-5 người ở giai đoạn quy mô:

```
Trưởng Quảng cáo (Khối 14 owner)
├── Ads FB Specialist        → [[Khối 14a - ADS Facebook]]
├── Ads Google Specialist    → [[Khối 14b - ADS Google]]
├── Ads TikTok Specialist    → [[Khối 14c - ADS TikTok]]
├── Ads YouTube Specialist   → [[Khối 14d - ADS YouTube]]
└── Data + Tracking Specialist → [[Khối 14e - Phân tích chỉ số ads]]
                              + [[UTM template chuẩn 4 nền tảng]]
                              + [[Checklist QA tracking đa kênh]]
```

Toàn đội đọc bắt buộc: **[[Khối 14f - Từ cấm FB Ads (cảnh báo nhân viên)]]** — checklist từ tránh + cảnh báo pháp lý.

## 📋 Lộ trình triển khai 30/60/90 ngày (chuẩn cho ADS từ T4)

> Hợp nhất từ 4 lộ trình của 4 nền tảng — đây là khung CHUNG PTL khuyên cho người mới.

| Giai đoạn | Mục tiêu | Việc cần làm | Tiêu chí đạt |
|---|---|---|---|
| **30 ngày** — Xây nền | Hạ tầng + baseline | Setup Business Portfolio (FB) + Google Ads account + TikTok Business Center + YouTube link Google Ads. Cài Pixel/Tag + CAPI/Server-side + Event Manager. Verify domain. Chuẩn hoá conversion goals (Primary). Tạo Author profile + GA4. Chuẩn bị 15-30 video creative đầu. Launch 2-3 campaign mỗi nền tảng. | Tracking 100% sạch; conversion event chạy đúng; campaign live có data baseline. |
| **60 ngày** — Máy test | Tối ưu có kỷ luật | TOF/MOF/BOF cho mỗi nền tảng. Custom audience + Lookalike. A/B test 1 biến/tuần. Automated rules. Đọc lead quality từ CRM. | Biết creative thắng vì sao + biết nút thắt phễu. |
| **90 ngày** — Khuếch đại | Scale có kiểm soát | Catalog/Dynamic remarketing. Value optimization. Offline events import. Conversion Lift / MMM. PMax + GMV Max. | Scale + số liệu sạch + không phụ thuộc 1 ad. |

## 🚦 Checklist 7 bước tối thiểu chung tất cả nền tảng

> Người mới TUYỆT ĐỐI không bỏ qua bước nào. Theo quy tắc PTL: "Không cài đo lường xong thì không bật ngân sách."

1. ☐ **Tài khoản & quyền**: BM/Business Center + Ad Account + 2FA + verify domain.
2. ☐ **Tracking**: Pixel/Tag + CAPI/Server-side + GA4 + dedup đúng + Event Match Quality kiểm tra.
3. ☐ **Conversion goals**: 1 Primary action/campaign + Secondary để học. Không đặt micro-conversion vào Primary.
4. ☐ **Audience**: TOF/MOF/BOF + custom audience tối thiểu 100-1000 users + lookalike từ purchaser/qualified lead.
5. ☐ **Creative**: video dọc 9:16 + ngang 16:9 + vuông 1:1; hook 3-5s đầu; CTA rõ; 3-5 góc khác biệt.
6. ☐ **Landing page**: khớp ad + CTA chính 1 cái + tốc độ ≤2.5s mobile + form ngắn nhất.
7. ☐ **Compliance**: review từ cấm FB ([[Khối 14f - Từ cấm FB Ads (cảnh báo nhân viên)]]) + check Special Ad Category cho Health/TPCN.

## 📊 KPI tổng & ngưỡng cảnh báo (chung 4 nền tảng)

> Chi tiết từng nền tảng ở sub-page; bảng dưới là **ngưỡng tham chiếu nhanh** trích từ [[Khối 14e - Phân tích chỉ số ads]].

| Tầng phễu | Chỉ số | Hỏi câu gì | Cảnh báo khi |
|---|---|---|---|
| **Awareness** | Reach, Impressions, CPM, **Frequency** | "QC có đến đúng người không?" | Frequency >3-5 = cháy tệp |
| **Consideration** | CTR, CPC, View Rate, Engagement | "Họ có quan tâm không?" | CTR < benchmark ngành = creative/target sai |
| **Conversion** | CR, CPA, **ROAS** | "Họ có mua/đăng ký không?" | CPA ≥ biên LN sản phẩm = lỗ; ROAS <1 = lỗ trực tiếp |

→ Đọc cụm chỉ số, không đọc lẻ. Vd: CTR cao + CR thấp = lỗi landing page. Chi tiết: [[Khung diagnose phễu]].

## 💬 Trích dẫn xuyên suốt 6 file

> "Đừng tối ưu từ Ads Manager, hãy tối ưu từ đường đi mua hàng." *(TikTok, gốc dòng 6)*

> "Smart Bidding không chữa được tracking sai." *(Google, gốc dòng 6)*

> "Đừng bắt đầu bằng target — bắt đầu bằng kết quả kinh doanh muốn mua." *(Facebook, gốc dòng 49)*

> "5 giây đầu quyết định bạn có được xem tiếp không." *(YouTube, gốc dòng 7)*

> "Chỉ số là phương tiện, lợi nhuận mới là mục đích." *(Phân tích chỉ số, dòng 508)*

> "Quảng cáo tốt mà shop fulfillment tệ thì vẫn gãy hệ thống." *(TikTok, gốc dòng 264)*

## 🎯 Hành động cho anh Chương — 5 việc cần làm (chuẩn bị T4)

> Đã đẩy vào [[../../actions|actions.md]] — chi tiết deadline.

1. **Trước T4**: Quyết **chiến lược white-hat vs grey-hat** cho ads TPCN. Em nghiêng white-hat — phù hợp commitment 24 tháng.
2. **Trước T4**: Tư vấn pháp lý **Luật QC 16/2012/QH13 + Nghị định 38/2021** + xác nhận nội dung quảng cáo bởi **Cục An toàn thực phẩm** trước khi viết creative đầu tiên.
3. **Tháng 5-6**: Setup hạ tầng đo lường — Pixel + CAPI + Tag + Server-side + GA4 + UTM + dashboard Looker Studio gom 4 nền tảng. **Không bật ngân sách trước khi tracking sạch**.
4. **Tháng 5-6**: Quyết định **ROAS mục tiêu** cho từng SKU TPCN dựa biên LN cụ thể — TPCN gross margin 60-80% → ROAS 3-5x giai đoạn đầu (xem [[Khối 14e - Phân tích chỉ số ads]] mục 5).
5. **Cả đội đọc**: [[Khối 14f - Từ cấm FB Ads (cảnh báo nhân viên)]] + [[Special Ad Category + chính sách Health-YMYL]] **TRƯỚC khi viết creative đầu tiên**.

## 🔗 Liên kết

### 6 sub-page Khối 14
- [[Khối 14a - ADS Facebook]] — Meta ecosystem, Advantage+, Pixel/CAPI, learning phase 50 events, 6 case study
- [[Khối 14b - ADS Google]] — 5 campaign types, Smart Bidding, Quality Score, RLSA, 4 case study
- [[Khối 14c - ADS TikTok]] — GMV Max mặc định 7/2025, 4 nhóm audience, 6 case study
- [[Khối 14d - ADS YouTube]] — 7 format video, 3 loại conversion, 5s hook
- [[Khối 14e - Phân tích chỉ số ads]] — 43 chỉ số, công thức, benchmark, diagnose phễu
- [[Khối 14f - Từ cấm FB Ads (cảnh báo nhân viên)]] — 9 nhóm từ tránh + cảnh báo VPCS + pháp lý VN

### 11 concept page (xuyên nền tảng)
- [[Learning Phase (50 events tuần)]] — chung Meta + TikTok
- [[TOF-MOF-BOF Funnel + Audience Layers]] — chung tất cả
- [[Pixel + CAPI + Event Deduplication]] — chung Meta + TikTok
- [[Advantage+ Family]] — Meta
- [[Smart Bidding (Google)]] — Google
- [[Quality Score vs Ad Rank]] — Google
- [[GMV Max - Product vs LIVE]] — TikTok
- [[5s Hook + Khung kịch bản video]] — YouTube/TikTok
- [[3 loại Conversion Click-Engaged-View-View-Through]] — YouTube/Google
- [[Khung diagnose phễu]] — bảng triệu chứng → nguyên nhân → hành động
- [[Special Ad Category + chính sách Health-YMYL]] — **bắt buộc đọc cho TPCN**
- [[ROAS theo biên lợi nhuận]] — quyết ngưỡng có lãi

### 2 tools
- [[Checklist QA tracking đa kênh]] — Pixel/CAPI/UTM hàng tuần
- [[UTM template chuẩn 4 nền tảng]] — copy-paste ready

### Khối IPS liên quan
- [[Khối 1 - Hồ sơ khách hàng]] — chốt persona TRƯỚC khi viết creative
- [[Khối 2 - Cách tìm kiếm từ khoá]] — keyword feed cho Google Search Ads
- [[Khối 9 - SEO Blog 2026]] — landing page chuẩn E-E-A-T
- [[Khối 10 - Squeeze Page]] — landing page chuẩn cho lead gen ads
- [[Khối 13 - SEO sản phẩm Website]] — landing page sản phẩm cho FB/Google Shopping
- [[Phạm Thành Long]] — tác giả tài liệu gốc
