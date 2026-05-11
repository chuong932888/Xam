---
type: concept
tags: [ads, policy, health, ymyl, tpcn, meta, ips, khoi-14]
created: 2026-05-09
updated: 2026-05-09
sources: ["[[Khối 14a - ADS Facebook]]", "[[Khối 14f - Từ cấm FB Ads (cảnh báo nhân viên)]]"]
---

# Chính sách Health/YMYL cho TPCN trên ads platform

> ⚠️ **TPCN ƯU TIÊN ĐỌC TRƯỚC KHI VIẾT CREATIVE ĐẦU TIÊN.**

> 🚨 **Sửa sau QA round 2 — phân biệt 2 chính sách KHÔNG được nhầm**:
> - **Special Ad Category (Meta)** chỉ gồm 4 nhóm: **Credit, Employment, Housing, Social Issues/Elections**. **Health/TPCN KHÔNG nằm trong Special Ad Category.**
> - **TPCN/Health** chịu **chính sách RIÊNG của Meta** (Personal Health Ads, Drugs & Pharmaceuticals, Sensational Content) + **YMYL guidelines (Google)** — cũng nghiêm nhưng KHÁC mechanism với Special Ad Category.

> **Định nghĩa các chính sách động chạm TPCN** *(theo PTL — Khối 14a dòng 224 + bổ sung em sửa sau QA)*:
> - **Personal Health Ads policy (Meta)**: cấm gợi nhắc personal attributes, before/after, ngụ ý chữa bệnh.
> - **Drugs & Pharmaceuticals (Meta)**: TPCN tuy không phải thuốc nhưng dễ bị flag chung nhóm.
> - **Sensational Content (Meta)**: cấm "shocking" claims.
> - **YMYL (Google)**: yêu cầu E-E-A-T cao trên landing page.
> - **Healthcare/Pharma market rule (TikTok)**: rule riêng từng quốc gia, VN nghiêm.

## 🚨 Vì sao TPCN khó hơn ngành thường

### Tại Meta
1. **Personal Health Ads policy** — cấm gợi nhắc personal attributes ("Bạn đang béo?", "Bạn bị mụn?") → tự động flag.
2. **Before/after photos** → bị từ chối hoặc giảm phân phối mạnh.
3. **Cấm ngụ ý chữa bệnh** → vi phạm policy Drugs & Pharmaceuticals.
4. **Sensational content policy** → cấm shocking claims ("Phương pháp thần kỳ", "Khỏi 100%").

⚠️ **TPCN KHÔNG nằm trong Special Ad Category** (chỉ Credit, Employment, Housing, Social Issues nằm trong đó). Nhưng TPCN vẫn bị **kiểm duyệt nghiêm** thông qua các policy riêng nói trên.

### Tại Google
1. **YMYL** (Your Money or Your Life) — Google áp **Quality Rater Guidelines** nghiêm hơn.
2. **Landing page yêu cầu E-E-A-T cao** — tác giả thật, chuyên gia, citation.
3. **Cấm/hạn chế** một số keyword TPCN trong Search Ads.

### Tại TikTok
1. **Healthcare/pharma có market rule riêng** ở từng quốc gia (gốc 14c dòng 263).
2. **Việt Nam**: ad/landing page bằng tiếng Việt + **disclaimer ngành bắt buộc ở ngôn ngữ địa phương**.

### Tại Việt Nam (pháp lý — KHÔNG có trong PTL gốc, em thêm)

3 luồng pháp lý động chạm:

1. **Luật Quảng cáo 16/2012/QH13 + Nghị định 38/2021**:
   - Cấm quảng cáo TPCN gây hiểu nhầm là thuốc chữa bệnh.
   - Bắt buộc xác nhận nội dung quảng cáo bởi **Cục An toàn thực phẩm** trước khi chạy.
   - Phạt 60-80 triệu/lần vi phạm.

2. **Luật ATVSTP 55/2010 + Nghị định 15/2018**:
   - TPCN bắt buộc công bố sản phẩm trước khi quảng cáo.

3. **Nghị định 147/2024/NĐ-CP** (hiệu lực 25/12/2024):
   - Tài khoản MXH bắt buộc xác thực số ĐT VN.
   - Acc clone/via để chạy ads = vi phạm.

## 📋 Checklist policy compliance — TPCN

> Đọc CHECKLIST này TRƯỚC khi launch creative đầu tiên.

### A. Tài khoản & Setup

- [ ] BM/Business Center đã verify business + verify domain.
- [ ] Tất cả admin có 2FA.
- [ ] Domain + Page + ad + LP cùng câu chuyện.
- [ ] Lịch sử thanh toán sạch.
- [ ] Account Quality không có warning.
- [ ] Đã chấp nhận Lead Ads Terms (nếu chạy lead form).

### B. Pháp lý VN (BẮT BUỘC)

- [ ] **Có giấy công bố sản phẩm** (Cục ATTP).
- [ ] **Xác nhận nội dung quảng cáo** từ Cục ATTP/Bộ Y tế **TRƯỚC khi chạy**.
- [ ] **Disclaimer hiển thị**: "Sản phẩm này không phải là thuốc, không có tác dụng thay thế thuốc chữa bệnh."
- [ ] **Số đăng ký Cục ATTP** hiển thị trên trang sản phẩm.
- [ ] **Giấy phép kinh doanh** hiển thị footer.
- [ ] Tài khoản MXH đã xác thực số ĐT VN (Nghị định 147/2024).

### C. Creative content

- [ ] **KHÔNG** dùng từ trong [[Khối 14f - Từ cấm FB Ads (cảnh báo nhân viên)]] (9 nhóm).
- [ ] **KHÔNG** chạm "personal attributes" (béo, mụn, bệnh, lão hoá).
- [ ] **KHÔNG** before/after photo gây hiểu nhầm.
- [ ] **KHÔNG** cam kết hiệu quả tuyệt đối ("100%", "đảm bảo", "chữa khỏi").
- [ ] **KHÔNG** ngụ ý chữa bệnh ("thuốc trị X", "khỏi bệnh Y").
- [ ] **CÓ** disclaimer "không phải là thuốc..." trên ad + landing page.

### D. Author + E-E-A-T (Google YMYL)

- [ ] Tác giả LP là **bác sĩ/chuyên gia thật** có hồ sơ.
- [ ] Author Box đầy đủ: ảnh, tên, chức danh, link LinkedIn/bệnh viện.
- [ ] Schema Article + Person markup.
- [ ] Citation từ nguồn chính phủ/báo cáo y tế (KHÔNG tự bịa số liệu).

### E. Landing Page

- [ ] PageSpeed mobile ≥80, ≤2.5s.
- [ ] Mobile-friendly.
- [ ] HTTPS.
- [ ] Privacy policy + Terms of Service hiển thị footer.
- [ ] Khớp thông điệp ad ↔ landing page.

## 🎯 Audience selection cho TPCN (KHÔNG phải Special Ad Category)

> 🚨 **Sửa sau QA round 2**: TPCN KHÔNG bị áp **Special Ad Category restrictions** (4 nhóm: Credit/Employment/Housing/Social Issues). Nhưng vẫn nên thận trọng với targeting để giảm rủi ro flag content policy.

📎 *Em đề xuất — phù hợp với best practice industry, không phải PTL gốc liệt kê*:

| Loại targeting | TPCN dùng | Ghi chú |
|---|---|---|
| Detailed targeting | ⚠️ Cẩn thận | Một số interest "Health" có thể trigger reviewer chặt hơn |
| Custom audience | ✅ Được | Customer list, website visitors *(consent đầy đủ + không tiết lộ tình trạng sức khoẻ cá nhân)* |
| Lookalike | ✅ Được | LAL 1-3% từ Purchaser hoặc High-value customer |
| Geo targeting | ✅ Được | Country/region/city OK |
| Age + Gender | ✅ Được | Health vẫn target được, KHÁC với Credit/Employment/Housing |
| Broad / Advantage+ | ✅ Khuyến nghị | Khi creative đủ tốt |

## 🎯 Pattern an toàn — Cách viết creative TPCN white-hat

### 5 nguyên tắc viết content

1. **Dùng "hỗ trợ", "góp phần"** thay vì "chữa", "đảm bảo".
2. **Mô tả tình trạng KHÔNG nhắc bệnh**: "khi cảm thấy mệt mỏi" thay vì "bệnh suy nhược thần kinh".
3. **Disclaimer cuối ad + landing page**.
4. **Bác sĩ chuyên môn xuất hiện** (tăng E-E-A-T).
5. **Citation từ nguồn chính phủ** khi có claim sức khoẻ.

### Bảng thay thế từ rủi ro

| Từ rủi ro | Thay bằng (white-hat) |
|---|---|
| "Chữa bệnh X" | "Hỗ trợ tình trạng X" hoặc "Người dùng có vấn đề X chia sẻ..." |
| "Cam kết 100%" | "Nhiều khách hàng đã phản hồi tích cực sau N tuần sử dụng" |
| "Trị mụn" | "Hỗ trợ làn da khoẻ mạnh" |
| "Giảm cân thần tốc" | "Hỗ trợ kiểm soát vóc dáng kết hợp chế độ ăn + tập luyện" |
| "Bạn đang béo phì?" | "Bạn quan tâm đến lối sống lành mạnh?" |
| "Thực phẩm chức năng" | "Sản phẩm bổ sung dinh dưỡng" *(tuỳ ngữ cảnh)* |

⚠️ Pattern thay thế là **suy luận white-hat**. Trước launch phải có **luật sư + Cục ATTP duyệt**.

## 🚨 Hậu quả vi phạm

### Meta
- Lần 1: ad bị từ chối, có thể appeal.
- Lần 2-3: BM/ad account bị warning.
- Nhiều lần / nghiêm trọng: **disable BM vĩnh viễn** → mất hết learning Pixel + audience.

### Google
- Vi phạm policy: ad disabled.
- Site spam → toàn site bị penalize SEO + bị remove khỏi Shopping/PMax.

### Việt Nam (pháp lý)
- Vi phạm Luật QC 16/2012: phạt **60-80 triệu/lần**.
- Quảng cáo TPCN sai → **thu hồi giấy công bố sản phẩm**.
- Nghiêm trọng → **đình chỉ kinh doanh**.

## 🎯 Hành động cho team ads TPCN

> Đẩy vào [[../../actions|actions.md]].

1. **Trước launch creative đầu tiên** (T4):
   - ☐ Luật sư review pháp lý compliance toàn bộ funnel.
   - ☐ Xin xác nhận nội dung quảng cáo từ Cục ATTP cho 3-5 creative core.
   - ☐ Verify mọi tài khoản MXH có xác thực số ĐT VN.

2. **Mọi creative + landing page**: qua **2 vòng QA**:
   - Vòng 1: kiểm 9 nhóm từ cấm + checklist policy.
   - Vòng 2: legal/compliance check.

3. **Onboarding nhân viên ads mới**: đọc bắt buộc:
   - Page này.
   - [[Khối 14f - Từ cấm FB Ads (cảnh báo nhân viên)]].
   - Luật QC 16/2012 + Nghị định 38/2021.

4. **Monitor hàng tháng**:
   - Account Quality (Meta).
   - Status creative bị từ chối → root cause analysis.
   - Cập nhật Meta Advertising Standards mới nhất.

## 🔗 Liên quan

- [[Khối 14f - Từ cấm FB Ads (cảnh báo nhân viên)]] — checklist 9 nhóm từ tránh
- [[Khối 14a - ADS Facebook]] — phần 6 chính sách Meta
- [[Khối 14c - ADS TikTok]] — phần 8 healthcare/pharma market rule
- [[E-E-A-T]] — bác sĩ chuyên môn = xương sống YMYL
- [[Khối 9 - SEO Blog 2026]] — TPCN = YMYL
