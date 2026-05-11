---
type: source
tags: [ips, khoi-18, san-tmdt, shopee, lazada, tiktok-shop, ptl]
status: active
created: 2026-05-09
updated: 2026-05-09
sources: ["[[raw/Đặc sản của Phạm Thành Long/IPS - 19 khối công việc/18_ Sàn thương mại ĐT]]"]
khoi: 18
---

# Khối 18 — Sàn thương mại điện tử (Tổng quan)

> **Nguồn**: thầy [[Phạm Thành Long]], khoá [[index|IPS]]. **3 file gốc** trong folder `18_ Sàn thương mại ĐT/`:
> - `Shopee.docx` (30KB, 205 đoạn) → [[Khối 18a - Shopee]]
> - `Lazada Seller.docx` (31KB, 234 đoạn) → [[Khối 18b - Lazada]]
> - `Tiktok.docx` (593KB, 482 đoạn) → [[Khối 18c - TikTok Shop]]

> ⚠️ **Cảnh báo về ví dụ trong tài liệu gốc**: Tài liệu PTL dùng **ví dụ minh hoạ là sản phẩm ngành xăm** (máy xăm pen, kim cartridge 1207RL, mực liner, giấy stencil...) vì PTL viết đúng cho ngữ cảnh anh Chương đang vận hành công ty cũ. **Đây không phải kiến thức xăm**, chỉ là vỏ ví dụ để làm rõ công thức bán sàn TMĐT. Khi áp dụng cho **TPCN**, anh dịch sang ví dụ TPCN tương ứng (vd: máy xăm pen → viên uống collagen, kim 1207RL → hộp 30 viên, stroke 4mm → liều dùng 1000mg/ngày).

> **Phân biệt nguồn trong page**:
> - ✅ **PTL gốc nói**: cấu trúc, công thức, số liệu, tài liệu Shopee/Lazada/TikTok seller center, citation [n] có sẵn.
> - 📎 **Em (agent) thêm**: ngữ cảnh áp dụng TPCN, gợi ý TPCN-specific, đánh dấu inline.
> - ⚠️ **Lưu ý cần xác minh**: các ngưỡng phí/policy có thể đã đổi sau ngày tài liệu được viết — phải check Seller Center thật trước khi triển khai.

## 🎯 TL;DR — 1 trang đọc 5 phút

**Bán sàn TMĐT 2026 không phải "đăng sản phẩm rồi chờ đơn"** — là **vận hành một hệ thống tăng trưởng khép kín** với 5 lớp khoá vào nhau:
1. **Độ khớp truy vấn** (relevance): title + category + thuộc tính + brand đúng.
2. **Chất lượng trang sản phẩm** (listing quality): ảnh + mô tả + thông số + giá đúng.
3. **Bằng chứng xã hội** (social proof): review + UGC + creator + LIVE.
4. **Độ tin cậy vận hành** (trust ops): tồn kho + giao hàng + CSKH + tỷ lệ hoàn.
5. **Khả năng nhân rộng bằng quảng cáo** (paid scaling): ads thông minh sau khi 4 lớp trên đã sạch.

**Chiếm "Top 1" theo nghĩa thực chiến** = chiếm vị trí hàng đầu trên **cụm truy vấn mục tiêu**, **có lợi nhuận dương**, **đủ lâu để tạo tín hiệu bán hàng và review** — KHÔNG phải đứng số 1 tuyệt đối cho mọi người dùng (vì cả 3 sàn đều cá nhân hoá hiển thị theo từng người mua).

| Sàn | Đặc trưng cốt lõi | Đòn bẩy quan trọng nhất 2026 | Khi dùng cho TPCN |
|---|---|---|---|
| **Shopee** | Hiển thị cá nhân hoá; campaign chính thức + voucher + flash sale + Tối đa Doanh thu | Hero SKU + preheat 14 ngày + war room ngày sale | Always-on chính cho TPCN VN — voucher/flash sale là vũ khí kéo doanh số |
| **Lazada** | 4 tầng: index → CTR → CVR → momentum; Sponsored Discovery + Max + LazMall | Manual exact cho 5-10 keyword tiền mặt + Sponsored Max khi đủ data | Tốt cho TPCN nhập khẩu, ngành cao cấp; LazMall cho thương hiệu chính hãng |
| **TikTok Shop** | GMV Max mặc định từ 7/2025; affiliate + LIVE + creator + Shop Ads | 10-20 Hero SKU + content engine + GMV Max always-on | Đòn bẩy mạnh nhất 2026 — TikTok Shop tăng 93% doanh thu/năm, thị phần 39.6% |

**5 nguyên tắc chung cả 3 sàn**:
1. **Hero SKU trước, mở rộng sau**: chọn 5-20 SKU chiến lược, dồn 80% lực vào đó. Đừng "mở quá nhiều SKU" — traffic loãng, thuật toán không đủ tín hiệu.
2. **Listing sạch trước khi tăng ads**: title + ảnh + mô tả + thuộc tính + giá đúng → rồi mới chạy ads. Ads chỉ khuếch đại thứ đã bán được.
3. **Biên đóng góp ở cấp đơn hàng**, không phải GMV. Tính lãi sau **mọi chi phí**: phí sàn + phí xử lý + VAT trên phí + voucher + ads + đóng gói + dự phòng hoàn/hủy.
4. **Vận hành sạch là SEO thực thụ**: chỉ số NFR/LSR/CRR/AHR/positive rating tác động trực tiếp lên hiển thị, không chỉ trải nghiệm khách.
5. **Không sửa lung tung trong 7 ngày đầu**: thuật toán cần thời gian học. Sửa quá sớm = phá learning phase. Mỗi lần sửa phải ghi log.

**3 sai lầm chết người chung cả 3 sàn**:
- Vào campaign khi listing còn yếu → đốt ngân sách + lộ điểm yếu nhanh hơn.
- Voucher/flash sale đại trà toàn shop → margin tốt gánh margin xấu.
- Đo theo GMV/doanh số mà không đo lãi đơn → tưởng thắng nhưng đốt tiền.

## 🧭 Mục đích trong IPS — Vai trò Khối 18 với TPCN

- **Khối 18 = kênh bán mass-market cho TPCN**. TPCN cần niềm tin (xem [[Khối 9 - SEO Blog 2026]]) và quảng cáo (xem Khối 14), nhưng **sàn TMĐT vẫn là nơi khách Việt có ý định mua thực tế** — đặc biệt sau khi đã được nuôi nóng qua [[Khối 5 - Chiến lược TikTok]] / [[Khối 4 - Chiến lược Facebook Fanpage]] / blog.
- **Vị trí trong [[Luồng khách hàng]]**: Sàn TMĐT là **nơi chốt đơn** ở giai đoạn cuối phễu — sau khi khách đã biết đến brand qua content, đã tin qua review/blog, đã được retarget qua ads.
- **Khác với website riêng**: sàn có sẵn **traffic + niềm tin + thanh toán + vận chuyển** → giảm rào cản mua. Đổi lại: phí sàn cao + phụ thuộc thuật toán + khó remarketing trực tiếp.
- **Vai trò nhân sự**: 1 Trưởng E-commerce (chiến lược) + 1-2 nhân viên SEO sản phẩm + 1 nhân viên ads sàn + 1-2 nhân viên CSKH (chia ca chat) + 1 nhân viên LIVE (TikTok Shop). Khi shop nhỏ có thể gộp.

## 🏗️ 6 đòn bẩy cốt lõi xuất hiện ở cả 3 sàn

PTL nói rõ trong file Shopee (và logic này áp dụng được cho cả Lazada/TikTok):

```
Lợi nhuận ròng = Lượt truy cập × CTR × CVR × AOV × biên gộp
                  – phí sàn – phí xử lý giao dịch – VAT trên phí
                  – trợ giá voucher/freeship – chi phí quảng cáo
                  – đóng gói – hao hụt/đổi trả – chi phí vận hành
```

**Sai phổ biến nhất**: chỉ nhìn GMV hoặc số đơn. **Đúng phải nhìn**: contribution margin (lợi nhuận đóng góp trên mỗi đơn) ở **cấp SKU**, vì campaign thắng mà lỗ biên thì chỉ là tăng trưởng giả.

| Đòn bẩy | Cách đo | Cách tăng |
|---|---|---|
| Lượt truy cập (Impressions) | Search impressions + recommend impressions | SEO listing đúng + ads đúng từ khoá |
| CTR | Impressions → Clicks | Ảnh 1, title rõ, giá tốt, freeship/voucher visible, rating ≥4.5 |
| CVR | Clicks → Orders | PDP đầy đủ thông tin, review tốt, FAQ rõ, combo, voucher chốt đơn |
| AOV | Doanh thu / số đơn | Combo, upsell, voucher ngưỡng đơn tối thiểu |
| Biên gộp | (Giá bán – giá vốn) / giá bán | Đàm phán giá vốn, giảm chi phí đóng gói, tối ưu mix sản phẩm |
| Chỉ số vận hành | NFR, LSR, CRR, response time | Stock buffer, ca trực rõ, quy trình đóng gói chuẩn |

## 📚 Khi nào đọc sub-page nào?

| Tình huống | Đọc page nào trước |
|---|---|
| **TPCN bắt đầu vào sàn — chọn 1 sàn để mở** | Đọc cả 3, nhưng ưu tiên [[Khối 18c - TikTok Shop]] (đang tăng trưởng mạnh) hoặc [[Khối 18a - Shopee]] (thị phần lớn nhất, mass) |
| **Đã có shop Shopee, muốn đẩy doanh số** | [[Khối 18a - Shopee]] — phần "Cách thắng chiến dịch" + "Lịch chạy chuẩn D-14 đến D+7" |
| **Cần SEO listing để lên top tìm kiếm** | Mỗi page đều có phần SEO riêng. Quy tắc chung: title đúng + thuộc tính đầy đủ + ảnh thật + review tốt |
| **Cần lập dashboard theo dõi shop** | [[Khối 18a - Shopee]] phần "Dashboard và chỉ số" + [[Khối 18b - Lazada]] phần "KPI dashboard tối thiểu" + [[Khối 18c - TikTok Shop]] phần "Quy trình đo chỉ số hằng ngày" |
| **Cần chuẩn bị campaign mega sale (11.11, 12.12, 4.4...)** | [[Khối 18a - Shopee]] phần "Lịch chạy chuẩn để thắng chiến dịch" |
| **Muốn vào LazMall hoặc shop chính hãng** | [[Khối 18b - Lazada]] phần "Chuẩn nội bộ nên dùng" + tiêu chí LazMall |
| **Cần SOP cho nhân viên SEO sản phẩm TikTok** | [[Khối 18c - TikTok Shop]] — có sẵn **SOP TTS-SEO-01** (10 bước SOP chính + phần phụ trợ: quy trình đo, lịch ngày/tuần, cây quyết định 4 trường hợp, checklist duyệt, mẫu phiếu, KPI nhân viên) |
| **Lập kế hoạch 30/60/90 ngày cho shop mới** | [[Khối 18a - Shopee]] phần "Kế hoạch 30/60/90" + [[Khối 18b - Lazada]] "Lộ trình 90 ngày" + [[Khối 18c - TikTok Shop]] "Lộ trình triển khai 3 tháng" |

## 🎯 Áp dụng vào TPCN — 3 hành động cụ thể

📎 *Em (agent) thêm — không có trong tài liệu gốc PTL.*

1. **Trước khi mở shop sàn cho TPCN, hoàn tất: hồ sơ KH ([[Khối 1 - Hồ sơ khách hàng]]) + keyword research ([[Khối 2 - Cách tìm kiếm từ khoá]])**. Lý do: 5 đòn bẩy đầu (relevance, listing, social proof, trust ops, ads) đều phụ thuộc vào việc hiểu **khách TPCN gõ gì khi tìm sản phẩm cho vấn đề của họ** (ngủ không ngon, viêm khớp, tăng đề kháng...).
2. **Chọn sàn theo ngách + giai đoạn**: TPCN cao cấp / chính hãng → LazMall (Lazada) là đòn bẩy niềm tin lớn. TPCN giá phổ thông + cần content nuôi nóng → TikTok Shop là kênh tăng trưởng mạnh nhất 2026. TPCN cần độ phủ + traffic mass-market → Shopee.
3. **YMYL warning**: TPCN thuộc nhóm Health & Personal Care — mọi sàn đều có quy định nghiêm ngặt về claim sức khoẻ. **Không được claim "chữa bệnh", "thay thế thuốc", "kết quả 100%"** trong title/ảnh/mô tả/video. Cần kiểm tra giấy phép TPCN, công bố sản phẩm, chứng nhận trước khi đăng.

## 🔗 Liên kết

- Quay lại [[index|IPS]] để xem 19 khối tổng thể.
- Bộ tài liệu gốc: `raw/Đặc sản của Phạm Thành Long/IPS - 19 khối công việc/18_ Sàn thương mại ĐT/`
- Mentor: [[Phạm Thành Long]]
- Khối liên quan đặc biệt:
  - [[Khối 14 - ADS Các nền tảng]] — ads nội sàn (Shopee Ads, Lazada Sponsored, TikTok Shop Ads) tương đồng nhiều với ads phễu ngoài
  - [[Khối 17 - Trả lời tin nhắn]] — chat shop là chỉ số CRR/response time tác động hiển thị
  - [[Khối 19 - Luồng khách hàng]] — sàn là điểm chốt đơn cuối phễu
