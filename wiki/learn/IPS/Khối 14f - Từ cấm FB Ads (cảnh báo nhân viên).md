---
type: source
tags: [ips, khoi-14, ads, facebook, tu-cam, compliance, ymyl, tpcn, ptl]
created: 2026-05-09
updated: 2026-05-09
sources: ["[[raw/Đặc sản của Phạm Thành Long/IPS - 19 khối công việc/14_ ADS Các nền tảng/📌 Tổng hợp những từ bị CẤM khi chạy Quảng cáo Facebook và bí thuật setup hàng VPCS.docx]]"]
khoi: 14
---

# Khối 14f — Từ cấm FB Ads — Checklist tránh cho nhân viên

> ⚠️ **MỤC ĐÍCH FILE NÀY**: Đây là **CHECKLIST TỪ TRÁNH** cho team viết quảng cáo TPCN — KHÔNG phải hướng dẫn lách luật.
>
> Anh Chương đã chốt **chiến lược white-hat đúng luật**. File này dùng để:
> 1. Team biết những từ nào FB sẽ flag → tránh dùng → bài duyệt nhanh hơn.
> 2. Team biết tại sao TPCN khó hơn ngành thường (chính cụm "Thực phẩm chức năng" đã nằm trong từ cấm).
> 3. Cảnh báo các kỹ thuật **VPCS** (vi phạm chính sách) mà tài liệu gốc PTL có nhắc — để team **KHÔNG ĐƯỢC DÙNG**.

## 🚨 CẢNH BÁO 3 LỚP — ĐỌC TRƯỚC KHI ÁP DỤNG

### Lớp 1 — Tài liệu gốc có thể lỗi thời

- File gốc **KHÔNG có ngày tháng** — không biết viết khi nào.
- FB Ads Policy **đổi 3-6 tháng/lần**. Nhiều "từ cấm" có thể đã được FB thay bằng tiêu chí ngữ cảnh (ML đọc cả câu chứ không match keyword).
- → **Coi list này là tham khảo, không phải checklist tuyệt đối**. Hàng tháng team phải tra **Meta Advertising Standards** mới nhất.

### Lớp 2 — Rủi ro pháp lý Việt Nam (KHÔNG có trong tài liệu gốc — em thêm)

> 📎 Phần này **em (agent) thêm** từ kiến thức pháp lý chung — không có trong tài liệu PTL gốc. Anh nên tư vấn luật sư xác minh.

3 luồng pháp lý động chạm khi quảng cáo TPCN ở Việt Nam:

1. **Luật Quảng cáo 16/2012/QH13 + Nghị định 38/2021/NĐ-CP**:
   - Cấm quảng cáo TPCN gây hiểu nhầm là thuốc chữa bệnh.
   - Bắt buộc có dòng: **"Sản phẩm này không phải là thuốc, không có tác dụng thay thế thuốc chữa bệnh."**
   - Bắt buộc xác nhận **nội dung quảng cáo bởi Cục An toàn thực phẩm/Bộ Y tế TRƯỚC khi chạy**.
   - Vi phạm → **phạt 60-80 triệu/lần + thu hồi giấy công bố**.

2. **Luật ATVSTP 55/2010/QH12 + Nghị định 15/2018/NĐ-CP**:
   - TPCN bắt buộc **công bố sản phẩm trước khi lưu thông + quảng cáo**.

3. **Nghị định 147/2024/NĐ-CP** (hiệu lực 25/12/2024):
   - Tài khoản MXH bắt buộc **xác thực số điện thoại VN/định danh**.
   - Chạy ads bằng **acc clone/via** = vi phạm trực tiếp, có thể bị xử phạt hành chính + khoá tài khoản đại trà.

**Nguyên tắc vàng**: **Né được FB không có nghĩa là né được luật VN.**

### Lớp 3 — Rủi ro thương hiệu dài hạn

Anh đặt mục tiêu **20 tỷ/tháng / 24 tháng** từ con số 0. Né luật ngắn hạn đẩy được 1 tỷ/tháng nhưng:

- Tài khoản BM bị burn → mất hết learning của Pixel, làm lại từ đầu.
- TPCN cần **uy tín dài hạn** (KH mua lại, giới thiệu) — nội dung sai sự thật giết retention.
- Bị Cục ATTP/Sở Y tế kiểm tra → đình chỉ kinh doanh.

## 📋 9 NHÓM TỪ CẦN TRÁNH (theo gốc PTL)

> ⚠️ **Đọc cách dùng**: nếu ad/landing page có những từ dưới đây → **HIGH RISK bị flag/từ chối**. Không có nghĩa là 100% bị từ chối — FB đọc ngữ cảnh — nhưng pattern này đã làm hỏng nhiều account.

### Nhóm 1 — Y tế / Sức khoẻ ⚠️ **TPCN ƯU TIÊN ĐỌC**

#### 1.1. Bộ phận cơ thể (FB cấm buôn bán bộ phận người, thuật toán quét keyword)

> Gan, tim, thận, bao tử, xương khớp...

#### 1.2. Tên chủ thể bệnh

> Viêm xoang, thấp khớp, suy thận, cao huyết áp, ung thư, **béo phì** *(gốc nguyên văn: "Từ này rất dễ vi phạm nếu bạn bán thực phẩm chức năng")*... hoặc bất kỳ căn bệnh nào tương tự.

#### 1.3. Sức khoẻ cá nhân (FB cấm hình before/after và mô tả kết quả không mong muốn)

> Bác sĩ chữa trị, bác sĩ điều trị, cấp cứu, khỏi bệnh, xét nghiệm, chết chóc, đau đớn, tuyệt vọng, thất vọng, tự tử, tử nạn, bệnh nhân, bệnh nhi, phòng khám bệnh...

#### 1.4. Thuốc chữa bệnh

> Thuốc giảm cân, thuốc tăng cân, thuốc trị cao huyết áp, thuốc đông y, thuốc trị suy thận, thuốc tăng cường sinh lý...

#### 1.5. Thành phần hoá/sinh học

> Collagen, Omega 3, vitamin – omega, axit – chất xơ, thành phần dược liệu trong thuốc...

⚠️ **CỰC KỲ QUAN TRỌNG**: TPCN của anh có thể bán collagen / vitamin / omega — mà chính tên thành phần có trong list. Cần học **cách viết khéo** (vd: "dưỡng chất hỗ trợ làn da" thay vì "collagen").

#### 1.6. Yêu cầu thông tin sức khoẻ

KHÔNG được đòi user khai sức khoẻ thể chất/tinh thần/bệnh tật trong form ads.

### Nhóm 2 — Spa / Thẩm mỹ viện

KHÔNG được viết câu kiểu:
- "Bạn đang thừa cân/béo phì?"
- "Bạn cảm thấy muộn phiền vì gương mặt của mình?"
- "Đừng tự ti về vòng 2 của bạn."
- "Chúng tôi là dịch vụ spa số một ở Việt Nam."
- "Liệu trình giúp chị em ngoài 40 trẻ lại 10 tuổi."
- "Quy trình thần kỳ đã được nhiều chị em thử nghiệm và thành công."
- "Phương pháp tăng vòng 1/vòng 3, giảm vòng 2 thần kỳ."
- "Đảm bảo giảm 10 ký sau 3 lần điều trị."

→ Nguyên tắc Meta: **không gợi nhắc personal attributes** (cân nặng, mụn, lão hoá...).

### Nhóm 3 — Tài chính / Tiền tệ *(không liên quan TPCN nhiều, nhưng team biết để tránh nếu chạy ads cross-sell sản phẩm tài chính)*

#### 3.1. Cho vay
> Vay, vay vốn, tiền tệ, tài chính, vay tín chấp, vay tín dụng, lãi suất, thuế, cho vay vốn, giải ngân, vay nóng... + bất kỳ payday loan.

#### 3.2. Đấu giá tiền xu/cổ — cấm 100%.

#### 3.3. Sản phẩm tài chính
- Cấm: ICO tiền ảo, quyền chọn nhị phân (binary options), CFD.
- Cấm yêu cầu user cung cấp số tài khoản/định tuyến/thẻ tín dụng/ghi nợ.

### Nhóm 4 — Giới tính / Quốc gia / Chủng tộc (HẠN CHẾ, không cấm 100%)

| Loại | Ví dụ |
|---|---|
| Giới tính | ông, bà, chú, cô, anh, em, nữ giới, nam giới (kiểu "ông lớn VinGroup", "anh ruột tôi...") |
| Quốc gia | Việt Nam, Nhật Bản, Hàn Quốc, Mỹ... |
| Chủng tộc | người dân tộc, người da đen, người da trắng... |

→ Nguyên tắc: **không nhắm vào nhóm bảo vệ** (protected class).

### Nhóm 5 — Theo dõi / Xâm phạm riêng tư

> Camera theo dõi, camera an ninh, camera quay lén, dịch vụ thám tử, theo dõi, phần mềm gián điệp...

### Nhóm 6 — Cam kết / Chắc chắn / So sánh nhất

⚠️ **TPCN ƯU TIÊN TRÁNH**:

> Cam kết 100%, đảm bảo 100%, chắc chắn rằng, sản phẩm uy tín nhất, thương hiệu nổi tiếng nhất của Mỹ (Pháp, Đức...), cam kết có việc làm sau khoá học...

→ Lý do TPCN trúng nặng: TPCN không được phép cam kết hiệu quả tuyệt đối (vi phạm cả FB lẫn luật QC VN).

### Nhóm 7 — Thương hiệu đã đăng ký

Cấm nhắc tên thương hiệu lớn (**Sneaker, Adidas, Pepsi**...) trong text/ảnh/video — TRỪ KHI là nhà phân phối chính thức có giấy tờ.

### Nhóm 8 — Các từ cấm khác (gộp)

⚠️ **TPCN trúng trực tiếp**:

> Thuốc lá, rượu, cờ bạc; Trị mụn, trị sẹo, trị thâm; Tăng cân, giảm cân, các từ chỉ thể trạng; **Thực phẩm chức năng**; Ăn kiêng; Hộ chiếu, sổ đỏ, sổ hộ khẩu, hẹn hò.

→ **Đây là vấn đề lớn nhất**: chính cụm "Thực phẩm chức năng" nằm trong từ cấm. Tức là FB tự động nghi ngờ ngay khi thấy ngành.

### Nhóm 9 — Hình ảnh

| Loại | Cấm/Hạn chế |
|---|---|
| 9.1. Ảnh nhạy cảm | Ảnh phẫu thuật, cận cảnh (thẩm mỹ, nha khoa) |
| 9.2. Ảnh so sánh trước-sau | **Before/after — TPCN cực kỳ tránh** |
| 9.3. Ảnh lộ da, bộ phận nhạy cảm | Bikini, đồ lót, trang sức cận cảnh, spa, mỹ phẩm |

## 🔴 Lỗi tài khoản — pattern khiến FB disable BM (gốc cuối tài liệu)

- Vi phạm chính sách QC.
- Từng vi phạm nhiều lần.
- Tạo nhiều quảng cáo liên tục, nhiều IP/wifi/thiết bị khác nhau.
- Không thanh toán nợ FB.
- Không hoạt động thường xuyên.
- Quản trị viên chung tài khoản có hành vi đáng ngờ.

## ⛔ 4 KỸ THUẬT VPCS — KHÔNG ĐƯỢC DÙNG

> ⚠️ **Đây là phần "bí thuật" trong tài liệu PTL gốc — anh Chương đã chốt KHÔNG dùng**. Em ghi lại ở đây để **TEAM BIẾT mà CẢNH GIÁC** — nếu nhân viên cũ (đã từng chạy ads ngành xăm) đề xuất dùng, anh có cơ sở từ chối.

| # | Kỹ thuật trong gốc | Rủi ro | Nguyên tắc anh Chương | 
|---|---|---|---|
| 1 | "Sét chiến dịch như bình thường nhưng thay vì dùng bài có sẵn → tạo bài QC mới" | Trung bình. Bài mới chưa có lịch sử bị report → dễ qua duyệt lần đầu. NHƯNG lặp pattern → FB nhận ra → disable. | ❌ KHÔNG DÙNG |
| 2 | "Camp đã lên không chỉnh sửa — sửa sẽ bị FB để ý" | Thấp về policy nhưng giới hạn khả năng tối ưu CPM/CPL | ⚠️ KHÔNG SỬA TRONG LEARNING PHASE — đây là **best practice chuẩn FB** chứ không phải kỹ thuật né |
| 3 | "Không tắt cam, chỉ giảm hoặc tăng ngân sách" | Thấp. Đây là **best practice chuẩn FB** (tránh reset learning phase) — không phải VPCS thật | ✅ Đây là cách đúng — không liên quan né luật |
| 4 | "Set 1-3-6: 1 chiến dịch, 3 nhóm, 6 bài. Ngân sách nhóm bằng nhau, nhóm nào ngon giữ lại" | Thấp. Đây là cấu trúc **ABO testing chuẩn** — không vi phạm | ✅ Cấu trúc test phổ biến, dùng được |

> ✋ Thực tế: gọi là "bí thuật VPCS" nhưng phần lớn là kỹ thuật vận hành tài khoản chuẩn FB. Phần "lách" thật chỉ là kỹ thuật #1 (tạo bài mới mỗi lần để qua duyệt).
>
> Tài liệu có 1 dòng nói thêm "Công cụ lách content khi lên camp ae tìm trên gg có rất nhiều" — KHÔNG nêu tên cụ thể. **Anh Chương ĐÃ CHỐT KHÔNG DÙNG.**

## ✅ HƯỚNG WHITE-HAT — Cách viết content TPCN ĐÚNG LUẬT mà vẫn hiệu quả

> 📎 Phần này em (agent) đề xuất từ best practice industry — KHÔNG có trong tài liệu PTL gốc.

### 5 nguyên tắc viết content TPCN đúng luật

1. **Không cam kết hiệu quả tuyệt đối** — dùng "hỗ trợ", "góp phần", "nhiều người dùng phản hồi" thay vì "chữa khỏi", "đảm bảo".
2. **Không gợi nhắc bệnh trực tiếp** — dùng "khi cảm thấy mệt mỏi", "tình trạng mất ngủ kinh niên" thay vì "bệnh suy nhược thần kinh".
3. **Bắt buộc disclaimer** "**Sản phẩm này không phải là thuốc, không có tác dụng thay thế thuốc chữa bệnh.**" — đặt cuối ad + landing page.
4. **Số đăng ký Cục ATTP** — hiển thị trên trang sản phẩm.
5. **Bác sĩ chuyên môn xuất hiện** — tăng E-E-A-T (xem [[E-E-A-T]] từ Khối 9).

### Pattern an toàn — thay thế từ cấm

| Từ rủi ro | Thay bằng (white-hat) |
|---|---|
| "Chữa bệnh X" | "Hỗ trợ tình trạng X" hoặc "Người dùng thường gặp vấn đề X chia sẻ..." |
| "Cam kết 100%" | "Nhiều khách hàng đã phản hồi tích cực sau N tuần sử dụng" |
| "Trị mụn" | "Hỗ trợ làn da khoẻ mạnh" |
| "Giảm cân thần tốc" | "Hỗ trợ kiểm soát vóc dáng kết hợp chế độ ăn + tập luyện" |
| "Bạn đang béo phì?" | "Bạn quan tâm đến lối sống lành mạnh?" |
| "Trước-sau" *(ảnh)* | Quá trình sử dụng + chia sẻ trải nghiệm *(không so sánh trực tiếp)* |
| "Thực phẩm chức năng" | "Sản phẩm bổ sung dinh dưỡng" *(tuỳ ngữ cảnh)* |

⚠️ **Lưu ý**: pattern thay thế trên là **suy luận white-hat** — không có trong tài liệu PTL gốc. Khi triển khai phải có **luật sư + cục ATTP duyệt** — đây là YMYL.

## 💬 Trích dẫn nguyên văn từ gốc

> "Béo phì — Từ này rất dễ vi phạm nếu bạn bán thực phẩm chức năng." *(dòng 7)*

> "Camp đã lên không chỉnh sửa sẽ rất dễ bị facebook để ý vì camp của ông phải có vấn đề ông mới sửa và xét duyệt lại từ đầu." *(dòng 3)*

> "Thực phẩm chức năng" — nằm trong list "MỘT SỐ TỪ NGỮ BỊ CẤM TRONG QUẢNG CÁO FACEBOOK KHÁC" *(dòng 62)*

## 🎯 Hành động cho team viết ads TPCN

> Đã đẩy vào [[../../actions|actions.md]].

1. **Trước viết creative đầu tiên** — luật sư review pháp lý + xin xác nhận nội dung quảng cáo từ Cục ATTP.
2. **Mọi creative + landing page** — qua **2 vòng QA**: (a) check 9 nhóm từ cấm ở trên; (b) check disclaimer + đăng ký Cục ATTP hiển thị đầy đủ.
3. **Hàng tháng** — tra cứu **Meta Advertising Standards** mới nhất (đặc biệt mục Health & Wellness) → cập nhật lại checklist này.
4. **Onboarding nhân viên ads mới** — đọc bắt buộc file này + [[Special Ad Category + chính sách Health-YMYL]] **TRƯỚC khi viết bài đầu tiên**.

## 🔗 Liên kết

- [[Khối 14 - ADS Các nền tảng]] — page mẹ
- [[Khối 14a - ADS Facebook]] — phần policy chi tiết
- [[Special Ad Category + chính sách Health-YMYL]] — concept Meta policy
- [[E-E-A-T]] — bác sĩ chuyên môn = xương sống tin cậy
- [[Khối 9 - SEO Blog 2026]] — TPCN = YMYL
