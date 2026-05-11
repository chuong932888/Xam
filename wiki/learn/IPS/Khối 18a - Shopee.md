---
type: source
tags: [ips, khoi-18, shopee, san-tmdt, ptl]
status: active
created: 2026-05-09
updated: 2026-05-09
sources: ["[[raw/Đặc sản của Phạm Thành Long/IPS - 19 khối công việc/18_ Sàn thương mại ĐT/Shopee.docx]]"]
khoi: 18
---

# Khối 18a — Làm chủ bán hàng Shopee và thắng chiến dịch

> **Nguồn**: thầy [[Phạm Thành Long]], khoá [[index|IPS]], file `Shopee.docx` (30KB, 205 đoạn).
> Tài liệu được PTL viết dựa trên Shopee Seller Center[1], Shopee Ads[2] và case study trong nước; có cập nhật chính sách phí và VAT giai đoạn 24/04–08/05/2026.
> Quay lại tổng quan: [[Khối 18 - Sàn thương mại điện tử]].

> ⚠️ **Cảnh báo về ví dụ ngành xăm trong tài liệu**: tài liệu PTL dùng ví dụ "máy xăm pen", "kim cartridge" trong phần mẫu title/mô tả vì viết cho ngữ cảnh anh Chương lúc đó. Nội dung **CỐT LÕI** (logic 6 đòn bẩy, lịch D-14 đến D+7, công thức ROAS/ACOS, dashboard, ma trận rủi ro) là **kiến thức bán Shopee áp dụng cho mọi ngành**, bao gồm TPCN. Anh dịch ví dụ sang TPCN khi áp dụng.

## 🎯 TL;DR

**Trên Shopee, "thắng" không đến từ một chiêu duy nhất** — đến từ hệ thống **6 đòn bẩy khoá vào nhau**: độ phủ truy vấn, CTR, CVR, AOV, chỉ số vận hành, và biên lợi nhuận sau toàn bộ chi phí.

**Công thức rút gọn cả tài liệu thành một câu**: chọn 3-5 hero SKU (sản phẩm chủ lực) có biên an toàn, **tối ưu trang sản phẩm trước**, **preheat ít nhất 14 ngày** trước campaign, sale-day chạy theo **war room**, hậu chiến dịch phải lấy review + khách quay lại.

Shopee Ads khuyến nghị chạy quảng cáo **ít nhất 2 tuần trước** giai đoạn cao điểm; vào ngày sale chi phí click có thể tăng nên **ngân sách tăng ít nhất gấp rưỡi**, ngày siêu sale có thể **gấp đôi**.

## 1. Khung chiến lược tổng thể

### 1.1 Công thức quản trị gốc (P&L)

```
Lợi nhuận ròng = Lượt truy cập × CTR × CVR × AOV × biên gộp
                 – phí sàn – phí xử lý giao dịch – VAT trên phí
                 – trợ giá voucher/freeship – chi phí quảng cáo
                 – đóng gói – hao hụt/đổi trả – chi phí vận hành
```

Sai phổ biến nhất: chỉ nhìn **GMV** hoặc số đơn. Đúng phải nhìn **contribution margin** ở **cấp SKU**, vì campaign thắng mà lỗ biên thì chỉ là tăng trưởng giả. Shopee đã **đổi tên "Phí Thanh Toán" thành "Phí Xử Lý Giao Dịch"**, điều chỉnh phí theo loại shop, và **áp VAT 10% trên phí dịch vụ** → bài toán lãi ròng phải tính ở cấp đơn hàng, không cảm tính.

### 1.2 Phân khúc khách 4 nhóm

| Nhóm | Đặc điểm | Đòn đánh |
|---|---|---|
| **Khách tìm kiếm mới** | Chưa biết shop, vào từ truy vấn cụ thể | SEO listing + ads search |
| **Khách so sánh** | Nhìn title, ảnh, giá, rating, số bán để chọn | Ảnh 1 nổi bật + giá tốt + nhiều review chất lượng |
| **Khách săn deal** | Phản ứng mạnh với flash sale, voucher, combo, live-exclusive | Voucher live + flash sale + kịch bản LIVE |
| **Khách quay lại** | Mua lặp lại, mua thêm phụ kiện | Voucher follower + upsell + bundle |

### 1.3 Kim tự tháp SKU

Không phải "bán thật nhiều SKU" — mà là 4 vai trò SKU:
- **Hero SKU**: kéo traffic và tín hiệu thuật toán.
- **Profit SKU**: giữ biên lợi nhuận.
- **Attach SKU**: bán kèm tăng AOV.
- **Repeat SKU**: kéo mua lại.

### 1.4 USP đo được, không nói chung chung

USP hữu dụng phải **đo được và nhìn thấy ngay ở title/ảnh/voucher**: giao nhanh, đủ phụ kiện, bảo hành rõ, đổi lỗi nhanh, giá theo combo tốt hơn, đúng thông số. KHÔNG viết "chất lượng tốt" — ai cũng nói vậy.

CTR chịu ảnh hưởng mạnh bởi: hình ảnh, tiêu đề, **thông tin nổi bật được lồng vào hình/tiêu đề**, và chương trình ưu đãi (freeship, hoàn xu, giảm giá, combo).

### 1.5 Bảng so sánh chiến lược theo quy mô shop

| Quy mô shop | Mô hình nên dùng | Số hero SKU | Mục tiêu chính | Nguồn traffic ưu tiên | Sai lầm chết người |
|---|---|---|---|---|---|
| **Mới** | Một ngành hàng hẹp, ít SKU nhưng rõ USP | 3 | Có đơn đầu, có review thật, giữ vận hành sạch | Tìm kiếm tự nhiên, voucher shop, flash sale shop, quảng cáo nhẹ | Mở quá nhiều SKU, chạy ads khi trang sản phẩm yếu |
| **Tăng trưởng** | Kim tự tháp: hero + attach + repeat | 5–10 | Scale doanh thu nhưng giữ biên | Campaign Shopee, search ads, livestream, combo | Chạy theo GMV, giảm giá vô tội vạ |
| **Lớn** | Danh mục theo cụm, ngân sách theo lợi nhuận biên | 10–30 | Tối đa hoá thị phần truy vấn và lợi nhuận | Tối đa Doanh thu, livestream/video, official campaign, CRM nội sàn | Dàn trải ngân sách, đổi cài đặt liên tục, thiếu postmortem |

### 1.6 Định giá 3 tầng

- **Giá niêm yết**: giữ khung tham chiếu, tạo room cho campaign.
- **Giá thường ngày có cạnh tranh**: không mất traffic nền.
- **Giá campaign**: chỉ áp cho hero SKU, có giới hạn thời gian và tồn kho.

**KHÔNG lấy "giá sale thật sâu" làm mặc định**. Giá ảo / sai lệch có thể bị Shopee xoá sản phẩm và tính điểm phạt.

### 1.7 Mô phỏng biên đóng góp theo quy mô shop

| Kịch bản giả định | Shop mới | Shop tăng trưởng | Shop lớn |
|---|---|---|---|
| AOV giả định | 150.000đ | 220.000đ | 320.000đ |
| Biên gộp sau giá vốn | 38% | 42% | 45% |
| Tổng phí sàn + xử lý + VAT trên phí | 10% | 11% | 12% |
| Voucher/freeship shop tài trợ | 4% | 5% | 6% |
| Ads phân bổ/đơn | 8% | 10% | 12% |
| Đóng gói + hao hụt + đổi trả dự phòng | 3% | 3.5% | 4% |
| **Biên đóng góp còn lại** | **13%** | **12.5%** | **11%** |

**Quy tắc thực chiến**: nếu biên đóng góp sau campaign **xuống dưới 8%** mà không có giá trị chiến lược rõ (mở khoá review, mở khoá khách mới, đẩy nhãn shop) → **không scale**.

### 1.8 Tồn kho & logistics

- Cập nhật kho ít nhất 1 lần/tuần, không kê vượt tồn thực.
- Dự trữ tồn riêng cho Shopee nếu bán đa kênh.
- Thời gian chuẩn bị: hàng có sẵn 2 ngày, hàng đặt trước 7 ngày.
- Nếu tạm không xử lý đơn → bật **chế độ Tạm nghỉ** trước **ít nhất 1 ngày**.
- Quy mô lớn cân nhắc **Shopee Xử Lý** (Shopee Fulfilled): kho tập trung, nhận đơn, đóng gói, xử lý.

### 1.9 CSKH

Tin nhắn tự động phải có: giờ hoạt động, chương trình khuyến mãi, thông tin liên hệ. Quy trình chuẩn sau khách đặt hàng: xác nhận → đóng gói → theo dõi vận chuyển → **chủ động xin đánh giá khi khách đã nhận**.

## 2. Cách thắng chiến dịch Shopee

### 2.1 Nguyên tắc chọn campaign — 4 điều kiện đủ

Chỉ vào campaign khi SKU đáp ứng **đủ 4**:
1. Biên còn dương sau giảm giá.
2. Tồn kho đủ.
3. Trang sản phẩm đã tối ưu.
4. Shop đủ người xử lý đơn/chat.

Thứ tự ưu tiên công cụ:
- **Voucher shop luôn bật**.
- **Flash Sale shop** cho SKU kéo traffic.
- **Combo** để kéo AOV.
- **Campaign chính thức Shopee** để lấy độ phủ.
- **Livestream/video** cho cụm SKU cần giải thích / chốt nhanh.

Trên giao diện app: khi khách vào shop, **voucher và Flash Sale shop hiện trước**. Seller Education khuyến nghị nên có **>1 mã giảm giá đang hoạt động**.

### 2.2 Lịch chạy chuẩn D-14 đến D+7

Lịch đúng KHÔNG bắt đầu vào ngày sale — bắt đầu ở **D-14**.

| Giai đoạn | Việc làm |
|---|---|
| **D-14 đến D-8** | Chọn hero SKU, sửa title/ảnh/thuộc tính, bật quảng cáo tìm kiếm, gom dữ liệu query, bắt đầu bỏ giỏ |
| **D-7 đến D-3** | Chốt voucher, combo, flash sale, lịch live, phân ca chat, phân ca đóng gói |
| **D-2 đến D-1** | Khoá tồn kho, nạp ngân sách, chuẩn bị kịch bản sale-day, tạo dashboard theo giờ |
| **D-day** | War room **2 giờ/lần**, chỉ đụng các biến có tác động lớn (ngân sách, bid, voucher, live slot) |
| **D+1 đến D+7** | Lấy review, bóc dữ liệu query, bóc SKU lời/lỗ, làm postmortem (KHÔNG để campaign kết thúc mà không có postmortem) |

Ngân sách: **tăng ít nhất gấp rưỡi** vào kỳ cao điểm; ngày siêu sale có thể **gấp đôi**. Bid cao hơn ngày thường.

### 2.3 Voucher xếp tầng theo mục tiêu

| Loại voucher | Mục tiêu | Cách dùng |
|---|---|---|
| Voucher kéo click | Cho hero SKU | Mệnh giá dễ nhìn |
| Voucher chốt đơn | Tăng AOV | Đặt ngưỡng giá trị đơn tối thiểu |
| Voucher follower | Lấy người theo dõi + khách quay lại | Tặng khi follow shop |
| Voucher live/video | Chỉ phát trong live hoặc gắn nội dung ngắn | "Giá chỉ có trên Live"; mã giảm giá chỉ hiện với người đang xem |

Tính năng Shopee LIVE liên quan: **Kịch bản Livestream** (soạn trước theo sản phẩm), **Phân tích Chuyên sâu** (đọc hiệu suất phiên).

### 2.4 Flash Sale shop — chỉ dùng cho 2 loại SKU

- Hero SKU cần đẩy tốc độ bán.
- SKU tồn cần xả có kiểm soát.

KHÔNG dùng cho SKU biên mỏng hoặc content yếu — sẽ tự đốt biên.

### 2.5 Bid CPC + điểm liên quan

Trên Shopee Ads, **thứ kiểm soát trực tiếp = bid CPC + mục tiêu ROAS**; còn **"điểm" quan trọng = điểm liên quan**, chịu tác động của:
- Độ liên quan từ khoá.
- Hành vi người dùng.
- Độ phổ biến sản phẩm.
- Hiệu suất vận hành của shop.

**Bid cao mà trang sản phẩm kém vẫn thua.**

Khuyến nghị từ khoá:
- **Từ khoá chính xác** cho từ ngắn, chung, cạnh tranh cao → kiểm soát chi phí.
- **Từ khoá mở rộng** cho cụm dài, mô tả rõ → CVR tốt hơn, cạnh tranh thấp hơn.
- Xem **lịch sử cụm từ tìm kiếm** trong báo cáo chi tiết để lọc query mạnh.
- Truy tìm **từ khoá ngách**: biến thể sai chính tả, viết tắt, cách gọi vùng miền.
- KHÔNG bid vào từ quá chung như chỉ tên thương hiệu hoặc tên thiết bị quá rộng → tốn tiền, lệch ý định mua.

Shop mới: bắt đầu bằng **giá thầu tự động** hoặc **Tối đa Doanh thu** cho 3-5 SKU mạnh nhất, rồi mới chuyển dần sang thủ công khi hiểu query.
- Giá thầu tự động: có thể tăng/giảm tới **50%** theo xác suất chuyển đổi.
- Tối đa Doanh thu: tối ưu theo ROAS trên nhiều vị trí. Khi tối ưu, **hạn chế thay đổi nhiều trong 1 ngày**, nếu cần điều chỉnh giữ trong **±20%** để không phá quá trình học.

### 2.6 A/B testing có kỷ luật

- Mỗi lần chỉ test **1 biến**: title / ảnh bìa / giá / voucher / live-thumbnail / bid.
- Giữ nguyên các biến còn lại.
- KHÔNG kết luận trước khi SKU có **ít nhất 7 ngày dữ liệu** hoặc đủ số nhấp/đơn tối thiểu.
- Test theo cụm truy vấn, không test trên toàn danh mục cùng lúc.
- **KHÔNG sửa liên tục**: thay đổi nhiều lần trong ngày làm gián đoạn quá trình học của hệ thống.

### 2.7 Livestream — booth chốt đơn, không phải chương trình giải trí

Live hiệu quả khi shop dùng nó như **thiết bị chốt đơn theo kịch bản**:
- 3 phút mở đầu kéo người xem.
- 10-15 phút demo hero SKU.
- 3 phút upsell/bundle.
- 2 phút chốt bằng voucher/live price.

Nghiên cứu live commerce: chất lượng phát trực tiếp, mức độ tương tác, giá trị cảm nhận, cảm giác giảm bất định đều ảnh hưởng rõ tới ý định mua. Video tăng ý định mua nhờ tăng lượng thông tin.

### 2.8 Case study từ Shopee Ads

Quảng cáo có thể đóng góp **25%–60% số đơn**, ROAS từ **20x đến 43x**. Đây không phải benchmark trung bình, nhưng chứng minh: khi sản phẩm cạnh tranh, giá hợp lý, nội dung tốt, vận hành ổn → paid traffic là động cơ tăng trưởng cực mạnh.

## 3. SEO Shopee để lên Top 1

### 3.1 Sự thật về Top 1

**KHÔNG có "Top 1 tuyệt đối" cho mọi khách hàng.** Shopee cá nhân hoá hiển thị theo từng người mua. Cách hiểu thực chiến: **chiếm top trên cụm truy vấn có giá trị, trong những phiên truy cập mục tiêu, đủ lâu để thuật toán thấy SKU này thật sự đáng được phục vụ**.

### 3.2 Nghiên cứu từ khoá — 4 lớp

1. **Seed keyword**: từ gốc theo ngành hàng và công dụng.
2. **Long-tail**: từ dài mô tả rõ nhu cầu, CVR tốt hơn.
3. **Ngách**: sai chính tả, viết tắt, vùng miền, cách gọi dân gian.
4. **Proof keyword**: query lấy từ báo cáo quảng cáo / search term report.

Công cụ phân tích thị trường: **Quân sư bán hàng** (Shopee Seller Education).

### 3.3 Title

Yêu cầu Shopee:
- Tiếng Việt có dấu, đủ ký tự, rõ nghĩa.
- Khớp với thông tin trên hình ảnh/sản phẩm.
- Khi quảng cáo không có hiển thị dù bid theo gợi ý → quay lại cải thiện tên sản phẩm và trang chi tiết.

**Bản chất**: title không chỉ để khách đọc — còn là **dữ liệu để hệ thống hiểu sản phẩm**.

**Công thức title**:
```
[Loại sản phẩm] + [thuộc tính chính] + [đối tượng/công dụng]
+ [thông số hoặc biến thể chính] + [thương hiệu nếu có]
```

KHÔNG nhồi nhiều từ khoá rác. Title đúng là title **làm tăng độ liên quan**, không phải dài vô tổ chức.

### 3.4 Mô tả sản phẩm — 6 khối

Yêu cầu Shopee: giải thích đặc tính, chất lượng, chức năng, lợi ích; đầy đủ kích thước, màu sắc, chất liệu, phụ kiện, bảo hành; điền đầy đủ thuộc tính.

Mô tả mơ hồ → giảm CVR + tăng đổi trả vì "nhận không giống mô tả".

**Template 6 khối** theo logic người mua đọc:
1. Vấn đề / nhu cầu
2. Sản phẩm giải quyết thế nào
3. Thông số kỹ thuật
4. Ai nên dùng / ai không nên dùng
5. Quy cách / phụ kiện / bảo hành
6. Cam kết giao hàng / đổi lỗi

### 3.5 Ảnh — yêu cầu kỹ thuật

- Tối thiểu **500×500 pixels**, độ phân giải tối thiểu **72dpi**.
- Phải dùng ảnh thật, rõ ràng, độ phân giải cao.
- **Tỉ lệ 3:4** giúp tăng cường hiển thị (test nếu tài khoản đã được hỗ trợ).
- Có công cụ **tối ưu ảnh bằng AI** của Shopee — dùng để tăng tính chuyên nghiệp, KHÔNG bóp méo sản phẩm thật.

### 3.6 Thuộc tính, danh mục — metadata thực sự trên Shopee

Shopee KHÔNG dạy nghĩ theo "backend tags" của website riêng. Metadata quan trọng nhất:
- Danh mục đúng.
- Thuộc tính đúng.
- Thương hiệu đúng.
- Phân loại đúng.
- Hashtag video/live đúng.
- Bộ từ khoá quảng cáo đúng.

Điền đầy đủ thuộc tính → "nâng cao khả năng tìm kiếm và nhận diện". Khi đăng bán phải điền: thương hiệu, chất liệu... để khách hiểu hơn về sản phẩm. Video nên có voucher và hashtag ngành hàng.

**Bẫy lớn**: sai ngành hàng, sai thương hiệu, sai ngôn ngữ, sai đồng nhất thông tin. Shopee có cơ chế **điều tiết lưu lượng** với:
- Tên/mô tả/hình ảnh chứa ngôn ngữ nước ngoài.
- Thông tin gây hiểu lầm.
- Nội dung không nhất quán.

### 3.7 CTR, CVR, review, fulfillment = SEO thật sự

Hiển thị trên Shopee chịu tác động của:
- Hành vi nhấp, bỏ giỏ, mua hàng.
- Độ phổ biến (lượt bán, xếp hạng đánh giá).
- Hiệu suất vận hành (tỷ lệ giao hàng thành công, lựa chọn vận chuyển).

**SEO thật sự = nội dung đúng + giá đúng + review đúng + vận hành đúng.**

Cửa sổ vàng cho review:
- Khách có **15 ngày** để đánh giá sau khi đơn hoàn thành.
- **30 ngày** để chỉnh sửa đánh giá.
→ Shop follow up đúng lúc.

Mục tiêu sau chiến dịch: KHÔNG chỉ thêm đơn — mà **thêm review chất lượng**.

## 4. Dashboard và chỉ số

Không có dashboard = không "điều hành", chỉ "phản ứng".

Dashboard 3 tầng: **traffic / chuyển đổi / lợi nhuận-vận hành**.

### 4.1 Định nghĩa chỉ số chuẩn Shopee Ads

- **ROAS** = GMV / Chi phí.
- **ACOS** = Chi phí / GMV × 100%.
- **CVR trực tiếp** = lượt chuyển đổi trực tiếp / số click.
- **CRR** = tỷ lệ trả lời chat trong 12 giờ.
- **NFR** = tỷ lệ đơn bị hủy/hoàn do lỗi người bán.
- **LSR** cao có thể dẫn tới điểm phạt.

### 4.2 Bảng KPI dashboard hằng ngày

| Nhóm | KPI | Cách hiểu | Tần suất | Ngưỡng cảnh báo |
|---|---|---|---|---|
| Traffic | Impressions, clicks, CTR | Bao nhiêu người nhìn thấy, nhấp vào | Ngày / 2 giờ ngày sale | CTR giảm 20% so với 7 ngày |
| Chuyển đổi | CVR, Add-to-cart rate, Orders | Vào xem rồi có mua không | Ngày / 2 giờ ngày sale | CVR giảm 15% |
| Giá trị đơn | AOV, attach rate | Một đơn trung bình đáng giá bao nhiêu | Ngày | AOV giảm 10% |
| Quảng cáo | ROAS, ACOS, CPC | Quảng cáo lời hay đốt tiền | Ngày / 2 giờ ngày sale | ACOS vượt trần biên lợi nhuận |
| Chất lượng shop | CRR, thời gian phản hồi chat | Trả lời khách có nhanh không | Ngày | CRR yếu, phản hồi chậm |
| Vận hành | NFR, LSR, thời gian chuẩn bị hàng | Hủy/lỗi/giao trễ có tăng không | Ngày/tuần | Chạm ngưỡng phạt |
| Chất lượng SP | Rating, số review mới, tỉ lệ review text/ảnh | Niềm tin tăng hay giảm | Ngày/tuần | Rating giảm, review tiêu cực tăng |
| Lợi nhuận | Contribution margin/order | Mỗi đơn còn lại bao nhiêu tiền thật | Ngày | Âm hoặc gần 0 |

### 4.3 4 biểu đồ nên có

1. **Traffic source mix** — nguồn lưu lượng đến từ đâu.
2. **CTR/CVR theo SKU**.
3. **Waterfall lợi nhuận theo SKU** — biểu đồ quan trọng nhất, trả lời "SKU nào tăng trưởng thật, SKU nào đốt tiền lấy tiếng".
4. **Heatmap rủi ro vận hành** theo ngày/ca.

### 4.4 Sơ đồ dữ liệu (ER diagram)

PTL gốc đề xuất sơ đồ dữ liệu (Mermaid `erDiagram`) để quản lý ở cấp đơn hàng & SKU, không chỉ aggregate. Bám theo các chỉ số Shopee Seller Center và Shopee Ads công bố.

**11 entity và quan hệ chính**:

```
SHOP ||--o{ PRODUCT          (shop sở hữu nhiều product)
PRODUCT ||--o{ SKU           (1 product có nhiều SKU/biến thể)
PRODUCT ||--o{ REVIEW        (1 product nhận nhiều review)
SKU ||--o{ INVENTORY_SNAPSHOT (1 SKU được theo dõi tồn kho theo ngày)
SHOP ||--o{ CAMPAIGN          (shop chạy nhiều campaign)
CAMPAIGN ||--o{ AD_SPEND_DAILY (1 campaign có chi phí ads theo ngày)
SHOP ||--o{ ORDER             (shop nhận nhiều order)
ORDER ||--o{ ORDER_ITEM       (1 order chứa nhiều item)
PRODUCT ||--o{ ORDER_ITEM     (1 product được bán dưới dạng nhiều order item)
SHOP ||--o{ TRAFFIC_DAILY     (shop có traffic theo ngày)
SHOP ||--o{ CHAT_LOG          (shop xử lý nhiều log chat)
ORDER ||--o{ RETURN_CASE      (1 order có thể tạo case hoàn trả)
```

**Trường chính (key fields) của 11 entity**:

| Entity | Trường chính |
|---|---|
| **SHOP** | shop_id, shop_type, segment |
| **PRODUCT** | product_id, category, hero_flag, list_price, campaign_price |
| **SKU** | sku_id, product_id, stock_on_hand, cogs |
| **CAMPAIGN** | campaign_id, campaign_type, start_date, end_date, target_roas |
| **AD_SPEND_DAILY** | campaign_id, date, impressions, clicks, spend, gmv |
| **ORDER** | order_id, shop_id, order_date, order_value, status |
| **ORDER_ITEM** | order_id, product_id, qty, net_sales |
| **REVIEW** | review_id, product_id, rating, review_type, review_date |
| **INVENTORY_SNAPSHOT** | sku_id, snapshot_date, sellable_stock, reserved_stock |
| **TRAFFIC_DAILY** | shop_id, date, source, sessions, add_to_cart |
| **CHAT_LOG** | chat_id, shop_id, date, response_minutes, outcome |
| **RETURN_CASE** | return_id, order_id, reason, seller_fault |

**Mục đích**: tránh chỉ nhìn aggregate (GMV/đơn) — phải có dữ liệu cấp SKU + cấp đơn hàng để tính contribution margin chính xác, biết SKU nào lời/lỗ thật, biết campaign nào đốt tiền.

## 5. Ma trận rủi ro

| Rủi ro | Xác suất | Tác động | Dấu hiệu sớm | Cách giảm thiểu |
|---|---|---|---|---|
| Đối thủ phá giá | Cao | Cao | CTR giữ nhưng CVR tụt | Khoá margin floor, chỉ giảm trên hero SKU, dùng combo thay vì giảm thẳng |
| Phí/policy thay đổi | Trung bình | Cao | Lãi ròng tụt dù đơn tăng | Cập nhật fee sheet theo ngày hiệu lực và loại shop mỗi tháng |
| Tồn kho lệch / hết hàng | Cao | Cao | Nhiều hủy đơn, giao trễ | Đồng bộ tồn kho, stock buffer riêng cho campaign |
| Trang sản phẩm bị hiểu sai / điều tiết traffic | Trung bình | Cao | Impression tụt bất thường | Soát title, mô tả, ngôn ngữ, thuộc tính, danh mục |
| Ads đốt tiền | Cao | Cao | CTR ổn nhưng ACOS tăng | Cắt từ khoá rộng kém chất lượng, dồn ngân sách về query lời |
| Review xấu sau sale | Trung bình | Cao | CVR tụt sau campaign | Kiểm hàng, đóng gói, xin review đúng lúc, xử lý tiêu cực nhanh |
| Vi phạm chat / buff ảo / giá ảo | Thấp–Trung bình | **Rất cao** | Bị cảnh báo, mất hiển thị | Quy trình compliance nội bộ, KHÔNG chơi "mẹo bẩn" |
| Team quá tải ngày sale | Cao | Trung bình–Cao | Chat chậm, giao trễ | Phân ca, war room, SOP theo giờ |

**3 lớp rủi ro cốt lõi**:
- **Rủi ro chính sách**: giá ảo, buff chỉ số ảo, vi phạm chat, yêu cầu khách hủy đơn → có thể bị xoá sản phẩm + tính điểm phạt.
- **Rủi ro vận hành**: NFR, LSR, phản hồi chat, đánh giá shop = tín hiệu trải nghiệm. Chuẩn vàng (**Shop Yêu Thích+** của Shopee làm benchmark): điểm đánh giá ≥4.8, phản hồi chat ≤2 giờ, NFR ≤3%, LSR ≤3%.
- **Rủi ro tài chính**: phí mới cuối T4-đầu T5/2026 + VAT 10% trên phí. Dùng file tính lãi cũ → doanh thu tăng nhưng lợi nhuận thật giảm.

## 6. Kế hoạch 30/60/90 ngày

| Giai đoạn | Mục tiêu | Hằng ngày | Hằng tuần | Đầu ra bắt buộc |
|---|---|---|---|---|
| **30 ngày đầu** | Dựng nền đúng | Kiểm chat, tồn kho, ads, review, hủy đơn, giao trễ | Sửa 20 SKU/tuần; chốt 3-5 hero SKU; dựng file lãi SKU | Bộ title-ảnh-mô tả-thuộc tính chuẩn; dashboard ngày |
| **60 ngày** | Tăng tốc có kiểm soát | Theo dõi war room cho hero SKU; cắt query lỗ | Test 1 biến/tuần/SKU; 1 live/tuần; 1 flash sale/tuần; 1 campaign/đợt | Cụm SKU lời rõ; query map; playbook campaign |
| **90 ngày** | Hệ thống hoá và scale | Giữ nhịp review, CSKH, replenishment | Nhân bản SKU thắng; phân tầng giá; lịch campaign quý | Máy tăng trưởng lặp lại: hero-attach-repeat |

**Checklist hằng ngày 7 dòng**: spend, impressions, CTR, CVR, đơn hoàn/hủy, chat SLA, stock cover.
**Checklist hằng tuần 5 dòng**: bóc query, bóc lãi, bóc review xấu, bóc top SKU, bóc campaign kế tiếp.

## 7. Template & sơ đồ

### 7.1 Mẫu title

Cấu trúc: `[Loại sản phẩm] + [thuộc tính chính] + [công dụng/đối tượng] + [thông số/biến thể] + [thương hiệu]`

Ví dụ minh hoạ trong tài liệu gốc *(ngữ cảnh đồ xăm — anh dịch sang TPCN khi áp dụng)*: "Máy xăm pen không dây lực khoẻ 4.0mm pin rời cho line và shading"

📎 *Em (agent) thêm — gợi ý ví dụ TPCN tương đương*:
- "Viên uống collagen Nhật Bản 1000mg đẹp da chống lão hoá hộp 30 viên [Brand]"
- "Vitamin tổng hợp đa sinh tố cho người lớn tuổi 60+ chai 60 viên hỗ trợ miễn dịch [Brand]"
- "Bột rau xanh hữu cơ detox đường ruột gói 200g cho người ăn kiêng [Brand]"

### 7.2 Mẫu mô tả 6 khối

```
Mở đầu
- Sản phẩm phù hợp với ai, giải quyết vấn đề gì (1-2 câu)

Khối lợi ích
- Độ ổn định
- Công năng chính
- Điểm khác biệt so với bản phổ thông

Khối thông số
- Kích thước
- Chất liệu
- Điện áp / công suất / dung lượng (hoặc liều dùng / hàm lượng cho TPCN)
- Phụ kiện kèm theo

Khối hướng dẫn dùng
- Cách dùng nhanh
- Lưu ý khi dùng
- Ai nên dùng / ai không nên dùng

Khối cam kết
- Kiểm hàng trước khi giao
- Hỗ trợ khi sản phẩm lỗi
- Thời gian xử lý đơn
```

### 7.3 Mẫu voucher

| Loại | Mức gợi ý |
|---|---|
| Voucher kéo đơn | Giảm 15k cho đơn từ 199k |
| Voucher tăng AOV | Giảm 30k cho đơn từ 399k |
| Voucher follower | Theo dõi shop nhận mã 20k |
| Voucher live | Chỉ trong live: giảm 25k cho 30 đơn đầu |

### 7.4 Kịch bản livestream 20 phút

| Phút | Nội dung |
|---|---|
| Phút 1 | 1 vấn đề khách đang gặp + hứa lợi ích rõ + treo voucher live ngay |
| Phút 2-8 | Demo hero SKU: cận cảnh, thông số, tình huống dùng, lỗi thường gặp nếu chọn sai |
| Phút 8-12 | So sánh 2 phiên bản / 2 mức giá / 2 nhu cầu mua |
| Phút 12-16 | Upsell bundle: sản phẩm chính + phụ kiện mua kèm |
| Phút 16-20 | Chốt bằng live price, số lượng còn lại, nhắc voucher, nhắc deadline |

### 7.5 Sơ đồ luồng chiến dịch (flowchart)

```
A[Chọn 3-5 hero SKU]
  → B{Biên đóng góp dương sau mọi chi phí?}
     - Không → A1[Loại SKU khỏi campaign]
     - Có → C[Soát title ảnh mô tả thuộc tính]
            → D{Tồn kho và ca vận hành đủ?}
               - Không → D1[Giảm quy mô hoặc đổi SKU]
               - Có → E[D-14 chạy preheat ads]
                      → F[Bóc query CTR CVR]
                      → G[D-7 chốt voucher combo flash sale live]
                      → H[D-1 khoá tồn kho ngân sách ca trực]
                      → I[D-day war room 2 giờ/lần]
                      → J{SKU nào lời thật?}
                         - SKU lời → K[Tăng ngân sách/bid có kiểm soát]
                         - SKU lỗ → L[Cắt/bóp query giảm ưu đãi]
                      → M[D+1 đến D+7 xin review bóc dữ liệu]
                      → N[Postmortem và nhân bản playbook]
```

## 8. Ba bước làm ngay

1. **Chọn 3-5 hero SKU và tính lại lãi theo từng đơn.** Đúng khi mỗi SKU có file lãi riêng tính đủ giá vốn, phí sàn, phí xử lý giao dịch, VAT trên phí, voucher, ads, đóng gói, dự phòng hoàn/hủy. Sai khi quyết định campaign bằng cảm giác hoặc chỉ nhìn doanh thu.
2. **Sửa 20 SKU quan trọng nhất theo thứ tự**: title → ảnh bìa → thuộc tính → mô tả. Đúng khi title rõ, tiếng Việt có dấu, khớp ảnh; ảnh thật, rõ, đạt chuẩn; thuộc tính điền đủ; mô tả có thông số và use case. Sai khi nhồi từ khoá, ảnh mờ, sai ngành hàng, mô tả hời hợt.
3. **Dựng lịch campaign 14 ngày + dashboard ngày sale.** Đúng khi biết trước D-14 làm gì, ai trực chat, ai trực đơn, ngân sách trần là bao nhiêu, KPI nào xem mỗi 2 giờ, ngưỡng nào tăng ngân sách, ngưỡng nào cắt query. Sai khi đợi tới ngày sale mới bật ads, mới làm voucher, hoặc mới kiểm tra tồn kho.

## 9. Áp dụng vào TPCN — gợi ý từ em (agent)

📎 *Phần này em thêm, không có trong tài liệu gốc.*

| Đặc điểm TPCN | Đòn bẩy Shopee phải dùng |
|---|---|
| **YMYL — claim sức khoẻ bị kiểm soát chặt** | Title + mô tả + ảnh KHÔNG được claim "chữa", "thay thế thuốc". Phải có giấy phép TPCN, công bố sản phẩm, GPP. |
| **Mua dùng thử trước khi mua dài hạn** | Hộp nhỏ / gói combo "starter pack" làm hero traffic SKU; hộp lớn / liệu trình 3-6 tháng làm profit SKU |
| **Khách cần nuôi dưỡng niềm tin lâu** | Review chất lượng (text + ảnh) cực kỳ quan trọng; cần SOP follow-up sau giao hàng để xin review |
| **Hành vi mua lặp lại cao** (TPCN dùng đều) | Repeat SKU = combo 3 hộp / chương trình thành viên / voucher follower; Mã tích luỹ |
| **Ngại tác dụng phụ** | FAQ trong PDP phải có: "Ai không nên dùng", "Có gây tác dụng phụ không", "Có cần kê đơn không" |
| **Giá nhạy cảm với chính sách giảm giá** | Voucher chốt đơn (ngưỡng đơn tối thiểu) tốt hơn giảm thẳng; Combo tốt hơn giảm sâu |

## 🔗 Liên kết

- Quay lại tổng quan [[Khối 18 - Sàn thương mại điện tử]].
- File gốc: `raw/Đặc sản của Phạm Thành Long/IPS - 19 khối công việc/18_ Sàn thương mại ĐT/Shopee.docx`
- Khối liên quan: [[Khối 14 - ADS Các nền tảng]] (so sánh với ads phễu ngoài), [[Khối 17 - Trả lời tin nhắn]] (chỉ số CRR), [[Khối 1 - Hồ sơ khách hàng]] (4 nhóm khách Shopee).

## 📚 Trích dẫn nguồn (theo PTL gốc)

Tài liệu gốc citation từ [1] đến [44]:
- [1][32] banhang.shopee.vn/edu/article/2345 — quản lý sản phẩm
- [2][22] link.springer.com/article/10.1007/s41870-025-02851-z — nghiên cứu live commerce
- [3][6][38][42] banhang.shopee.vn/edu/article/21087 — phí sàn 2026
- [4][7][18][24] ads.shopee.vn/learn/faq/87/1390 — dịch vụ hiển thị Shopee
- [5][10][15][41][44] ads.shopee.vn/news/117 — chuẩn bị mega sale
- [8] ads.shopee.vn/learn/inspiration/208/585 — CTR và yếu tố ảnh hưởng
- [9] banhang.shopee.vn/edu/article/16252 — chỉ tiêu vận hành shop
- [11] cdngarenanow-a.akamaihd.net (PDF tỷ lệ đơn không thành công)
- [12] banhang.shopee.vn/edu/article/26958 — Shopee Xử Lý
- [13] banhang.shopee.vn/edu/article/1844 — đăng ký campaign
- [14] banhang.shopee.vn/edu/article/19319 — voucher shop
- [16] banhang.shopee.vn/edu/article/20503 — LIVE features
- [17] banhang.shopee.vn/edu/article/2242 — Flash Sale Của Shop
- [19][25] ads.shopee.vn/learn/faq/118/610 — từ khoá quảng cáo
- [20] ads.shopee.vn/news/713 — Tối đa Doanh thu
- [21] ads.shopee.vn/learn/faq/398/2041 — kỷ luật optimization
- [23] ads.shopee.vn/learn/inspiration/208/1457 — case study quảng cáo
- [26][40][43] banhang.shopee.vn/edu/article/2100 — title chuẩn
- [27] banhang.shopee.vn/edu/article/2911 — mô tả sản phẩm
- [28] banhang.shopee.vn/edu/article/10587 — kích thước ảnh
- [29] mdpi.com/1999-5903/11/11/224 — nghiên cứu video commerce
- [30] banhang.shopee.vn/edu/article/250 — thuộc tính sản phẩm
- [31] banhang.shopee.vn/edu/article/26757 — sản phẩm bị điều tiết lưu lượng
- [33][34][35][39] ads.shopee.vn/learn/faq/119/634 — theo dõi hiệu quả chiến dịch
- [36] banhang.shopee.vn/edu/article/2310 — chính sách
- [37] banhang.shopee.vn/edu/article/4804 — Shop Yêu Thích+
