---
type: source
tags: [ips, khoi-18, lazada, lazmall, san-tmdt, ptl]
status: active
created: 2026-05-09
updated: 2026-05-09
sources: ["[[raw/Đặc sản của Phạm Thành Long/IPS - 19 khối công việc/18_ Sàn thương mại ĐT/Lazada Seller.docx]]"]
khoi: 18
---

# Khối 18b — Playbook thống trị Lazada Seller và leo Top 1

> **Nguồn**: thầy [[Phạm Thành Long]], khoá [[index|IPS]], file `Lazada Seller.docx` (31KB, 234 đoạn).
> Tài liệu được PTL viết dựa trên Lazada Seller Center, Sponsored Solutions, các tài liệu sale 2025-2026 và nghiên cứu trên dữ liệu marketplace của Lazada.
> Quay lại tổng quan: [[Khối 18 - Sàn thương mại điện tử]].

> ⚠️ **Cảnh báo về ví dụ ngành xăm trong tài liệu**: tài liệu PTL dùng ví dụ "máy xăm pen", "kim cartridge 1207RL", "tattoo supply" trong phần mẫu title/từ khoá vì viết cho ngữ cảnh anh Chương lúc đó. Nội dung **CỐT LÕI** (4 tầng xếp hạng, Sponsored Discovery/Max, ROI Lazada vs Margin ROI, LazMall benchmark, lộ trình 90 ngày) là **kiến thức bán Lazada áp dụng cho mọi ngành**, bao gồm TPCN.

> ⚠️ **Lưu ý quan trọng từ tài liệu gốc**: Lazada **KHÔNG công bố công thức organic ranking đầy đủ**. Phần "organic blueprint" trong báo cáo là **mô hình suy luận có căn cứ** từ Seller Center, Sponsored Solutions và nghiên cứu trên chính dữ liệu Lazada, KHÔNG phải công thức bí mật nội bộ. Trong bộ tài liệu công khai cũng KHÔNG thấy mô tả một trường "backend keyword" phổ quát cho mọi ngành hàng như Amazon.

## 🎯 TL;DR

**Muốn lên Top 1 trên Lazada, BỎ cách nghĩ "SEO title là đủ"**. Phải xếp đúng **4 tầng**:
1. **Tầng index**: title + category + brand + model + attributes + variation.
2. **Tầng CTR**: ảnh 1 + giá + freeship + tag khuyến mãi + rating.
3. **Tầng CVR**: review + FAQ + Lorikeet/A+ content + trust + CSKH.
4. **Tầng momentum**: ads + campaign tạo sales velocity đúng bộ từ khoá tiền mặt.

**Thiếu một tầng → Top 1 chỉ là cú nổ ngắn rồi rơi.**

**3 kết luận chiến lược quan trọng nhất**:
1. **Top 1 phải hiểu theo từ khoá CÓ LÃI**, không phải từ khoá vanity.
2. **ROI trong tài liệu Lazada = Doanh thu / Chi phí quảng cáo** (gần với ROAS hơn lợi nhuận ròng) → nếu KHÔNG đo Margin ROI riêng, rất dễ "lãi doanh số, lỗ tiền".
3. Organic ranking hoàn chỉnh KHÔNG được Lazada công bố công khai → mọi "công thức" đều là mô hình suy luận.

**Bộ công cụ ads Lazada 2026**:
- **Sponsored Discovery** (Tài Trợ Hiển Thị Sản Phẩm): chiếm search + recommendation.
- **Sponsored Max** (Tài Trợ Max): scale bằng AI (Toàn Gian Hàng / Theo Sản Phẩm).
- **Sponsored Display** (Tài Trợ Hiển Thị): CPD/CPM cho nhận diện.
- **Brand Search** (Tài Trợ Tìm Kiếm Thương Hiệu): beta cho seller đủ điều kiện.
- **Affiliate / CPS**: trả phí theo sale.
- **CPAS / Collaborative Ads**: Meta + Google → kéo external traffic.

Cập nhật 2025-2026: báo cáo theo giờ, tab riêng cho Chiến Dịch Tăng Cường, tính năng mới cho Max như **Đẩy Nhanh** (mở biên độ khám phá xuống tối đa 30% thấp hơn ROI mục tiêu), **bảo vệ ROI**, báo cáo chuyển đổi tốt hơn.

## 1. Logic xếp hạng và hệ thống đòn bẩy

### 1.1 4 lớp đòn bẩy

| Tầng | Lazada/nguồn công khai nói gì | Đòn bẩy phải đánh | KPI chính |
|---|---|---|---|
| **Khả năng được tìm thấy** | Điểm nội dung cao tăng hiển thị; thuộc tính đầy đủ giúp dễ tìm hơn | Title, category, brand, model, attributes, variations | Search impressions, Content Score |
| **Khả năng được nhấp** | Hình ảnh, review, giá cạnh tranh, freeship, voucher tác động mạnh đến CTR/CVR | Ảnh 1, giá, freeship, badge, rating, số review | CTR |
| **Khả năng được mua** | CR = đơn hàng / click; nội dung sản phẩm tốt tăng chuyển đổi | PDP, FAQ, review proof, Lorikeet/A+ | CVR, add-to-cart |
| **Độ khoẻ vận hành** | Positive rating, chat response, SOT, cancel, return đều được Seller Center đo | CSKH, tồn kho, SLA xử lý đơn | Positive Seller Rating, 10MRR, SOT |
| **Động lượng bán** | Doanh số trước đó là một phần "chất lượng" của sản phẩm quảng bá | Ads, campaign, bundle, review velocity | Units/day, organic share |

Nghiên cứu ACL 2026 trên dữ liệu marketplace Lazada: chuẩn hoá và làm giàu thuộc tính giúp tăng GMV trong **Search 5,32%** và trong **Recommendation 7,89%** qua A/B testing online → **attributes là một lớp SEO ẩn**. Điền sơ sài → khó giữ vị trí bền, kể cả khi title có vẻ "đúng SEO".

### 1.2 Chuẩn nội bộ nên dùng (cao hơn ngưỡng sàn)

KHÔNG dùng ngưỡng sàn làm tiêu chuẩn chiến thắng. Ví dụ ngưỡng LazMall:
- Phản hồi nhanh: từ **70%** trở lên.
- 10MRR: từ **40%** trở lên.
- Hủy đơn do lỗi nhà bán: từ **4%** trở xuống.
- Trả hàng: từ **3%** trở xuống.

Gói giao nhanh:
- FFR+/N0: từ **90%** trở lên.
- Hủy đơn do lỗi nhà bán: từ **5%** trở xuống.

**Chuẩn nội bộ "Top 1 bền"** (cao hơn rõ rệt):
- Positive Seller Rating > 90%.
- 10MRR > 70%.
- Seller-fault cancel < 2%.
- Stockout giờ = 0 trên hero SKU.

## 2. Chiến thắng chiến dịch và quảng cáo

### 2.1 Bảng so sánh loại chiến dịch/chương trình

| Loại | Vai trò đúng | Dùng khi nào | Sai lầm hay gặp |
|---|---|---|---|
| **Chiến Dịch Tăng Cường** | Khuếch đại hiển thị cho sản phẩm khuyến mãi mùa cao điểm | Mega sale, ngày đôi, hero SKU có offer mạnh | Vào chiến dịch khi PDP yếu hoặc stock mỏng |
| **LazFlash** | Kênh traffic khuyến mại rất mạnh | Hero SKU giá thật sự gắt | Dùng cho SKU biên lợi nhuận quá thấp |
| **Flash Sale Store** | Flash sale do shop chủ động | Muốn kiểm soát nhịp sale, SKU, banner | Chạy quá nhiều SKU một lúc |
| **FreeShip Max** | Giảm rào cản phí ship, tăng conversion | Ngành nhạy cảm phí ship, AOV thấp/trung bình | Dùng đại trà làm rỗng profit |
| **LazCoins** | Booster cho decision | SKU có traffic sẵn nhưng CVR chưa đủ | Đồng tài trợ sai SKU |
| **Combo linh hoạt** | Tăng AOV | Có nhiều SKU bổ trợ logic | Bundle vô nghĩa, không tăng attach rate |
| **Sponsored Discovery** | Search + recommendation performance | Luôn-on cho bộ từ khoá tiền mặt | Trộn SKU mới và SKU trưởng thành |
| **Sponsored Max** | Scale bằng AI trên nội sàn | Khi đã có dữ liệu hoặc muốn phủ storewide | Đặt ROI mục tiêu quá cao |
| **Affiliate / CPS** | Mở rộng sale theo kết quả | Kỳ sale, SKU dễ review/viral | Hoa hồng quá thấp, không kéo được publisher |

### 2.2 Nguyên tắc campaign

**Campaign chỉ khuếch đại thứ ĐÃ bán được**. Nếu hero SKU chưa có CTR, review, stock và offer tốt, campaign chỉ phóng đại lỗi.

Tài liệu Mega Lazada nhấn mạnh: phải đảm bảo đủ **ngân sách/ngân quỹ quảng cáo xuyên suốt chiến dịch**. Từ 2025-2026, Chiến Dịch Tăng Cường cho phép **tham gia nhiều campaign cùng lúc** và có **tab riêng để quản lý**.

### 2.3 Chiến thuật từng bước

1. Chia SKU thành 3 nhóm: **hero cash, hero traffic, tail profit**.
2. Lập lịch 3 nhịp: **làm nóng 14-21 ngày**, **khoá offer 3-7 ngày**, **điều chỉnh theo giờ trong ngày sale**. Báo cáo theo giờ dạng tích luỹ từ 2026 rất hữu ích.
3. Voucher theo vai trò: kéo click / tăng AOV / cứu rating. KHÔNG phát voucher toàn shop "trải thảm".
4. **FreeShip Max** chỉ gắn cho SKU có tiềm năng CVR.
5. **LazFlash** dùng cho ít SKU nhưng offer phải vượt trội; **Flash Sale Store** dùng khi shop cần chủ động kịch bản.
6. **Combo linh hoạt** chỉ có ý nghĩa nếu kéo được AOV và attach rate; không tăng AOV → bundle chỉ làm listing rối.

**KPI campaign**: GMV uplift, contribution margin sau khuyến mãi, voucher redemption rate, AOV uplift, stockout hours, seller-fault cancel rate.

**Template Campaign War Room**:
```
SKU | Giá gốc | Giá sale | Voucher | Freeship subsidy | Stock cover | CTR | CVR | Margin/order | Go/No-Go
```

**Offer Stack Map**: phân tầng offer cho Hero / Traffic / Tail.

### 2.4 Bẫy & cách sửa (campaign)

- Vào campaign với **30-50 SKU**: SAI, traffic loãng → chỉ đánh **5-20 hero SKU thật sự**.
- Voucher đồng loạt toàn shop: SAI, margin tốt gánh margin xấu → voucher theo cụm SKU/ngành hàng.
- Tăng ads mà không tăng stock + CSKH: SAI, top lên rồi rơi → phê duyệt ads-stock-service như **một gói**.

### 2.5 Checklist ưu tiên (campaign)

- **P0**: Hero SKU có review, stock cover **tối thiểu 21 ngày**, không warning nội dung.
- **P0**: Margin sau khuyến mãi còn dương.
- **P1**: Ví quảng cáo đủ cho cả kỳ sale.
- **P1**: FreeShip Max/voucher chỉ gắn cho SKU có khả năng chốt đơn.
- **P2**: Có bundle hỗ trợ hero traffic SKU.

### 2.6 Sponsored Discovery & Keyword Conquest

**Nguyên tắc**: Auto để đào dữ liệu; Manual để chinh phục vị trí; Boost để khuếch đại trong mùa sale.

**Sự thật phải nắm**:
- Sản phẩm quảng bá có thể xuất hiện trong **kết quả tìm kiếm, đề xuất trang chủ và trang chi tiết**.
- 4 loại campaign: tự động, quảng bá sản phẩm mới, Chiến Dịch Tăng Cường, thủ công.
- **Ngân sách ngày**: nên đủ cho **tối thiểu 100 click/campaign**.
- **Quảng bá sản phẩm mới/testing**: 30 ngày để chạy tối đa hiệu quả; nếu cần test nhanh có thể 7 ngày.
- **Manual keyword selection**: phù hợp seller muốn sản phẩm lên vị trí đầu ở từ khoá cụ thể.
- **Tối đa 100 sản phẩm/campaign**, nên chia theo ngành hàng trọng tâm.
- **Audience bid boost**: mức khởi điểm gợi ý **+15%**.
- Tài Trợ Hiển Thị Sản Phẩm KHÔNG dùng được nếu **NCP từ 12 trở lên**.

### 2.7 Chiến thuật từng bước (Sponsored Discovery)

1. Tạo **4 lớp campaign** cho mỗi cụm keyword tiền mặt: **Auto Mining, Manual Exact, New Product/NPL, Boost/Mega**.
2. Cho auto chạy **7-14 ngày** để khai thác search terms; KHÔNG mở manual rộng ngay từ đầu.
3. Chuyển **5-10 keyword thắng** sang manual exact để đánh vị trí.
4. Bật **FSS** (Search First Slot) **chỉ cho keyword đã chứng minh có lãi**.
5. Tách SKU theo maturity: mới / hero / phòng thủ. Đừng nhét tất vào một campaign.
6. Chọn SKU quảng bá theo logic Lazada: tìm nhiều, xu hướng, bán chạy, đánh giá cao; có giá cạnh tranh, freeship, voucher → khả năng chuyển đổi tốt hơn.

**KPI**: CTR, CVR, CPC, **ROI theo Lazada**, **Margin ROI nội bộ**, top-slot efficiency, spend/order theo keyword.

**Template Keyword Bank**:
```
Keyword | Intent | Hero SKU | CTR | CVR | CPC | Rank target | Decision
```

**Bid Ladder**: bid bảo vệ / bid khai thác / bid test.

### 2.8 Bẫy Sponsored Discovery

- Manual quá rộng từ ngày 1: SAI, không có data → auto trước, manual sau.
- Trộn SKU mới + SKU trưởng thành: SAI, thuật toán tối ưu lẫn lộn → tách campaign.
- Chỉnh bid mỗi ngày khi campaign mới chạy: SAI, chưa đủ dữ liệu → khung đánh giá cố định **3-7 ngày**.

### 2.9 Bảng so sánh định dạng quảng cáo

| Định dạng | Mục tiêu tốt nhất | Cách tính giá thầu | Khi nên dùng |
|---|---|---|---|
| **Tài Trợ Hiển Thị Sản Phẩm** (Discovery) | Search + recommendation performance | CPC | Chiếm bộ từ khoá tiền mặt |
| **Tài Trợ Max - Toàn Gian Hàng** | Scale phủ toàn shop bằng AI | ROI target / Max CPC / Auto bid | Shop nhiều SKU, cần phủ rộng |
| **Tài Trợ Max - Theo Sản Phẩm** | Scale nhóm hero SKU | ROI target / Max CPC / Auto bid | Muốn kiểm soát nhóm sản phẩm chặt |
| **Tài Trợ Hiển Thị** | Nhận diện thương hiệu / reach | CPD, CPM GD, CPM Bidding | Launch brand, phủ banner |
| **Tài Trợ Tìm Kiếm Thương Hiệu** | Bảo vệ branded search | Beta/eligible sellers | Shop có traffic thương hiệu rõ |
| **Affiliate** | Sale theo kết quả | CPS (gần CPA) | SKU dễ review, sale dates |
| **CPAS / Collaborative Ads** | External high-intent + remarketing | Theo external setup | Hero PDP đã chứng minh CVR |

### 2.10 Tài Trợ Max — cách dùng đúng

1. SKU có **≥5 đơn trong 7 ngày** → ưu tiên bid theo **Mục tiêu ROI**; chưa đủ data → dùng **Max CPC** hoặc **Auto bid**.
2. Ít thời gian → dùng **Toàn Gian Hàng**. Muốn kiểm soát sâu → dùng **Theo Sản Phẩm**.
3. Cho máy học **7 ngày đầu**; KHÔNG chỉnh sửa sớm. Sửa quá sớm có thể đẩy chiến dịch quay lại learning phase.
4. Duy trì ngân sách ổn định. Từ 2026, Max có thêm **Đẩy Nhanh** (mở biên độ khám phá xuống tối đa 30% thấp hơn ROI mục tiêu để tăng traffic nhanh hơn), **bảo vệ ROI**, báo cáo chuyển đổi tốt hơn.
5. **Một sản phẩm KHÔNG thể đồng thời** được quảng bá trong Discovery và Max - Toàn Gian Hàng. Nếu cùng đủ điều kiện ở Max toàn gian hàng và Max theo sản phẩm → hệ thống ưu tiên **Max theo sản phẩm**.

### 2.11 Case study Adidas

Adidas tại Việt Nam dùng Max **chọn các SKU AOV cao nhưng đang ít được nhìn thấy**, đặc biệt nhóm dưới 100 lượt xem. Kết quả: **ROI tăng 3 lần**, **đơn hàng tăng 8%**.

**Bài học**: tư duy "không chỉ nuôi sản phẩm đang mạnh, mà khai phá sản phẩm có lợi nhuận cao nhưng chưa đủ hiển thị".

### 2.12 Affiliate, CPAS, Display — khi nào dùng

- **Affiliate/CPS**: SKU dễ review, dễ demo, dễ "viral", có hoa hồng đủ hấp dẫn. Phí trả khi đơn được ghi nhận theo logic **click-attributed trong 48 giờ**.
- **CPAS/Google**: chỉ chạy khi PDP đã mạnh và review đủ. PDP yếu → external traffic là cách đốt tiền nhanh nhất.
- **Display/CPM**: chỉ đáng dùng khi bài toán là **reach/brand**, không phải chốt đơn ngay trong ngày đầu.

### 2.13 Checklist ưu tiên (ads tổng)

- **P0**: Max dùng đúng loại bid theo maturity SKU.
- **P0**: KHÔNG sửa campaign trong **7 ngày đầu** trừ lỗi cực lớn.
- **P1**: External traffic chỉ đổ vào top PDP đã chứng minh CVR.
- **P1**: Affiliate có hoa hồng đủ hút publisher.
- **P2**: Display chỉ bật khi đã có story thương hiệu và budget nhận diện.

## 3. SEO sản phẩm để lên Top 1

### 3.1 Keyword research

**Nguyên tắc**: KHÔNG săn từ khoá volume to nhất; săn cụm từ khoá **mua hàng rõ nhất**.

Lazada có hệ đề xuất từ khoá trong Sponsored Discovery; tài liệu quảng cáo nói rõ **keyword relevance rất quan trọng cho CTR, CR và CPC**.

**Chiến thuật từng bước**:
1. Lấy keyword từ **5 nguồn**: gợi ý tìm kiếm, đề xuất trong ads, báo cáo auto, title top đối thủ, chat/review khách.
2. Chia thành **5 nhóm**: exact buying, attribute, use-case, problem-solution, brand-defense.
3. Quy tắc **70/20/10**: 70% budget cho keyword tiền mặt, 20% cho long-tail có lãi, 10% cho test.
4. Mỗi hero SKU chỉ nên có **1-2 keyword chính**. Muốn Top 1 bền → dồn tín hiệu rõ vào **một intent rõ**.

**KPI**: search impressions, CTR, CVR, CPC, organic units/day sau giai đoạn ads làm nóng.

**Template**:
```
Keyword | Intent | Hero SKU | Price promise | Image angle | CTR | CVR | Rank target
```

**Bẫy**: 1 keyword gắn cho quá nhiều SKU, hoặc chỉ đánh head-term rộng. **Sửa**: 1 keyword chủ lực = 1 hero SKU chủ lực.

### 3.2 Title, backend keyword và thuộc tính

**Nguyên tắc**: tiêu đề phải **thẳng, đúng sự thật, chỉ chứa keyword liên quan**; điền đầy đủ thuộc tính để tăng searchable. Optional attributes tăng khả năng được tìm thấy.

**Quan trọng**: Lazada KHÔNG có trường "backend keyword" phổ quát như Amazon. Backend layer thực tế trên Lazada hiểu là:
```
category + brand + model + attributes + variation names
+ description/Lorikeet + dữ liệu từ khoá quảng cáo
```

Nếu ngành hàng/tài khoản có ô từ khoá bổ sung → dùng nó như **lớp phụ**, KHÔNG thay cho title/attributes.

**Công thức title**:
```
[Brand] + [Loại sản phẩm] + [Model/Dòng] + [thuộc tính mua hàng mạnh nhất] + [quy cách/biến thể]
```

**Quy tắc**:
1. Đặt **keyword chính ở đầu title**.
2. KHÔNG nhồi từ và KHÔNG chèn "sale, số 1, rẻ nhất" vào title.
3. Điền đủ thuộc tính bán hàng thật sự khách dùng để tìm: model, thông số, tương thích, quy cách.
4. Đặt tên biến thể theo ngôn ngữ người mua thực sự gõ, KHÔNG đặt kiểu nội bộ.

### 3.3 Ví dụ title (từ tài liệu gốc)

⚠️ *Tài liệu gốc dùng ngữ cảnh "tattoo supply" — em giữ nguyên cho độ phủ, nhưng anh dịch sang TPCN khi áp dụng.*

| Loại ví dụ | Mẫu |
|---|---|
| **Title kém** | `HOT SALE Máy xăm siêu xịn giá rẻ số 1 tattoo pen cực mạnh` |
| **Title tốt** | `[Thương hiệu] Máy xăm pen không dây stroke 3.5mm pin 1520mAh máy xăm line shading` |
| **Title tốt cho consumable** | `[Thương hiệu] Kim cartridge 1207RL kim xăm tiệt trùng dùng cho máy pen hộp 20 cái` |

**Ví dụ backend keyword nếu có ô bổ sung** *(theo ngữ cảnh tattoo trong tài liệu)*:
```
may xam pen, may xam khong day, tattoo pen wireless,
may xam line, may xam shading, stroke 3.5mm,
pin 1520mah, may xam cho tho xam
```

📎 *Em (agent) thêm — gợi ý title TPCN tương đương*:
- Title kém: `HOT SALE viên uống collagen siêu xịn giá rẻ số 1 đẹp da chống lão hoá`
- Title tốt: `[Brand TPCN] Viên uống collagen Nhật Bản 1000mg hộp 30 viên đẹp da chống lão hoá`
- Title cho consumable refill: `[Brand TPCN] Bột collagen peptide 5000mg gói 30 sachet bổ sung collagen hằng ngày`

**KPI**: Content Score, mức hoàn tất attributes, search impressions trước/sau chỉnh title, CTR trước/sau đổi title.

### 3.4 Ảnh, bullet points, Lorikeet/A+ và store branding

Yêu cầu Lazada:
- Hình ảnh phải tập trung vào sản phẩm, **không dùng before/after**, không hình không liên quan, không hiệu ứng gây hiểu sai.
- Có **Lorikeet/A+ content** để tạo nội dung sản phẩm hấp dẫn.
- Store decoration mới có **review gallery, promotion page, store search**.
- Logo: nền trắng hình vuông tối thiểu **300x300**, tối đa **400x400**; có guideline kích thước ảnh mẫu cho thương hiệu.

**Chiến thuật ảnh**:
1. **Ảnh 1 chỉ làm một việc**: tăng CTR.
2. Ảnh 2-3 chốt tính năng và bằng chứng mua hàng mạnh nhất.
3. Ảnh 4-5 chốt specs/tương thích/what's in box.
4. Ảnh 6-8 chốt FAQ, so sánh, review proof, bảo hành/chính sách.
5. Lorikeet/A+ dùng để **xử lý phản đối mua hàng**, KHÔNG để viết brochure dài dòng.
6. Brand asset phải đồng nhất.

**Checklist ảnh**:
- **P0**: Ảnh 1 khác trực diện cụm đối thủ.
- **P0**: PDP có proof + compatibility + what's in box.
- **P1**: Lorikeet có FAQ và review proof.
- **P2**: Store có review gallery + promotion page + store search.

### 3.5 CTR, CVR, sales velocity và organic momentum

**Nguyên tắc**: KHÔNG có sales velocity thì KHÔNG có Top 1 bền. Lazada nêu rằng "chất lượng sản phẩm quảng bá" có chứa: doanh số trước đó, review tích cực, hình ảnh.

**Chiến thuật**:
1. Tạo **"đụn doanh số" cho hero SKU** thay vì dàn đều sang nhiều SKU.
2. Mỗi keyword chính phải có **một offer stack riêng**: ảnh đúng intent + giá đúng tâm lý + freeship + voucher + review.
3. Chạy ads **2-4 tuần làm nóng**; khi organic share tăng → giảm spend từ từ, KHÔNG tắt đột ngột.
4. **Cây quyết định**:
   - CTR thấp → sửa ảnh/title.
   - CTR tốt nhưng CVR thấp → sửa PDP/offer/review.
   - CTR và CVR tốt nhưng volume thấp → tăng bid/budget/campaign pressure.

**KPI**: CTR theo keyword, CVR PDP, units/day trên hero SKU, review velocity, organic share sau **14-28 ngày**.

## 4. Giá, kho, vận hành, reviews, thương hiệu, cross-border

### 4.1 Bảng so sánh chiến lược giá

| Chiến lược | Khi dùng | Ưu điểm | Rủi ro | KPI |
|---|---|---|---|---|
| **EDLP** (Everyday Low Price) | SKU chuẩn hoá, cạnh tranh cao | CVR ổn định | Khó tạo đột biến | CTR, CVR, margin/order |
| **High-Low theo kỳ sale** | Có lịch sale rõ | Tận dụng peak traffic | Khách bị "dạy" chờ sale | GMV uplift, margin kỳ sale |
| **Hero loss leader** | Cần kéo khách vào gian | Kéo top nhanh | Không có upsell là lỗ | NCO (new-customer orders), attach rate |
| **Bundle/combo** | Có SKU bổ trợ | Tăng AOV, tăng profit tuyệt đối | Bundle vô nghĩa thì không ai mua | AOV, attach rate |
| **Variant ladder** | Có bản premium rõ | Kéo người mua lên cấu hình lợi nhuận cao | Cấu trúc biến thể rối giảm CVR | Mix bản bán, contribution/order |

### 4.2 Công thức quản trị tối thiểu

```
Contribution/order = Doanh thu thuần – giá vốn – phí sàn
                     – voucher/freeship subsidy – đóng gói – dự phòng hoàn trả

CPC trần       = Contribution/order × CVR

Voucher trần   = Contribution/order – lợi nhuận mục tiêu
```

**Kết luận**: KHÔNG khoá giá trước khi có P&L. Seller Center có công cụ **dự tính phí** — dùng nó như bước **bắt buộc** trước khi vào campaign.

### 4.3 Kho, logistics, SLA vận hành

- Đa số campaign yêu cầu giao hàng **đúng hạn**.
- Đơn tiêu chuẩn có thể bị hủy nếu KHÔNG đáp ứng cam kết trong **3 ngày**.
- Chương trình giao nhanh: **FFR+/N0 ≥90%**, **seller-fault cancellation ≤5%**.
- 3 cách xử lý đơn: tự xử lý, seller linked shipping, **FBL** (Fulfilled by Lazada).

**Chiến thuật**:
1. Forecast tồn kho theo 3 lớp: **base demand + campaign uplift + return/defect buffer**.
2. **Rule ads theo stock cover**:
   - **>21 ngày** → mới scale.
   - **14-21 ngày** → chỉ giữ keyword chính.
   - **<14 ngày** → ngừng ép top.
3. Theo dõi ở **cấp biến thể**, không chỉ cấp SKU tổng.
4. Chọn mô hình fulfillment dựa trên khả năng giữ SOT, không chỉ chi phí đơn lẻ.

**KPI**: stock cover days, stockout hours, SOT (Speed of Trade), seller-fault cancel, order aging.

### 4.4 CSKH, review, seller rating, fulfillment metrics

- **Positive seller rating > 80%** → Lazada ưu tiên cho ưu đãi riêng.
- **10MRR** = phản hồi trong 10 phút trong khung **8:00-23:00**.
- **LazMall ngưỡng**: phản hồi nhanh ≥70%, 10MRR ≥40%, hủy đơn ≤4%, trả hàng ≤3%.
- Lazada có chương trình **khuyến khích review cho sản phẩm ít đánh giá**, đồng thời **cấm spam khách**.

**Chiến thuật**:
1. SKU mới: dùng **cơ chế review của nền tảng**, KHÔNG xin review phản cảm ngoài luồng.
2. Hero SKU: SOP hậu mãi trong **3 ngày đầu sau giao hàng**.
3. Ticket/chat: ack trong **10 phút**, chẩn đoán trong **1 giờ**, chốt giải pháp trong **24 giờ**.
4. Dùng chuẩn LazMall làm **chuẩn vàng nội bộ**, kể cả chưa vào LazMall.
5. Theo dõi **review velocity**, không chỉ tổng review.

**KPI**: Positive Seller Rating, 10MRR, rating sản phẩm, review velocity, return rate, resolution time.

### 4.5 Store branding & cross-border

Store decoration mới: **review gallery, promotion page, tìm kiếm trong shop** → tăng dwell time, cross-sell.

Lazada hoạt động trên **6 thị trường Đông Nam Á**, có logistics đầu-cuối, năng lực cross-border/last-mile.

**3 lựa chọn**:
- **Local-first**: nhanh nhất để chốt Top 1.
- **Regional expansion**: chỉ mở khi core market đã ổn **60-90 ngày**.
- **Imported assortment**: phù hợp nếu có nguồn hàng khác biệt + lead time chắc.

→ Nếu mục tiêu hiện tại là Top 1 nội địa, cross-border chỉ là **pha hai** sau khi nội địa đã ổn review, stock, warranty, seller health.

## 5. KPI, công cụ, template, screenshot

### 5.1 KPI dashboard tối thiểu

| Nhóm | KPI | Chu kỳ theo dõi |
|---|---|---|
| Index | Content Score, attribute completion, search impressions | Ngày/tuần |
| Click | CTR theo SKU, CTR theo keyword | Ngày |
| Chuyển đổi | CVR, add-to-cart, AOV | Ngày |
| Ads | CPC, **ROI Lazada**, **Margin ROI**, spend/day | Ngày/giờ trong Mega |
| Reviews | Rating, review count, review velocity | Tuần |
| Vận hành | Positive Seller Rating, 10MRR, SOT, cancel, return | Ngày |
| Tồn kho | Stock cover, stockout hours | Ngày |
| Organic lift | Organic units/day, organic share sau ads | Tuần |

### 5.2 Template nên triển khai ngay

**Keyword map**:
```
Keyword | Intent | Hero SKU | CTR | CVR | CPC | Rank target | Decision
```

**P&L campaign**:
```
SKU | Price | Voucher subsidy | Freeship subsidy | Platform fee | COGS
| Return reserve | Contribution/order | CPC trần | Go/No-Go
```

**Hero SKU audit**:
```
SKU | Content Score | Review count | Rating | Stock cover
| Title ready | Images ready | Ads ready | Campaign ready
```

### 5.3 4 chart/diagram nên có trong báo cáo nội bộ

1. **Keyword quadrant**: X = CTR, Y = CVR, bubble = spend.
2. **Profit waterfall**: Price → promo → fees → ads → contribution.
3. **Daily units vs organic share**.
4. **Stock cover heatmap** theo biến thể.
5. **Review velocity chart**.

### 5.4 Screenshot nên chèn (báo cáo nội bộ)

- Seller Center → Quản lý sản phẩm → Điểm nội dung / tối ưu listing.
- Sponsored Discovery → Báo cáo từ khoá.
- FSS / Audience reporting.
- Tài Trợ Max → learning / ROI protection / conversion report.
- Seller metrics dashboard: positive rating, 10MRR, SOT, cancel.
- Store decoration: review gallery, promotion page, store search.

## 6. Lộ trình 90 ngày từ launch đến Top 1

Mục tiêu 90 ngày đầu KHÔNG phải "phủ cả ngành" — mà là **chiếm dứt điểm một đầu cầu lợi nhuận**, rồi dùng dữ liệu từ đó mở rộng. Bám logic Lazada về learning phase, lựa chọn loại bid, discovery mining, Boost Campaign, báo cáo theo giờ.

### 6.1 Gantt 90 ngày

```
Section Nền móng (Ngày 1-21)
- Audit SKU và P&L (D1-D7)
- Sửa title, attributes, variations (D8-D17)
- Làm ảnh, PDP, Lorikeet, review flow (D8-D21)

Section Đào dữ liệu (Ngày 12-32)
- Chạy Discovery Auto (D12-D25)
- Thu keyword thắng và loại keyword lỗ (D26-D32)

Section Đánh chiếm (Ngày 26-66)
- Mở Discovery Manual exact (D26-D46)
- Bật FSS cho keyword có lãi (D47-D56)
- Mở Max Store hoặc Product (D29-D49)

Section Khuếch đại (Ngày 41-65)
- Gắn freeship, voucher, combo (D41-D50)
- Vào Flash/Boost/Mega phù hợp (D51-D64)
- Mở affiliate hoặc external có chọn (D51-D64)

Section Củng cố (Ngày 66-90)
- Tăng organic share, giảm spend dần (D66-D79)
- Mở rộng thêm keyword cluster số 2 (D80-D90)
```

### 6.2 Mốc kiểm soát theo giai đoạn

**Ngày 1-14**:
- Xong audit P&L.
- Xong title, attributes, ảnh 1, PDP, review flow.
- Content Score hero SKU đạt mức cao nội bộ, không còn cảnh báo lớn.

**Ngày 15-30**:
- Auto campaign chạy đủ để có data.
- Chốt được keyword thắng/thua.
- Có **5-10 keyword tiền mặt đầu tiên**.

**Ngày 31-60**:
- Manual exact chạy cho keyword tiền mặt.
- Bắt đầu có organic lift ở một phần keyword.
- Max được mở đúng loại bid theo maturity.

**Ngày 61-90**:
- Vào campaign/Boost/Flash có chọn lọc.
- Hero SKU giữ được stock, rating, seller health trong khi scale.
- Bắt đầu mở **keyword cluster thứ hai**, KHÔNG bỏ cluster thứ nhất.

### 6.3 Ba bước làm ngay (72 giờ đầu)

| Bước | Việc trong 72h | Tiêu chí đúng | Dấu hiệu sai |
|---|---|---|---|
| **Bước đầu** | Chọn 5-10 hero SKU và 10 keyword tiền mặt | Mỗi keyword có 1 hero SKU chính | 1 keyword gắn cho 4-5 SKU |
| **Bước kế** | Audit lại title, attributes, ảnh 1, PDP, review proof | Hero SKU không còn lỗ hổng thông tin | Khách vẫn phải chat hỏi thông số cơ bản |
| **Bước cuối** | Mở cấu trúc ads: Auto Mining + Manual Exact + Max | Có phân tầng rõ chiến dịch và KPI | Một campaign ôm tất cả SKU |

## 7. Áp dụng vào TPCN — gợi ý từ em (agent)

📎 *Phần này em thêm, không có trong tài liệu gốc.*

| Đặc điểm Lazada × TPCN | Đòn bẩy nên dùng |
|---|---|
| **LazMall = niềm tin + brand cao cấp** | TPCN chính hãng nên đầu tư vào LazMall — niềm tin shop chính hãng cực quan trọng với health & wellness |
| **Khách Lazada thường so sánh kỹ + đọc review nhiều hơn Shopee** | Lorikeet/A+ content phải có FAQ chi tiết: liều dùng, đối tượng, tác dụng phụ, có cần kê đơn không |
| **Cross-border tiềm năng cho TPCN nhập khẩu** | Có nguồn nhập từ Nhật/Hàn/Mỹ → cân nhắc Lazada cross-border ở pha 2 |
| **ROI Lazada = doanh thu/chi phí ads → Margin ROI là phải tính riêng** | TPCN biên cao nhưng phí sàn + voucher + freeship cao → tính Margin ROI riêng cho mỗi keyword |
| **Discovery Auto rất phù hợp cho TPCN** | Khách TPCN tìm theo nhu cầu (đẹp da, ngủ ngon, giảm cân...) thay vì tên brand → Auto đào ra long-tail intent rất tốt |

## 🔗 Liên kết

- Quay lại tổng quan [[Khối 18 - Sàn thương mại điện tử]].
- File gốc: `raw/Đặc sản của Phạm Thành Long/IPS - 19 khối công việc/18_ Sàn thương mại ĐT/Lazada Seller.docx`
- Khối liên quan: [[Khối 18a - Shopee]] (so sánh với Shopee), [[Khối 14 - ADS Các nền tảng]] (CPAS/Google).

## 📚 Trích dẫn nguồn (theo PTL gốc)

Tài liệu gốc citation từ [1] đến [46]:
- [1][2][5][7] sellercenter.lazada.vn quản lý sản phẩm — điểm nội dung & thuộc tính
- [3] lazadasolutions.com Chiến Dịch Tăng Cường tab riêng (T4/2026)
- [4][18][23][32] Sponsored Discovery Archives
- [6][29] arxiv.org/abs/2604.16950 — AutoPKG nghiên cứu attribute knowledge graph
- [8] sellercenter.lazada.vn — tiêu chuẩn LazMall
- [9][12][13] sellercenter.lazada.vn Help Center
- [10] lazadasolutions 11.11 Mega Sales (T11/2025)
- [11][42] lazadasolutions cập nhật báo cáo dữ liệu (T2/2026)
- [14] sellercenter.lazada.vn Combo linh hoạt
- [15] lazadasolutions Sponsored Discovery overview
- [16][20][28] Sponsored Discovery Archives trang 6
- [17][19] Sponsored Discovery Archives trang 5
- [21] lazadasolutions Sponsored Display fee models
- [22][36] lazadasolutions yếu tố quyết định thứ hạng
- [24] lazadasolutions Sponsored Affiliate
- [25][26][46] lazadasolutions Sponsored Max getting-started
- [27] lazadasolutions Sponsored Max upgrade highlights
- [30] lazadasolutions Adidas case study
- [31] sellercenter.lazada.vn Affiliate cookie 48h
- [33][40] sellercenter.lazada.co.th Inappropriate Content Policy
- [34] sellercenter.lazada.vn chính sách nội dung sản phẩm
- [35] sellercenter.lazada.vn Brand interface guideline
- [37] sellercenter.lazada.vn Công cụ ước tính chi phí
- [38] sellercenter.lazada.vn SOT SLA
- [39] sellercenter.lazada.vn Chính sách mới NBH
- [41][45] sellercenter.lazada.vn Hướng dẫn trang trí gian hàng
- [43] lazadasolutions Sponsored Max ROI Protection
- [44] sellercenter.lazada.vn Bảng tổng hợp chỉ số NBH
