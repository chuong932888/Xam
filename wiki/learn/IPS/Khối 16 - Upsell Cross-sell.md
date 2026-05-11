---
type: source
tags: [ips, khoi-16, upsell, cross-sell, aov, ptl]
created: 2026-05-09
updated: 2026-05-09
sources: ["[[raw/Đặc sản của Phạm Thành Long/IPS - 19 khối công việc/16_ Upsell_Cross-sell]]"]
khoi: 16
status: active
---

# Khối 16 — Upsell / Cross-sell (Hệ thống dùng chung mọi ngành)

> Nguồn: thầy [[Phạm Thành Long]], khoá [[index|IPS]] — file gốc `16_ Upsell_Cross-sell.docx` (1062 dòng, 27 phần).
> ✅ PTL gốc nói: toàn bộ framework, định nghĩa, công thức, ma trận, kịch bản, ví dụ đa ngành.
> 📎 Em (agent) thêm: TL;DR, vai trò TPCN, ví dụ TPCN ở các bảng, hành động sau khi đọc.
> 💎 Đây là file **đậm đặc nhất** trong 4 file ingest hôm nay — nên đọc kỹ để dựng hệ thống bán thêm cho TPCN.

## 🎯 TL;DR — đọc 5 phút

**Câu định vị mạnh nhất** (PTL):
> *"Upsell/cross-sell không phải là 'bán thêm'. Đó là giúp khách mua đủ để đạt kết quả họ muốn."*

**Khác biệt người yếu vs người giỏi**:
- Người yếu: "Anh/chị lấy thêm cái này không?"
- Người giỏi: "Để dùng cái này ra kết quả tốt, anh/chị còn thiếu 1–2 phần quan trọng. Tôi tách cho anh/chị 3 mức: tiết kiệm, cân bằng, và tối ưu."

**3 đòn bẩy vàng**:
1. **Mô hình 3 tầng Tiết kiệm/Cân bằng/Tối ưu** — bán dễ nhất gói giữa.
2. **Chẩn đoán trước, bán sau** — 5 câu hỏi trước khi đề xuất.
3. **Bán theo hành trình, không theo sản phẩm** — sản phẩm có thể đổi, hành trình KH (chưa biết → mua thử → muốn kết quả tốt → muốn duy trì) gần như luôn giống nhau.

**4 việc hệ thống đúng phải làm được**:
1. Chẩn đoán đúng nhu cầu
2. Đưa 3 mức lựa chọn rõ ràng
3. Gợi ý món bổ trợ có lý do thật
4. Chăm sóc sau mua để bán tiếp tự nhiên

## 🧭 Vai trò Khối 16 với TPCN

- **Đòn bẩy AOV (giá trị đơn trung bình) lớn nhất**. KH TPCN không mua 1 hộp — họ mua liệu trình. Upsell từ "hộp đơn" lên "liệu trình 3 tháng" + cross-sell vitamin C / lộ trình ăn uống / tư vấn 1-1 → AOV tăng đáng kể so với bán lẻ. *(Mức tăng cụ thể em không có số liệu PTL — anh tự đo qua AOV/Attach Rate sau khi triển khai.)*
- **TPCN có lợi thế tự nhiên cho cross-sell**: sản phẩm tiêu hao theo chu kỳ (30/60/90 ngày) → bán định kỳ + membership rất phù hợp.
- **Ngách TPCN cụ thể chưa chốt** — anh sẽ điền vào "Mẫu bảng triển khai 1 sản phẩm" (mục 20) khi chốt sản phẩm chính.

## 📋 27 PHẦN ĐẦY ĐỦ

---

### 1. Hiểu đúng: Upsell và Cross-sell

#### Upsell = bán bản tốt hơn (nâng cấp lựa chọn hiện tại)

| Khách định mua | Upsell đúng |
|---|---|
| Gói cơ bản | Gói tiêu chuẩn / cao cấp |
| Sản phẩm dung lượng nhỏ | Dung lượng lớn hơn, dùng lâu hơn |
| Dịch vụ thường | Dịch vụ nhanh hơn / kỹ hơn / bảo hành tốt hơn |
| Khoá học cơ bản | Khoá có sửa bài + lộ trình + hỗ trợ |
| Phần mềm gói thấp | Gói nhiều tính năng / nhiều người dùng |

**Cách nói**:
- ❌ "Cái này đắt hơn"
- ✅ "Cái này phù hợp hơn với mục tiêu của anh/chị"

#### Cross-sell = bán thêm thứ bổ trợ (giúp sản phẩm chính phát huy hiệu quả)

| Khách mua | Cross-sell đúng |
|---|---|
| Điện thoại | Ốp, sạc, tai nghe, bảo hành |
| Khoá học | Tài liệu, coaching, bài tập, cộng đồng |
| Máy móc | Vật tư, bảo trì, hướng dẫn sử dụng |
| Dịch vụ spa | Sản phẩm chăm sóc tại nhà |
| Nhà hàng | Món phụ, đồ uống, tráng miệng |
| Phần mềm | Đào tạo sử dụng, tích hợp, hỗ trợ kỹ thuật |
| Nội thất | Giao lắp, vệ sinh, bảo hành mở rộng |

**Cách nói**:
- ❌ "Mua thêm đi"
- ✅ "Nếu thiếu phần này, trải nghiệm chính sẽ không trọn vẹn"

---

### 2. Nguyên tắc gốc: Bán theo KẾT QUẢ, không bán theo món hàng

KH không thật sự mua sản phẩm. Họ mua kết quả.

| Ngành | Khách tưởng họ mua | Thật ra họ mua |
|---|---|---|
| Làm đẹp | Kem, liệu trình, mỹ phẩm | Da đẹp hơn, tự tin hơn |
| Giáo dục | Khoá học | Kỹ năng, nghề nghiệp, thu nhập |
| Nhà hàng | Món ăn | Trải nghiệm, no bụng, vui vẻ |
| Bán lẻ | Sản phẩm | Tiện lợi, an tâm, thể hiện bản thân |
| Phần mềm | Tính năng | Tiết kiệm thời gian, giảm lỗi, tăng hiệu quả |
| Thiết bị | Máy móc | Hiệu suất, độ bền, ít hỏng |
| Tư vấn DN | Gói tư vấn | Giải quyết vấn đề, tăng doanh thu, giảm rủi ro |

📎 **TPCN**: KH tưởng mua "viên collagen" — thật ra mua "tự tin khi nhìn gương + được khen trẻ + bớt lo già".

**Câu hỏi gốc của hệ thống**: *Khách muốn đạt kết quả gì, và họ còn thiếu gì để đạt kết quả đó?*

---

### 3. Công thức hệ thống dùng chung

> Sản phẩm chính → Mục tiêu của khách → Rủi ro nếu mua thiếu → Món nâng cấp → Món bổ trợ → Gói đề xuất → Chăm sóc sau mua

**Bảng xương sống**:

| Thành phần | Câu hỏi cần trả lời |
|---|---|
| Sản phẩm chính | Khách đang muốn mua gì? |
| Mục tiêu | Họ mua để làm gì? |
| Rủi ro | Nếu chỉ mua món này thì có thể thiếu gì, lỗi gì, bất tiện gì? |
| Upsell | Phiên bản nào tốt hơn, bền hơn, nhanh hơn, đầy đủ hơn? |
| Cross-sell | Cần thêm gì để dùng tốt hơn? |
| Gói | Có thể đóng thành combo nào dễ chọn? |
| Sau mua | Khi nào KH cần mua tiếp, nâng cấp, bảo trì, học thêm? |

---

### 4. Mô hình 3 tầng: TIẾT KIỆM – CÂN BẰNG – TỐI ƯU

> **Không nên chỉ đưa 1 lựa chọn. Cũng không nên đưa quá nhiều. Tốt nhất là 3 mức.**

| Mức | Dành cho ai | Mục tiêu | Cách nói |
|---|---|---|---|
| **Tiết kiệm** | Người mới thử, ngân sách thấp | Đủ dùng, ít rủi ro | "Mức này đủ để bắt đầu" |
| **Cân bằng** ⭐ | Người nghiêm túc, muốn hiệu quả tốt | Đủ đầy, đáng tiền nhất | "Mức này phù hợp nhất với đa số khách" |
| **Tối ưu** | Người muốn kết quả cao, dùng lâu dài | Trọn gói, ít phải đổi/nâng cấp | "Mức này dành cho người muốn làm bài bản" |

**Cách trình bày chuẩn**:
> "Em có 3 hướng: Tiết kiệm — đủ dùng. Cân bằng — hợp lý nhất, ít thiếu. Tối ưu — đầy đủ, dùng lâu dài, ít phải nâng cấp. Anh/chị muốn tôi ghép theo hướng nào?"

→ Cách bán **rất sạch**. Không ép khách. Nhưng KH dễ ra quyết định.

---

### 5. Luật vàng: KHÔNG upsell trước khi chẩn đoán

**Sai lầm lớn nhất**: vừa thấy KH hỏi giá đã đẩy gói cao → KH nghĩ *"Ông này chỉ muốn moi tiền mình"*.

**Cách đúng**: hỏi 3–5 câu chẩn đoán trước.

#### 5 câu hỏi chẩn đoán dùng chung (HỌC THUỘC)

1. "Anh/chị mua để dùng cho mục đích gì?"
2. "Mình dùng một lần, dùng thường xuyên, hay dùng lâu dài?"
3. "Hiện anh/chị đã có những gì rồi?"
4. "Điều anh/chị sợ nhất khi mua là gì: tốn tiền, mua sai, khó dùng, không hiệu quả, hay thiếu hỗ trợ?"
5. "Ngân sách mình muốn giữ trong khoảng nào?"

**Sau đó mới đề xuất**:
> "Dựa trên mục tiêu của anh/chị, tôi không khuyên chọn bản rẻ nhất. Tôi khuyên chọn bản cân bằng vì nó giải quyết đúng vấn đề anh/chị đang lo."

→ **Upsell dựa trên nhu cầu, không phải upsell dựa trên lòng tham.**

---

### 6. 8 NHÓM UPSELL DÙNG ĐƯỢC MỌI NGÀNH

#### 1. Upsell theo CHẤT LƯỢNG
Bản thường → bản tốt hơn.
- Sản phẩm phổ thông → sản phẩm cao cấp
- Dịch vụ thường → dịch vụ chuyên sâu
- Khoá học video → khoá học có sửa bài
- Gói phần mềm cơ bản → gói chuyên nghiệp

> "Bản cơ bản dùng được. Nhưng nếu anh/chị muốn ổn định hơn, bền hơn, ít lỗi hơn thì bản này đáng hơn."

#### 2. Upsell theo TỐC ĐỘ
Chậm → nhanh.
- Giao thường → giao nhanh
- Dịch vụ 7 ngày → dịch vụ 24 giờ
- Hỗ trợ thường → hỗ trợ ưu tiên
- Khoá tự học → khoá có người kèm

> "Nếu anh/chị không gấp, gói thường ổn. Nếu cần kết quả nhanh và ít mất thời gian tự xử lý, gói nhanh hợp hơn."

#### 3. Upsell theo ĐỘ ĐẦY ĐỦ
Một phần → trọn gói.
- Mua lẻ → mua combo
- Tư vấn một buổi → lộ trình nhiều buổi
- Sản phẩm đơn → bộ đầy đủ
- Khoá học đơn lẻ → chương trình hoàn chỉnh

> "Mua lẻ thì được, nhưng dễ thiếu. Gói này được ghép để anh/chị dùng trọn vẹn hơn."

#### 4. Upsell theo BẢO HÀNH / AN TÂM
Không bảo vệ → có bảo vệ.
- Bảo hành thường → bảo hành mở rộng
- Hỗ trợ cơ bản → hỗ trợ cao cấp
- Dịch vụ một lần → dịch vụ có cam kết theo dõi
- Sản phẩm → sản phẩm + bảo trì

> "Phần này không phải mua vì hôm nay cần, mà mua để khi có vấn đề thì không bị động."

#### 5. Upsell theo CÁ NHÂN HOÁ
Mẫu có sẵn → làm riêng theo tình huống của khách.
- Mẫu có sẵn → thiết kế riêng
- Gói chung → gói theo nhu cầu
- Khoá đại trà → coaching cá nhân
- Dịch vụ tiêu chuẩn → dịch vụ theo yêu cầu

> "Bản thường phù hợp số đông. Nhưng trường hợp của anh/chị có điểm riêng, nên bản cá nhân hoá sẽ ít sai hơn."

#### 6. Upsell theo TẦN SUẤT SỬ DỤNG
KH dùng càng nhiều, càng nên mua bản tốt hơn.
- Dùng 1 lần → bản cơ bản
- Dùng hằng tuần → bản tốt
- Dùng hằng ngày → bản cao cấp
- Dùng để kinh doanh → bản chuyên nghiệp

> "Nếu dùng ít thì bản thường đủ. Nhưng nếu dùng thường xuyên, bản rẻ sẽ nhanh lộ điểm yếu."

#### 7. Upsell theo MỤC TIÊU KIẾM TIỀN
Dành cho khách mua để làm nghề, kinh doanh, tạo thu nhập.
- Học chơi → học làm nghề
- Dùng cá nhân → dùng kinh doanh
- Công cụ nhỏ → hệ thống làm việc
- Sản phẩm lẻ → bộ chuyên nghiệp

> "Nếu mua để dùng chơi, mình chọn tiết kiệm. Nếu mua để tạo thu nhập, nên chọn theo độ ổn định và hiệu quả dài hạn."

#### 8. Upsell theo GIẢM RỦI RO
KH không sợ trả thêm tiền — họ sợ trả tiền sai.
> "Bản rẻ không sai. Nó chỉ sai nếu mục tiêu của anh/chị cần nhiều hơn thế."
> Hoặc: "Tốn thêm một chút lúc đầu có thể giúp tránh tốn lại nhiều lần về sau."

---

### 7. 10 NHÓM CROSS-SELL DÙNG ĐƯỢC MỌI NGÀNH

#### 1. Món BẮT BUỘC ĐỂ DÙNG ĐƯỢC
Máy cần phụ kiện · Khoá học cần tài liệu/bài tập · Phần mềm cần cài đặt · Sản phẩm cần bộ sạc, dây, vật tư.
> "Món chính là phần lõi. Nhưng để dùng được ngay, anh/chị cần thêm phần này."

#### 2. Món GIÚP DÙNG TỐT HƠN
Sản phẩm chăm sóc sau dịch vụ · Tài liệu kèm khoá học · Công cụ kèm phần mềm · Phụ kiện tăng hiệu suất.
> "Cái này không bắt buộc, nhưng giúp trải nghiệm tốt hơn rõ rệt."

#### 3. Món GIÚP TIẾT KIỆM THỜI GIAN
Giao nhanh · Lắp đặt tận nơi · Cài đặt sẵn · Hướng dẫn sử dụng · Dịch vụ làm thay.
> "Nếu anh/chị muốn tự làm thì không cần. Nếu muốn tiết kiệm thời gian và tránh lỗi, nên thêm phần này."

#### 4. Món GIÚP GIẢM LỖI
Hướng dẫn chuyên sâu · Bảo trì · Kiểm tra định kỳ · Gói hỗ trợ · **Checklist sử dụng** (= danh sách kiểm tra, giúp không bỏ sót bước quan trọng).
> "Phần này giúp anh/chị tránh lỗi khi dùng, đặc biệt là giai đoạn đầu."

#### 5. Món TIÊU HAO / MUA ĐỊNH KỲ ⭐ *(quan trọng cho TPCN)*
Mỹ phẩm dùng hằng tháng · Vật tư ngành nghề · Phụ kiện thay thế · Gói bảo trì · Gói nguyên liệu · Gói thuê bao.
> "Cái này dùng hết theo thời gian. Mua theo combo sẽ đỡ thiếu và thường tiết kiệm hơn."

#### 6. Món BẢO VỆ SẢN PHẨM CHÍNH
Ốp, túi, hộp bảo vệ · Bảo hành mở rộng · Vệ sinh/bảo dưỡng · Bảo hiểm thiết bị · Dịch vụ kiểm tra định kỳ.
> "Mình đã đầu tư món chính rồi, phần này giúp bảo vệ khoản đầu tư đó."

#### 7. Món NÂNG TRẢI NGHIỆM
Đồ uống kèm món ăn · Quà tặng kèm dịch vụ · Gói phòng đẹp hơn · Phụ kiện thẩm mỹ · **Thành viên VIP** (Very Important Person — KH đặc biệt, được ưu tiên).
> "Phần này không bắt buộc, nhưng làm trải nghiệm trọn vẹn hơn."

#### 8. Món ĐÀO TẠO / HƯỚNG DẪN
Khoá hướng dẫn · Buổi coaching · Tài liệu sử dụng · Workshop · Cộng đồng hỗ trợ.
**Coaching** = kèm cặp trực tiếp, giúp KH làm đúng và sửa lỗi nhanh.
> "Mua sản phẩm là một phần. Biết dùng đúng mới tạo ra kết quả."

#### 9. Món CÁ NHÂN HOÁ
Khắc tên · Thiết kế riêng · Gói theo nhu cầu · Cấu hình riêng · Tư vấn riêng.
> "Nếu muốn giống số đông thì bản thường được. Nếu muốn hợp với anh/chị hơn, bản cá nhân hoá sẽ đáng hơn."

#### 10. Món CỘNG ĐỒNG / THÀNH VIÊN ⭐ *(quan trọng cho TPCN)*
**Membership** (= gói thành viên, KH trả tiền hoặc đăng ký để nhận quyền lợi định kỳ) · Câu lạc bộ KH · Gói định kỳ · Nhóm hỗ trợ · Ưu đãi thành viên.
> "Nếu anh/chị dùng thường xuyên, gói thành viên sẽ lợi hơn mua từng lần."

---

### 8. Ma trận Upsell/Cross-sell dùng chung

| Khách mua | Upsell nên gợi ý | Cross-sell nên gợi ý | Cách nói |
|---|---|---|---|
| Sản phẩm cơ bản | Bản tốt hơn / bền hơn | Phụ kiện, bảo hành, hướng dẫn | "Bản này đủ dùng, nhưng bản kia ổn định hơn nếu dùng lâu" |
| Dịch vụ một lần | Gói nhiều buổi / chuyên sâu | Chăm sóc sau dịch vụ, sản phẩm hỗ trợ | "Một lần giải quyết trước mắt, gói này giúp duy trì kết quả" |
| Khoá học | Gói có sửa bài / coaching | Tài liệu, cộng đồng, công cụ | "Học xong mà có người sửa lỗi sẽ tiến nhanh hơn" |
| Phần mềm | Gói nhiều tính năng | Cài đặt, đào tạo, tích hợp | "Có phần mềm chưa đủ, đội cần biết dùng đúng" |
| Thiết bị | Bản công suất cao hơn | Bảo trì, phụ kiện, vật tư | "Thiết bị tốt cần vật tư và bảo trì đúng để bền" |
| Đồ ăn / uống | Size lớn / combo | Món phụ, topping, tráng miệng | "Combo này đủ bữa hơn và lợi hơn mua lẻ" |
| Làm đẹp | Liệu trình cao hơn | Sản phẩm chăm sóc tại nhà | "Làm tại tiệm là một phần, chăm ở nhà mới giữ kết quả" |
| Tư vấn | Gói triển khai | Theo dõi, báo cáo, đào tạo đội ngũ | "Tư vấn chỉ ra hướng, triển khai mới tạo kết quả thật" |

---

### 9. Luật đề xuất: KHI NÀO BÁN GÌ?

> Không phải lúc nào cũng upsell/cross-sell. Phải đúng thời điểm.

#### Thời điểm 1: TRƯỚC KHI MUA
- **Mục tiêu**: chẩn đoán và định hướng.
- **Câu nói**: "Trước khi chốt, tôi hỏi nhanh để tránh anh/chị mua sai."
- Phù hợp: upsell theo mục tiêu.

#### Thời điểm 2: KHI KH ĐÃ CHỌN SẢN PHẨM CHÍNH
- **Mục tiêu**: đề xuất món bổ trợ cần thiết.
- **Câu nói**: "Anh/chị chọn món chính này là ổn. Để dùng trọn vẹn hơn, có 2 món nên cân nhắc."
- Phù hợp: cross-sell.

#### Thời điểm 3: LÚC THANH TOÁN
- **Mục tiêu**: thêm món nhỏ, dễ quyết.
- Ví dụ: phụ kiện, gói bảo hành, dịch vụ giao nhanh, sản phẩm tiêu hao, tài liệu hướng dẫn.
- **Câu nói**: "Món này nhiều khách mua kèm vì dùng ngay với sản phẩm chính."

#### Thời điểm 4: SAU KHI MUA 1–3 NGÀY
- **Mục tiêu**: hỗ trợ sử dụng, phát hiện thiếu sót.
- **Tin nhắn**: "Anh/chị dùng thử chưa? Có điểm nào vướng không? Tôi kiểm tra giúp để dùng đúng ngay từ đầu."
- → Cross-sell rất tự nhiên vì xuất phát từ vấn đề thật.

#### Thời điểm 5: SAU 7–14 NGÀY
- **Mục tiêu**: nâng cấp hoặc bổ sung.
- **Tin nhắn**: "Sau một thời gian dùng, thường khách sẽ gặp 1 trong 3 vấn đề này. Anh/chị đang vướng điểm nào?"
- Phù hợp bán: hướng dẫn nâng cao, bảo trì, phụ kiện, dịch vụ chuyên sâu, gói chăm sóc tiếp.

#### Thời điểm 6: SAU 30 NGÀY HOẶC CHU KỲ TIÊU HAO ⭐ *(vàng cho TPCN)*
- **Mục tiêu**: bán lại, bán định kỳ.
- **Tin nhắn**: "Phần này thường dùng hết sau khoảng X ngày. Anh/chị có muốn tôi chuẩn bị gói định kỳ để khỏi bị thiếu không?"
- Phù hợp: ngành có sản phẩm tiêu hao, dịch vụ lặp lại, bảo trì, chăm sóc.

---

### 10. Cách đóng gói OFFER

**Offer** = đề nghị bán hàng, tức toàn bộ thứ KH nhận được khi mua.

**Một offer tốt gồm 6 phần**:

| Thành phần | Vai trò |
|---|---|
| Sản phẩm/dịch vụ chính | Thứ KH đang muốn mua |
| Kết quả cam kết hợp lý | KH hiểu mua xong được gì |
| Món bổ trợ | Giúp dùng tốt hơn |
| Hỗ trợ | Giúp KH yên tâm |
| Ưu đãi | Tạo lý do mua ngay |
| Lựa chọn rõ ràng | Giúp KH dễ quyết |

**Công thức**: *Gói Cân Bằng = Sản phẩm chính + món cần thiết + hướng dẫn + bảo hành/hỗ trợ + ưu đãi khi mua combo*.

**Cách viết**:
- ❌ "Combo A gồm 5 món"
- ✅ "Combo A giúp anh/chị bắt đầu đầy đủ, không thiếu đồ, không phải mua lẻ nhiều lần"

---

### 11. Đặt tên gói theo KẾT QUẢ, không đặt theo giá

| Tên yếu | Tên mạnh |
|---|---|
| Gói cơ bản | Gói **bắt đầu đúng** |
| Gói trung bình | Gói **cân bằng** |
| Gói cao cấp | Gói **tối ưu dài hạn** |
| Combo sản phẩm | **Bộ dùng trọn vẹn** |
| Gói dịch vụ | **Lộ trình giải quyết vấn đề** |
| Gói học | **Lộ trình làm được** |

**Tên tốt phải trả lời câu hỏi**: "Khách mua xong sẽ đạt điều gì?"

📎 **TPCN gợi ý**: "Lộ trình da căng 60 ngày" / "Bộ trẻ hoá toàn diện U40" / "Gói duy trì sắc đẹp 12 tháng" — thay vì "Gói 1, Gói 2, Gói 3".

---

### 12. KỊCH BẢN BÁN HÀNG dùng chung (7 tình huống)

#### Kịch bản 1: KHI KHÁCH HỎI GIÁ
> Khách: "Cái này bao nhiêu?"
> Người bán: "Giá bản này là X. Nhưng để tránh anh/chị mua sai, tôi hỏi nhanh: mình dùng cho mục đích gì và dùng thường xuyên không?"
>
> *(Sau khi khách trả lời)*: "Vậy tôi tách cho anh/chị 3 lựa chọn: tiết kiệm, cân bằng và tối ưu. Anh/chị không cần lấy bản đắt nhất, chỉ cần lấy bản đúng mục tiêu."

#### Kịch bản 2: KHI MUỐN UPSELL
> "Bản anh/chị đang chọn dùng được. Nhưng với mục tiêu anh/chị nói lúc nãy, tôi khuyên cân nhắc bản cao hơn vì nó giải quyết được 3 điểm: bền hơn, ít lỗi hơn, và đỡ phải nâng cấp sớm."

#### Kịch bản 3: KHI MUỐN CROSS-SELL
> "Món chính này là đúng. Nhưng nếu chỉ lấy món này thì anh/chị có thể thiếu phần hỗ trợ để dùng hiệu quả. Tôi gợi ý thêm món này vì nó giúp tránh lỗi/tiết kiệm thời gian/tăng trải nghiệm."

#### Kịch bản 4: KHI KH NÓI ĐẮT
> Khách: "Đắt quá."
> Người bán: "Đúng, nếu so với bản rẻ nhất thì nó đắt hơn. Nhưng mình đang so theo mục tiêu sử dụng. Nếu anh/chị chỉ dùng thử, tôi sẽ khuyên bản tiết kiệm. Nếu muốn dùng lâu dài và ít rủi ro, bản cân bằng đáng hơn."
>
> *(Sau đó)*: "Mình muốn tối ưu theo ngân sách trước mắt hay tối ưu theo hiệu quả lâu dài?"

#### Kịch bản 5: KHI KH CHỈ MUỐN MUA MÓN CHÍNH
> Khách: "Tôi lấy mỗi cái này thôi."
> Người bán: "Được. Tôi không ép mua thêm. Nhưng tôi nói rõ để anh/chị chủ động: món này dùng tốt nhất khi đi cùng phần này. Nếu anh/chị đã có rồi thì không cần mua. Nếu chưa có, tôi khuyên lấy thêm để tránh thiếu khi sử dụng."

#### Kịch bản 6: KHI KH PHÂN VÂN GIỮA 2 GÓI
> "Nếu ưu tiên tiết kiệm, chọn gói thấp. Nếu ưu tiên đỡ phải mua lại và dùng ổn định hơn, chọn gói giữa. Còn gói cao chỉ đáng nếu anh/chị dùng thường xuyên hoặc muốn làm bài bản."
>
> → **Tạo niềm tin** vì không cố đẩy gói cao bằng mọi giá.

#### Kịch bản 7: KHI KH CẦN QUYẾT ĐỊNH NHANH
> "Tôi chốt lại đơn giản: Gói thấp = đủ bắt đầu. Gói giữa = đáng tiền nhất. Gói cao = đầy đủ và lâu dài nhất. Với nhu cầu của anh/chị, tôi chọn gói giữa."
>
> → **Người bán giỏi phải DÁM khuyến nghị**. Không được chỉ ném lựa chọn cho khách tự bơi.

---

### 13. Công thức "KHÔNG THỂ BỎ QUA" — 5 yếu tố

Một đề xuất khiến KH khó bỏ qua thường có 5 yếu tố:

#### 1. Đúng VẤN ĐỀ
KH phải thấy: "Đúng là mình đang cần cái này."

#### 2. Đúng THỜI ĐIỂM
- Đừng bán bảo trì khi KH chưa mua máy.
- Đừng bán khoá nâng cao khi KH chưa học nền.
- Đừng bán gói cao khi KH chỉ thử nghiệm.

#### 3. Đúng MỨC TIỀN
Không phải rẻ nhất. Nhưng phải hợp với khả năng và mục tiêu.

#### 4. Có lý do MUA CÙNG LÚC
- Mua combo lợi hơn mua lẻ
- Có hướng dẫn đi kèm
- Có bảo hành/hỗ trợ
- Có ưu đãi khi mua cùng
- Có thể dùng ngay, không thiếu

#### 5. Có cảm giác BỎ QUA SẼ THIỆT
Không phải doạ khách. Mà chỉ ra hậu quả thật:
- Mua thiếu phải quay lại mua thêm
- Dùng sai dễ hỏng
- Không có hướng dẫn dễ mất thời gian
- Không bảo trì dễ giảm tuổi thọ
- Không học đúng dễ làm sai lâu dài

**Câu nói**: "Anh/chị có thể mua riêng từng phần. Nhưng nếu lấy cùng bộ này, mình dùng được ngay, đồng bộ hơn và có người hỗ trợ khi cần."

---

### 14. Cấu trúc COMBO chuẩn — 5 lớp

| Lớp | Nội dung | Ví dụ |
|---|---|---|
| Lớp 1 | Sản phẩm/dịch vụ chính | Máy, khoá học, liệu trình, phần mềm |
| Lớp 2 | Phần BẮT BUỘC | Phụ kiện, tài liệu, cài đặt |
| Lớp 3 | Phần TĂNG HIỆU QUẢ | Hướng dẫn, chăm sóc, bảo trì |
| Lớp 4 | Phần AN TÂM | Bảo hành, hỗ trợ, đổi trả |
| Lớp 5 | Phần GIỮ CHÂN | Ưu đãi lần sau, gói định kỳ, cộng đồng |

#### Mô hình chung 3 gói

| Gói | Có gì | Phù hợp với |
|---|---|---|
| **Tiết kiệm** | Sản phẩm chính + 1-2 phần cần thiết + hỗ trợ cơ bản | Người mới thử |
| **Cân bằng** ⭐ | Sản phẩm chính + đủ phần cần thiết + hướng dẫn sử dụng + hỗ trợ sau mua + ưu đãi tốt hơn mua lẻ | Đa số khách |
| **Tối ưu** | Bản tốt hơn + đầy đủ phần bổ trợ + hỗ trợ ưu tiên + bảo hành/chăm sóc mở rộng + theo dõi sau mua | Người dùng nghiêm túc, lâu dài, kinh doanh |

---

### 15. Hệ thống theo VÒNG ĐỜI KHÁCH HÀNG

> **Đừng nhìn khách như một đơn hàng. Hãy nhìn khách như một hành trình.**

| Giai đoạn | Tâm lý KH | Nên bán gì |
|---|---|---|
| Tìm hiểu | Chưa chắc, sợ mua sai | Gói nhập môn, tư vấn, bản dùng thử |
| Bắt đầu | Cần dễ dùng, ít rủi ro | Gói cơ bản + hướng dẫn |
| Dùng thường xuyên | Muốn tiện, ổn định | Gói cân bằng, phụ kiện, bảo trì |
| Nghiêm túc | Muốn kết quả tốt hơn | Gói nâng cấp, đào tạo, cá nhân hoá |
| Chuyên nghiệp | Muốn tối ưu hiệu suất | Gói cao cấp, hỗ trợ ưu tiên, hệ thống |
| Trung thành | Muốn lợi ích dài hạn | Thành viên, định kỳ, ưu đãi riêng |

**Đòn bẩy lớn nhất**: *Lần đầu bán đúng. Những lần sau bán dễ.* Lần đầu sai → KH không quay lại. Lần đầu đúng → KH tự nhiên tin khi đề xuất thêm.

---

### 16. Bảng LUẬT ĐỀ XUẤT sản phẩm

> Biến upsell/cross-sell thành **hệ thống**, không phụ thuộc cảm tính nhân viên.

| Tình huống KH | Dấu hiệu | Đề xuất chính | Upsell | Cross-sell |
|---|---|---|---|---|
| Mới bắt đầu | Hỏi nhiều, sợ sai, ngân sách thấp | Gói nhập môn | Gói có hướng dẫn | Tài liệu/phụ kiện cơ bản |
| Muốn dùng lâu | Hỏi độ bền, bảo hành | Gói cân bằng | Bản cao hơn | Bảo hành/bảo trì |
| Dùng thường xuyên | Hỏi số lượng, hiệu suất | Gói số lượng lớn | Gói chuyên nghiệp | Vật tư định kỳ |
| Cần nhanh | Hỏi thời gian, deadline | Gói nhanh | Hỗ trợ ưu tiên | Giao nhanh/làm thay |
| Sợ rủi ro | Hỏi lỗi, đổi trả, cam kết | Gói an tâm | Bảo hành mở rộng | Hướng dẫn, kiểm tra |
| Muốn cá nhân hoá | Hỏi theo nhu cầu riêng | Gói thiết kế riêng | Gói cao cấp | Tư vấn riêng |
| Mua để kinh doanh | Hỏi hiệu quả, lợi nhuận | Gói chuyên nghiệp | Gói hệ thống | Đào tạo, hỗ trợ, bảo trì |

→ **Mỗi ngành chỉ cần thay sản phẩm cụ thể vào bảng này.**

---

### 17. Kênh áp dụng

#### Tại CỬA HÀNG
Nhân viên phải có 3 việc:
1. Hỏi nhu cầu
2. Đưa 3 mức lựa chọn
3. Chốt món bổ trợ cần thiết

**Câu chuẩn**: "Em không hỏi anh/chị mua thêm không. Em hỏi để xem mình có đang thiếu phần nào để dùng tốt không."

#### ONLINE CHAT
**Cấu trúc tin nhắn**: "Để em tư vấn đúng, anh/chị cho em xin 3 thông tin: mục đích dùng, tần suất dùng, ngân sách dự kiến. Em sẽ ghép 3 phương án cho dễ chọn."

⚠️ Không nên gửi một đống ảnh sản phẩm rồi bắt khách tự chọn.

#### WEBSITE / SÀN TMĐT
Nên có các phần:
- "Thường mua cùng"
- "Nâng cấp lên bản tốt hơn"
- "Combo tiết kiệm hơn mua lẻ"
- "Khách mới nên chọn"
- "Gói dùng lâu dài"
- "Bảo hành/hỗ trợ thêm"

⚠️ Đừng gợi ý linh tinh. Gợi ý sai làm giảm niềm tin.

#### SAU MUA — Nhịp tin nhắn

| Thời điểm | Nội dung |
|---|---|
| Ngày 1 | Hỏi khách đã nhận/dùng chưa |
| Ngày 3 | Hỏi có vướng gì không |
| Ngày 7 | Gợi ý cách dùng tốt hơn |
| Ngày 14 | Đề xuất món nâng cấp nếu phù hợp |
| Ngày 30 | Nhắc mua lại / bảo trì / gói định kỳ |

**Mẫu tin nhắn vàng**: "Anh/chị dùng thử chưa? Nếu có điểm nào chưa ổn, gửi tôi xem. Tôi kiểm tra giúp trước khi mình phải mua thêm hay đổi món khác."
→ Tin này hay vì nó **không bán trước. Nó giúp trước.** Sau đó bán tự nhiên hơn.

---

### 18. Chỉ số CẦN ĐO

> Không đo thì hệ thống chỉ là cảm giác.

| Chỉ số | Nghĩa đơn giản | Mục tiêu |
|---|---|---|
| **AOV** | Average Order Value = giá trị đơn hàng trung bình | Tăng giá trị mỗi đơn |
| **Attach Rate** | Tỷ lệ KH mua kèm | Biết cross-sell có hiệu quả không |
| **Upsell Rate** | Tỷ lệ KH chọn gói cao hơn | Biết upsell có hiệu quả không |
| **Repeat Rate** | Tỷ lệ KH mua lại | Biết chăm sóc sau mua có tốt không |
| **CLV** | Customer Lifetime Value = giá trị vòng đời KH | Biết một KH đem lại bao nhiêu tiền dài hạn |
| **Conversion Rate** | Tỷ lệ chốt đơn | Đảm bảo bán thêm không làm rơi khách |
| **Refund/Complaint Rate** | Tỷ lệ hoàn/trả/khiếu nại | Kiểm tra có bán quá tay không |

#### Công thức đơn giản

- **AOV** = Tổng doanh thu / Số đơn hàng
  *Ví dụ: doanh thu 100tr, 100 đơn → AOV = 1tr/đơn.*
- **Attach Rate** = Số đơn có mua kèm / Tổng số đơn
  *Ví dụ: 100 đơn, 40 đơn có mua thêm phụ kiện → 40%.*
- **Upsell Rate** = Số khách chọn gói cao hơn / Tổng số khách được tư vấn
  *Ví dụ: 100 KH được tư vấn, 35 chọn gói giữa hoặc cao → 35%.*

---

### 19. 5 QUY ĐỊNH BẮT BUỘC cho nhân viên

#### 1. KHÔNG bán thêm khi chưa hỏi nhu cầu
- ❌ "Anh/chị lấy thêm cái này đi"
- ✅ "Anh/chị dùng cho mục đích gì để em xem có cần thêm không?"

#### 2. KHÔNG ép gói cao nếu khách không phù hợp
KH chỉ dùng thử mà ép gói cao là sai. KH dùng chuyên nghiệp mà khuyên bản quá rẻ cũng sai.
> **Nguyên tắc**: Không bán đắt nhất. Bán đúng nhất.

#### 3. Mỗi đơn chỉ đề xuất TỐI ĐA 2–3 món bổ trợ
Đề xuất quá nhiều làm KH ngợp. Cấu trúc tốt:
- 1 món **nên có**
- 1 món **giúp tốt hơn**
- 1 món **bảo vệ / an tâm**

#### 4. Mỗi đề xuất phải CÓ LÝ DO
- ❌ "Cái này hay lắm"
- ✅ "Cái này giúp anh/chị tránh lỗi này, tiết kiệm thời gian này, hoặc dùng bền hơn"

#### 5. Sau mua PHẢI chăm sóc
Bán xong mất hút = mất cơ hội lớn nhất.

**CRM** = Customer Relationship Management (hệ thống quản lý quan hệ KH). Dù chưa có phần mềm lớn, dùng Google Sheet cũng được. Cần lưu:
- Tên khách
- Đã mua gì
- Mục tiêu sử dụng
- Ngân sách
- Vấn đề từng gặp
- Ngày cần chăm lại
- Món nên gợi ý tiếp theo

---

### 20. MẪU BẢNG TRIỂN KHAI cho 1 sản phẩm bất kỳ

> Sếp chỉ cần thay dữ liệu ngành mình vào.

| Mục | Nội dung |
|---|---|
| Sản phẩm chính | … |
| Khách mua để làm gì? | … |
| Ai là khách mới? | … |
| Ai là khách dùng thường xuyên? | … |
| Ai là khách chuyên nghiệp? | … |
| Bản tiết kiệm | … |
| Bản cân bằng | … |
| Bản tối ưu | … |
| Món mua kèm bắt buộc | … |
| Món mua kèm nên có | … |
| Món bảo vệ/an tâm | … |
| Món mua định kỳ | … |
| Tin nhắn sau 1 ngày | … |
| Tin nhắn sau 7 ngày | … |
| Tin nhắn sau 30 ngày | … |
| Chỉ số cần đo | AOV, Attach Rate, Repeat Rate |

📎 **TPCN — anh sẽ điền sau khi chốt sản phẩm**: ví dụ "viên collagen 60 viên" → bản tiết kiệm 1 hộp / cân bằng 3 hộp + lộ trình / tối ưu 6 hộp + tư vấn 1-1 + cộng đồng VIP.

---

### 21. VÍ DỤ ÁP DỤNG ĐA NGÀNH

#### Spa / làm đẹp
| Sản phẩm chính | Upsell | Cross-sell |
|---|---|---|
| Chăm sóc da 1 buổi | Liệu trình 5–10 buổi | Sản phẩm chăm sóc tại nhà |
| Gói thường | Gói chuyên sâu | Kem chống nắng, serum, tái khám |
| Dịch vụ đơn | Membership tháng | Tư vấn da cá nhân |

> "Một buổi giúp cải thiện trước mắt. Nhưng để giữ kết quả, mình cần chăm tại nhà và theo liệu trình."

#### Giáo dục / đào tạo
| Sản phẩm chính | Upsell | Cross-sell |
|---|---|---|
| Khoá video | Khoá có sửa bài | Tài liệu, bài tập, cộng đồng |
| Khoá cơ bản | Lộ trình nâng cao | Coaching 1-1 |
| Học một kỹ năng | Học trọn lộ trình nghề | Công cụ thực hành |

> "Xem bài học giúp biết cách làm. Sửa bài mới giúp biết mình sai ở đâu."

#### Nhà hàng / cafe
| Sản phẩm chính | Upsell | Cross-sell |
|---|---|---|
| Size nhỏ | Size lớn | Topping, món phụ |
| Món đơn | Combo | Đồ uống, tráng miệng |
| Ăn một lần | Thẻ thành viên | Voucher lần sau |

> "Lấy combo này đủ bữa hơn và lợi hơn mua lẻ."

#### Thiết bị / máy móc
| Sản phẩm chính | Upsell | Cross-sell |
|---|---|---|
| Máy cơ bản | Máy công suất cao hơn | Phụ kiện, vật tư |
| Bảo hành thường | Bảo hành mở rộng | Bảo trì định kỳ |
| Mua máy | Gói lắp đặt/hướng dẫn | Đào tạo sử dụng |

> "Máy tốt mà dùng sai hoặc thiếu bảo trì thì vẫn nhanh xuống. Gói này giúp dùng ổn định hơn."

#### Phần mềm
| Sản phẩm chính | Upsell | Cross-sell |
|---|---|---|
| Gói cá nhân | Gói đội nhóm | Đào tạo sử dụng |
| Gói cơ bản | Gói chuyên nghiệp | Tích hợp hệ thống |
| Mua phần mềm | Gói **onboarding** | Hỗ trợ kỹ thuật |

**Onboarding** = hướng dẫn KH bắt đầu sử dụng đúng cách.
> "Có phần mềm chưa đủ. Đội cần được hướng dẫn để dùng đúng và tạo hiệu quả."

#### Tư vấn / doanh nghiệp
| Sản phẩm chính | Upsell | Cross-sell |
|---|---|---|
| Buổi tư vấn | Dự án triển khai | Báo cáo, đào tạo đội ngũ |
| Gói phân tích | Gói đồng hành | Theo dõi chỉ số |
| Chiến lược | Hệ thống vận hành | **SOP**, đào tạo nhân sự |

**SOP** = Standard Operating Procedure (quy trình thao tác chuẩn).
> "Tư vấn giúp thấy hướng. Triển khai mới tạo kết quả thật."

---

### 22. 5 BẪY CẦN TRÁNH

| Bẫy | Sai lầm | Sửa |
|---|---|---|
| 1. Nghĩ upsell là bán món đắt hơn | Thực ra là bán món **phù hợp hơn với mục tiêu cao hơn** | Hỏi mục tiêu trước, đề xuất theo mục tiêu |
| 2. Cross-sell quá nhiều | KH mua 1 món, NV đề xuất thêm 7 món → KH phòng thủ | Tối đa **2–3 món** thật sự liên quan |
| 3. Bán thêm bằng nỗi sợ giả | "Không mua cái này là hỏng hết" → mất niềm tin | Chỉ nói **rủi ro thật**, có lý do rõ ràng |
| 4. Giảm giá thay vì tăng giá trị | Giảm giá nhanh làm KH nghĩ giá ban đầu là ảo | Thêm: hướng dẫn, bảo hành, tư vấn, checklist, sản phẩm mẫu, ưu đãi lần sau, giao/lắp/cài đặt |
| 5. Không chăm sau mua | Bán thêm mạnh nhất xảy ra sau khi KH đã dùng và tin | Setup nhịp tin nhắn ngày 1/3/7/14/30 |

---

### 23. CÔNG THỨC CÂU NÓI CHUẨN — bộ câu vàng

> Sếp có thể dùng cho mọi ngành.

#### Câu hỏi mở đầu
> "Anh/chị mua để dùng cho mục đích gì? Tôi hỏi để tư vấn đúng, tránh mình mua thiếu hoặc mua quá tay."

#### Câu upsell
> "Bản này dùng được. Nhưng với mục tiêu của anh/chị, bản cao hơn hợp hơn vì nó bền hơn, đầy đủ hơn và ít phải nâng cấp lại."

#### Câu cross-sell
> "Món này nên đi kèm vì nó giúp anh/chị dùng sản phẩm chính hiệu quả hơn, không phải mua bổ sung nhiều lần."

#### Câu đưa 3 lựa chọn
> "Tôi tách cho anh/chị 3 mức: tiết kiệm, cân bằng và tối ưu. Với nhu cầu hiện tại, tôi khuyên mức cân bằng."

#### Câu xử lý giá cao
> "Nếu mình chỉ so giá, bản rẻ nhất luôn thắng. Nhưng nếu so theo hiệu quả sử dụng và rủi ro mua lại, bản này đáng hơn."

#### Câu tạo niềm tin
> "Tôi không khuyên anh/chị lấy bản đắt nhất. Tôi khuyên bản ít sai nhất với nhu cầu hiện tại."

#### Câu chốt combo
> "Mua lẻ vẫn được. Nhưng combo này giúp anh/chị dùng được ngay, đồng bộ hơn và tiết kiệm hơn so với mua từng phần."

#### Câu sau mua
> "Anh/chị dùng thử chưa? Có vướng điểm nào không? Tôi kiểm tra giúp để mình dùng đúng từ đầu."

---

### 24. HỆ THỐNG HOÀN CHỈNH — 6 bước vận hành

#### Bước 1: PHÂN LOẠI SẢN PHẨM
Mỗi sản phẩm/dịch vụ phải có:
- Bản thấp / giữa / cao
- Món mua kèm bắt buộc
- Món mua kèm nên có
- Món mua kèm định kỳ
- Dịch vụ hỗ trợ
- Dịch vụ bảo vệ/an tâm

#### Bước 2: PHÂN LOẠI KHÁCH (5 nhóm)

| Nhóm khách | Đặc điểm | Cách bán |
|---|---|---|
| Mới thử | Sợ sai, sợ tốn | Gói tiết kiệm, hướng dẫn rõ |
| Mới bắt đầu | Muốn dễ dùng | Gói nhập môn đầy đủ |
| Dùng thường xuyên | Cần ổn định | Gói cân bằng, mua kèm |
| Nghiêm túc | Muốn kết quả tốt | Gói nâng cấp, hỗ trợ |
| Chuyên nghiệp | Muốn hiệu suất cao | Gói tối ưu, định kỳ, ưu tiên |

#### Bước 3: THIẾT KẾ 3 GÓI
- **Gói Tiết Kiệm**: đủ dùng, giá dễ vào
- **Gói Cân Bằng**: đáng tiền nhất → **gói Sếp muốn bán nhiều nhất**
- **Gói Tối Ưu**: đầy đủ, cao cấp, tạo mốc so sánh và phục vụ KH nghiêm túc

#### Bước 4: VIẾT LUẬT ĐỀ XUẤT
- KH dùng thường xuyên → bản bền hơn
- KH sợ lỗi → hướng dẫn/bảo hành
- KH thiếu kinh nghiệm → gói có hỗ trợ
- KH mua để kinh doanh → gói chuyên nghiệp
- KH mua lần đầu → combo nhập môn
- KH mua lại lần 2 → gói định kỳ
- KH dùng gần hết chu kỳ → nhắc mua bổ sung

#### Bước 5: VIẾT KỊCH BẢN NHÂN VIÊN
Mỗi nhân viên phải thuộc:
- 5 câu hỏi chẩn đoán
- 3 câu upsell
- 3 câu cross-sell
- 3 câu xử lý từ chối
- 3 câu chăm sóc sau mua

→ **Không để nhân viên tự nói theo cảm hứng.**

#### Bước 6: ĐO SỐ LIỆU HẰNG TUẦN
Mỗi tuần kiểm tra:
- Đơn trung bình tăng hay giảm?
- Bao nhiêu KH mua kèm?
- Bao nhiêu KH chọn gói giữa/cao?
- KH có phàn nàn bị ép mua không?
- KH có quay lại không?
- Món mua kèm nào hiệu quả nhất?
- Món nào đề xuất nhiều nhưng ít ai mua?

---

### 25. KHUYẾN NGHỊ CHIẾN LƯỢC

> **Phương án tối ưu**: Không xây hệ thống upsell/cross-sell theo sản phẩm. Hãy xây theo "hành trình khách hàng".

Vì sản phẩm có thể thay đổi. Nhưng hành trình KH gần như luôn giống nhau:
1. Chưa biết rõ
2. Muốn mua thử
3. Cần dùng đúng
4. Muốn kết quả tốt hơn
5. Muốn tiết kiệm thời gian
6. Muốn an tâm
7. Muốn nâng cấp
8. Muốn duy trì
9. Muốn được ưu tiên
10. Muốn mua lại dễ hơn

→ **Ai kiểm soát được hành trình này, người đó bán thêm rất tự nhiên.**

---

### 26. MẪU HỆ THỐNG MỘT TRANG (đưa cho đội sale dùng ngay)

```
HỆ THỐNG UPSELL/CROSS-SELL CHUẨN

1. Hỏi trước khi bán
   - Mục đích dùng là gì?
   - Dùng bao lâu / tần suất thế nào?
   - Đã có gì rồi?
   - Sợ nhất điều gì?
   - Ngân sách khoảng bao nhiêu?

2. Phân loại khách
   Mới thử / Bắt đầu / Dùng thường xuyên / Nghiêm túc / Chuyên nghiệp

3. Đưa 3 lựa chọn
   Tiết kiệm / Cân bằng / Tối ưu

4. Đề xuất upsell
   Bản tốt hơn nếu khách dùng lâu, dùng nhiều, cần kết quả cao, hoặc sợ rủi ro.

5. Đề xuất cross-sell
   Món bổ trợ nếu giúp khách dùng tốt hơn, tiết kiệm thời gian, giảm lỗi,
   hoặc bảo vệ sản phẩm chính.

6. Không ép
   - Không bán món không liên quan
   - Không đề xuất quá 3 món
   - Không đẩy gói cao nếu khách không phù hợp

7. Chăm sau mua
   Ngày 1: hỏi nhận hàng/dùng chưa
   Ngày 3: hỏi có vướng không
   Ngày 7: gợi ý dùng tốt hơn
   Ngày 30: nhắc mua lại / bảo trì / nâng cấp

8. Đo số
   AOV, Attach Rate, Upsell Rate, Repeat Rate, khiếu nại
```

---

### 27. KẾT LUẬN

> **Muốn upsell/cross-sell thành công trong mọi ngành, đừng dùng mẹo vặt. Hãy xây hệ thống.**

Hệ thống đúng phải làm được 4 việc:
1. Chẩn đoán đúng nhu cầu
2. Đưa 3 mức lựa chọn rõ ràng
3. Gợi ý món bổ trợ có lý do thật
4. Chăm sóc sau mua để bán tiếp tự nhiên

**Câu định vị mạnh nhất cho mọi ngành**:
> *"Tôi không bán thêm để anh/chị chi nhiều hơn. Tôi đề xuất để anh/chị mua đúng hơn, dùng tốt hơn và ít phải sửa sai hơn."*

---

## 🛠️ HÀNH ĐỘNG SAU KHI ĐỌC

> Áp dụng vào TPCN — anh chốt khi xác định ngách.

- [ ] **Sau khi chốt sản phẩm TPCN chính**: điền MẪU BẢNG TRIỂN KHAI (mục 20) — 3 gói + món mua kèm + nhịp tin nhắn sau mua.
- [ ] **Trước khi lên ads T4**: viết bộ kịch bản 7 tình huống (mục 12) cho nhân viên CSKH — fill placeholder bằng ngôn ngữ TPCN.
- [ ] **Tạo bảng luật đề xuất** (mục 16) cho nhân viên — thay sản phẩm cụ thể vào.
- [ ] **Thiết kế membership / gói định kỳ TPCN**: TPCN là ngành tiêu hao chu kỳ — đây là đòn bẩy CLV lớn nhất.
- [ ] **Setup tracking 7 chỉ số** (mục 18): AOV, Attach Rate, Upsell Rate, Repeat Rate, CLV, Conversion Rate, Refund Rate.
- [ ] **Nhịp tin nhắn sau mua**: tạo automation gửi tin ngày 1/3/7/14/30 (qua Zalo OA + email — phối với [[Khối 8 - MXH khác Zalo]] và [[Khối 12 - Email marketing]]).

## 🔗 Liên kết

- 🎯 Khối liền kề: [[Khối 15 - Sale Page]] (sale page bán món chính trước khi cross-sell) · [[Khối 17 - Trả lời tin nhắn]] (kịch bản inbox áp dụng 5 câu chẩn đoán) · [[Khối 12 - Email marketing]] (chăm sau mua qua email).
- 🧭 [[Khối 19 - Luồng khách hàng]] — Upsell/Cross-sell = Điểm chạm 10 (Chăm sóc sau mua).
- 📚 Source gốc: [[raw/Đặc sản của Phạm Thành Long/IPS - 19 khối công việc/16_ Upsell_Cross-sell]]
- 👤 Mentor: [[Phạm Thành Long]]
