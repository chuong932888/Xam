---
type: source
tags: [ips, khoi-12, email, marketing, retention, ptl, copywriting, automation, deliverability]
created: 2026-05-09
updated: 2026-05-09
sources: ["[[raw/Đặc sản của Phạm Thành Long/IPS - 19 khối công việc/12_ Email marketing.docx]]"]
khoi: 12
---

# Khối 12 — Email Marketing

> Nguồn gốc: IPS của Phạm Thành Long — tài liệu gốc 281 đoạn văn + 10 bảng.

---

## TL;DR

Email marketing là kênh **kéo khách từ hộp thư về landing page** — không phải nơi bán hàng trực tiếp. Hiệu quả phụ thuộc vào 3 yếu tố: hạ tầng kỹ thuật (domain reputation), chất lượng danh sách (ai trong list), và copywriting (tiêu đề + nội dung). Tài liệu chia làm 2 phần: Phần A — vận hành thực tế (10 chương); Phần B — lộ trình 12 tháng từ người mới lên chuyên gia.

---

## PHẦN A: TÀI LIỆU VẬN HÀNH

### Chương 1 — Tư duy gốc

**3 nguyên lý cốt lõi:**

**Nguyên lý 1 — Email là "được duyệt vào", không phải "gửi đi"**
Mỗi email bị Gmail/Outlook chấm điểm và đưa vào: Hộp chính / Quảng cáo / Spam / Chặn.

**Nguyên lý 2 — 3 trụ cột quyết định email vào đâu** (bảng gốc):

| Trụ cột | Trọng số | Nội dung |
|---|---|---|
| Kỹ thuật | 30% | SPF, DKIM, DMARC, IP/domain reputation |
| Hành vi danh sách | 50% | Mở, click, báo spam, hủy đăng ký |
| Nội dung | 20% | Tiêu đề, từ khóa, tỉ lệ chữ/hình |

**Nguyên lý 3 — Email là chiếc cầu, không phải nơi bán**
- Mục tiêu của email: dẫn người đọc tới trang bán hàng (landing page).
- Đừng cố bán hết trong email. Email chỉ làm 1 việc: **tạo cú click**.
- Tập trung quá vào "viết thư hay" → trang bán hàng sẽ vắng người.

---

### Chương 2 — Hạ tầng kỹ thuật (làm 1 lần, hưởng mãi)

#### 2.1. Domain & Email gửi
- Dùng **domain riêng cho marketing** (ví dụ: `mail.congtyban.com` hoặc `news.congtyban.com`).
- Không dùng `@gmail.com`, `@yahoo.com` để gửi marketing.
- Friendly From dạng: `Chương từ TattooX <chuong@tattoox.com>`. Email "no-reply" giảm 30% open rate.

#### 2.2. Xác thực domain (BẮT BUỘC)
- **SPF**: Khai báo máy chủ nào được gửi với danh nghĩa domain.
- **DKIM**: Chữ ký số trên mỗi email.
- **DMARC**: Quy tắc xử lý email không xác thực.
- **BIMI**: Hiện logo trong Gmail (cần DMARC enforcement). Tăng open rate 10–15%.
- **rDNS (Reverse DNS)**: IP gửi tra ngược ra đúng domain.
- Kiểm tra tại `mxtoolbox.com` — cả 4 bản ghi phải xanh.

#### 2.3. Công cụ giám sát miễn phí
- **Google Postmaster Tools** (`postmaster.google.com`): Xem điểm uy tín domain với Gmail.
- **Microsoft SNDS**: Xem điểm với Outlook/Hotmail.
- **MXToolbox Blacklist Monitor**: Báo động khi domain/IP bị blacklist.

---

### Chương 3 — Danh sách sạch

#### 3.1. Cách thu email
- **CHỈ** thu từ người tự đăng ký (opt-in). Không mua, không xin, không scrape.
- Bật **Double Opt-in** trên TẤT CẢ form.
- Mỗi nguồn thu phải có **Lead Magnet** rõ ràng (ebook, video, checklist, voucher).
- Form ghi rõ: "Bạn sẽ nhận X email/tuần về Y. Có thể hủy bất kỳ lúc nào."

#### 3.2. Phân nhóm danh sách (segmentation)
- Theo **nguồn**: Form / FB ads / Hội thảo / Đã mua…
- Theo **hành vi**: Đã mở 5 email gần nhất / Không mở 30 ngày / Click sản phẩm A…
- Theo **vòng đời**: Khách mới (<7 ngày) / Đang nuôi dưỡng (7–30 ngày) / Đã mua / Cũ không hoạt động.

#### 3.3. Vệ sinh danh sách
- Mỗi tháng: Xóa **hard bounce**.
- Mỗi 3 tháng: **Re-engagement** cho người 60 ngày không mở. Sau chiến dịch, ai vẫn không phản hồi → xóa.
- Mỗi 6 tháng: Dùng **NeverBounce/ZeroBounce** để lọc email "chết".
- Bẫy thường gặp: Tiếc giữ list to. **1.000 email tương tác > 10.000 email "chết".**

---

### Chương 4 — Warm-up Domain mới

Bảng lịch warm-up (từ file gốc):

| Tuần | Số email/ngày | Đối tượng | Mục tiêu |
|---|---|---|---|
| 1 | 20–50 | Nhóm tương tác cao nhất | Open >50% |
| 2 | 50–100 | Nhóm tương tác trung bình | Open >40% |
| 3 | 100–500 | Mở rộng tiếp | Open >30% |
| 4 | 500–2.000 | Toàn list hoạt động | Open >25% |
| 5+ | Tăng gấp đôi/tuần | Toàn list | Theo dõi chặt KPI |

**Quy tắc vàng**: Không tăng quá 100% so với tuần trước. Open <20% → dừng tăng, giữ mức cũ thêm 1 tuần.

---

### Chương 5 — Tiêu đề & Preheader (CHƯƠNG QUAN TRỌNG NHẤT)

**Tiêu đề + Preheader quyết định 47% việc email được mở.**

#### 5.1. Quy tắc độ dài (bảng gốc)

| Vị trí | Độ dài tối ưu | Ghi chú |
|---|---|---|
| Máy tính (Gmail/Outlook) | 41–50 ký tự | Hiển thị đầy đủ |
| Điện thoại (33 ký tự đầu) | Phần quan trọng nhất | iPhone ~40, Gmail Android 33 |
| Tổng tối đa | ≤ 60 ký tự | Vượt là bị cắt trên hầu hết thiết bị |
| Preheader | 37–90 ký tự | Bổ sung tiêu đề, KHÔNG lặp lại |

**Quy tắc front-loading**: Đặt từ khóa quan trọng nhất trong **33 ký tự đầu**. Sau 33 ký tự coi như mất.

#### 5.2. Năm công thức tiêu đề "ăn khách"

**Công thức 1: KHẨN CẤP + BỐI CẢNH**
Tâm lý: FOMO (Fear Of Missing Out) + cho hiểu vì sao mình nhận email này.
Mẫu:
- "Ối, tôi nhập nhiều hàng quá – phải bán rẻ thôi"
- "Cái này đóng lúc 12h đêm Chương ơi"
- "Còn 3 suất cuối, bạn có muốn không?"
- "Phải gửi gấp – kẻo quên"

**Công thức 2: TÒ MÒ + CÂU CHUYỆN (Curiosity Gap)**
Tâm lý: Information Gap — não con người bị ép buộc phải lấp khoảng trống nhận thức. Đưa câu hỏi, KHÔNG đưa câu trả lời.
Mẫu:
- "Cái này rất xấu hổ…"
- "Suýt nữa thì tôi quên gửi email này…"
- "Bạn đã có cái này chưa?"
- "Bạn có thấy cái quầng mắt ở dưới mắt mình không?"
- "Chương ơi, bạn đã xem cái này chưa?"

**Công thức 3: VẤN ĐỀ + GIẢI PHÁP**
Tâm lý: Đập đúng nỗi đau + hứa hẹn.
Mẫu:
- "Tỉ lệ mở email của bạn đã được khắc phục"
- "Hết đau lưng sau 3 ngày – cách tôi làm"
- "Bán không ai mua? Đây là lý do thật"

**Công thức 4: PHÁ VỠ KHUÔN MẪU (Pattern Interrupt)**
Tâm lý: Não bộ chú ý đến điều BẤT THƯỜNG, bỏ qua điều quen thuộc.
Mẫu:
- "Đây là email tôi viết cho bạn – nhưng tôi không muốn bạn mở nó"
- "Đây là bức thư bán hàng, và tôi muốn bạn mở nó"
- "Tôi đã sai – và cần xin lỗi bạn"

**Công thức 5: SỐ + LỢI ÍCH**
Số gây cảm giác cụ thể, dễ tin. Số lẻ (3, 5, 7, 11) hiệu quả hơn số chẵn.
Mẫu:
- "5 lỗi giết chết doanh nghiệp nhỏ"
- "Tôi mất 47 triệu vì sai lầm này"
- "3 phút đọc – thay đổi 3 năm tới"

#### 5.3. Từ ngữ NÊN dùng trong tiêu đề (bảng gốc)

| Loại từ | Ví dụ |
|---|---|
| Tò mò nhẹ | "Hỏi nhanh", "Bạn có biết…" |
| Thân mật | "Dành riêng cho bạn", "Chương ơi…" |
| Bí mật | "Bí mật", "Sự thật là…" |
| Tin tức | "Tin nóng", "Tin mới", "Cập nhật" |
| Cảnh báo | "Sai lầm", "Cảnh báo", "Đừng làm…" |
| Phủ định | "Bạn không tin được đâu" |

#### 5.4. Từ ngữ TUYỆT ĐỐI TRÁNH (kích hoạt spam filter)
- "MIỄN PHÍ", "FREE"
- "BẤM VÀO ĐÂY", "CLICK NGAY"
- "CHIẾN THẮNG", "TRÚNG THƯỞNG"
- "MUA HÀNG", "ĐẶT HÀNG", "ĐẶT NGAY"
- "GIẢM 90%", "$$$"
- "ĐẢM BẢO 100%", "TRIỆU PHÚ"
- VIẾT HOA TOÀN BỘ
- !!!!!!! (nhiều dấu chấm than)

#### 5.5. Emoji — sự thật khoa học (từ file gốc)

> Gốc ghi rõ: "Ý kiến của bạn: Không dùng icon" — sau đó phản bác bằng thực tế khoa học.

- Trong bán lẻ, lifestyle, B2C: 1–2 emoji có thể **TĂNG open rate 5–15%**.
- Trong B2B, tài chính, pháp lý, y tế: Emoji **GIẢM uy tín**, giảm open rate.
- Dùng quá 2 emoji: luôn giảm hiệu quả và dễ vào spam.
- Emoji bị Gmail tính là **2 ký tự** khi đếm độ dài.
- Lời khuyên: Nếu ngành B2C/bán lẻ — test 1 emoji ở đầu hoặc cuối. Nếu là B2B — không dùng.

#### 5.6. Preheader (đừng bỏ trống)
- KHÔNG để trống — Gmail sẽ lấy dòng đầu của email body làm preheader, thường rất xấu.
- KHÔNG lặp lại tiêu đề — lãng phí "bất động sản" thứ 2.
- Ví dụ bổ sung đúng cách:
  - Tiêu đề: "Cái này đóng lúc 12h đêm"
  - Preheader: "Khóa học 9 ngày để xây chuỗi email tự bán hàng. Còn 7 suất."

---

### Chương 6 — Nội dung Email (Cách viết)

#### 6.1. Nguyên tắc viết
- Đừng bắt đầu bằng "Xin chào" — nhảy thẳng vào câu chuyện.
- Viết cho **1 người cụ thể**, không viết cho đám đông. Tưởng tượng đang nói chuyện với 1 khách cụ thể bạn biết.
- Bán sự **BIẾN ĐỔI**, không bán tính năng.
  - Sai: "Khóa học có 12 video, 5 bài tập, 3 buổi live."
  - Đúng: "Sau 9 ngày, bạn có chuỗi email tự gửi mỗi tuần và bán hàng cho bạn ngay cả khi đang ngủ."
- **1 email = 1 mục đích = 1 CTA duy nhất.** Cho người đọc 3 lựa chọn → họ không chọn cái nào.

#### 6.2. Cấu trúc 1 email — Framework PAS (bảng gốc)

PAS = Problem – Agitate – Solution (Vấn đề – Khoét sâu – Giải pháp). Đây là framework hiệu quả nhất cho email bán hàng.

| Phần | Nội dung | Độ dài |
|---|---|---|
| Hook (mồi câu) | Câu mở đầu đánh trúng cảm xúc | 1–2 câu |
| Problem | Gọi tên vấn đề người đọc đang gặp | 2–4 câu |
| Agitate | Khoét sâu nỗi đau – cho thấy hậu quả nếu không sửa | 3–5 câu |
| Story/Bridge | Câu chuyện cá nhân hoặc case study | 1 đoạn |
| Solution | Giới thiệu giải pháp ngắn gọn | 2–3 câu |
| CTA | Lời kêu gọi hành động duy nhất | 1 câu + 1 nút |

#### 6.3. Bốn framework copywriting nâng cao

**Framework 1: PAS (Problem – Agitate – Solution)**
Khi dùng: Email bán hàng, sales page.
Ví dụ:
- P: "Bạn gửi email mà không ai mở?"
- A: "Mỗi email không mở là 1 khách hàng tuột mất. 1 năm 50 email × 5.000 người = 250.000 cơ hội bị bỏ phí."
- S: "Khóa học 9 ngày dạy bạn viết tiêu đề đạt open rate 40%."

**Framework 2: AIDA (Attention – Interest – Desire – Action)**
Khi dùng: Email cho khách mới, chưa biết gì về bạn.
- A: Tiêu đề gây sốc.
- I: Câu chuyện liên quan tới họ.
- D: Cho thấy "trước–sau" khi dùng giải pháp.
- A: CTA rõ ràng.

**Framework 3: BAB (Before – After – Bridge)**
Khi dùng: Email kể chuyện thành công, case study.
- Before: "Cách đây 6 tháng, tôi gửi email cho 3.000 người, chỉ 50 người mở."
- After: "Bây giờ, tôi gửi cho 800 người, 320 người mở, 24 người mua."
- Bridge: "Tôi đã làm 3 việc khác đi, đây là việc đầu tiên…"

**Framework 4: Star – Story – Solution**
Khi dùng: Email kết nối cảm xúc, xây dựng thương hiệu cá nhân.
- Star: Giới thiệu nhân vật chính (có thể là bạn, là khách hàng).
- Story: Hành trình của họ.
- Solution: Giải pháp giúp họ thoát khỏi vấn đề.

#### 6.4. Checklist kỹ thuật khi soạn 1 email

**Tiêu đề:**
- 41–50 ký tự (máy tính), từ khóa quan trọng trong 33 ký tự đầu.
- Không VIẾT HOA toàn bộ, không nhiều !!!.
- Tránh từ kích hoạt spam.
- Test 2 phiên bản (A/B test).

**Preheader:**
- 37–90 ký tự, bổ sung tiêu đề, không lặp lại.

**Thân email:**
- Mở đầu bằng câu chuyện, không bằng "Xin chào".
- Tỉ lệ chữ/hình ≥ 80/20.
- 200–500 từ (nuôi dưỡng) hoặc 500–800 từ (bán hàng).
- 1 CTA chính (có thể nhắc lại 2 lần trong cùng email nếu dài).
- CTA dạng nút nổi bật, không chỉ link chữ.
- Không dùng link rút gọn (bit.ly).

**Footer:**
- Tên công ty + Địa chỉ thật.
- Link Hủy đăng ký rõ ràng.
- Lý do người nhận có trong list.

**Kỹ thuật:**
- Dung lượng < 100KB.
- Có phiên bản plain text song song HTML.
- Alt text cho mọi hình ảnh.
- Test trên Gmail / Outlook / iPhone Mail / Yahoo.

---

### Chương 7 — Chuỗi 14 ngày (3 giai đoạn)

> Lưu ý từ file gốc: đây chỉ là chuỗi tham khảo. Có thể thêm email nhắc nhở sau các email quan trọng.

**Giai đoạn 1 — LÀM QUEN (Ngày 1–3):**

| Ngày | Loại | Mục đích | Open kỳ vọng |
|---|---|---|---|
| 1 | Giao Lead Magnet | Trao giá trị đã hứa | 60–80% |
| 2 | Câu chuyện cá nhân | Kết nối cảm xúc | 40–50% |
| 3 | Gọi tên vấn đề | Khẳng định bạn hiểu họ | 35–45% |

**Giai đoạn 2 — NUÔI DƯỠNG (Ngày 4–10):**

| Ngày | Loại | Framework gợi ý |
|---|---|---|
| 4 | Phá hiểu lầm #1 | PAS |
| 6 | Phá hiểu lầm #2 | PAS |
| 8 | Case study nhỏ | BAB |
| 10 | Mở lộ trình | Star–Story–Solution |

**Giai đoạn 3 — BÁN (Ngày 11–14):**

| Ngày | Loại | Framework gợi ý |
|---|---|---|
| 11 | Giới thiệu giải pháp | AIDA |
| 12 | Xử lý phản đối | PAS |
| 13 | Câu chuyện quyết định | BAB |
| 14 | Lời mời cuối | AIDA + FOMO |

---

### Chương 8 — Lịch gửi & Tần suất

- Tần suất: **2–3 email/tuần** là tối ưu.
- Khung giờ: **8h–10h sáng** hoặc **19h–21h tối**.
- Ngày tốt: Thứ 3, 4, 5. Tránh thứ 2 và cuối tuần.
- Nhất quán: Cam kết gì giữ vững.
- Không gửi >10.000 email cùng lúc. Chia làm nhiều đợt cách **30 phút**.

---

### Chương 9 — Đo lường & KPI

**Bảng ngưỡng KPI (từ file gốc):**

| Chỉ số | Tốt | Cảnh báo | Nguy hiểm |
|---|---|---|---|
| Open rate | 25–40% | 15–25% | < 15% |
| Click rate | 3–8% | 1–3% | < 1% |
| Bounce rate | < 2% | 2–5% | > 5% |
| Unsubscribe | < 0.5% | 0.5–1% | > 1% |
| Spam complaint | < 0.1% | 0.1–0.3% | > 0.3% — DỪNG NGAY |
| Inbox placement | > 90% | 70–90% | < 70% |

**Công cụ đo lường:**
- `Mail-tester.com` — test điểm spam (≥ 8/10 mới gửi).
- **Google Postmaster Tools** — điểm uy tín Gmail.
- **GlockApps** — test inbox placement.
- **MXToolbox** — kiểm tra blacklist.

---

### Chương 10 — Kịch bản khủng hoảng

**Dấu hiệu**: Open tụt >30%, spam complaint >0.3%, Postmaster báo "Low".

**7 bước xử lý (từ file gốc):**
1. DỪNG mọi chiến dịch đại trà.
2. Kiểm tra blacklist tại MXToolbox.
3. Xem Google Postmaster Tools.
4. Phân tích chiến dịch gần nhất — tiêu đề, nội dung, list.
5. Chỉ gửi cho "list vàng" (tương tác trong 30 ngày).
6. Quay lại quy trình warm-up.
7. Sau 3–4 tuần điểm tốt mới mở rộng.

---

## PHẦN B: LỘ TRÌNH TỪ NGƯỜI MỚI THÀNH CHUYÊN GIA

> Phần này tổng hợp từ CXL, ANA, HubSpot, Google (ghi chú trong file gốc).

### 9 kỹ năng cốt lõi

**Cấp độ 1 — NỀN TẢNG (1–3 tháng đầu):**

**Kỹ năng 1: Email Copywriting**
- Viết tiêu đề ăn khách (5 công thức ở Chương 5).
- Viết thân email theo framework (PAS, AIDA, BAB, Star–Story–Solution).
- A/B test tiêu đề và CTA.
- Bài tập (từ file gốc): Viết 30 tiêu đề/ngày trong 30 ngày, test 5 tiêu đề/tuần.

**Kỹ năng 2: Hiểu hạ tầng kỹ thuật**
- Cấu hình SPF, DKIM, DMARC, BIMI.
- Đọc Google Postmaster Tools.
- Xử lý blacklist.
- Bài tập: Tự cấu hình từ A–Z cho 1 domain mới.

**Kỹ năng 3: Quản lý danh sách (List Hygiene)**
- Double opt-in.
- Phân nhóm cơ bản (theo nguồn, hành vi).
- Vệ sinh định kỳ.
- Bài tập: Dọn 1 list cũ — đo open rate trước và sau.

**Cấp độ 2 — TRUNG CẤP (3–6 tháng):**

**Kỹ năng 4: Email Automation (Tự động hóa)**
- Welcome series (chuỗi chào mừng).
- Cart abandonment (giỏ hàng bỏ quên).
- Re-engagement (kích hoạt lại khách cũ).
- Behavioral triggers (kích hoạt theo hành vi: mở/click/mua).
- Công cụ: Mailchimp, ActiveCampaign, GetResponse, Klaviyo.
- Bài tập: Xây 1 chuỗi welcome 5 email tự động chạy.

**Kỹ năng 5: Advanced Segmentation (Phân nhóm nâng cao)**
- Behavioral segmentation: phân theo hành vi mua (RFM — Recency, Frequency, Monetary).
- Predictive segmentation: dùng AI dự đoán ai sắp mua.
- Lifecycle segmentation: phân theo giai đoạn vòng đời khách.
- Bài tập: Phân list 1 doanh nghiệp thành 8 nhóm khác nhau, gửi nội dung khác nhau, đo doanh thu.

**Kỹ năng 6: Phân tích dữ liệu**
- Đọc và hiểu các chỉ số: Open, Click, Conversion, Revenue per email, Customer Lifetime Value.
- Hiểu cohort analysis (phân tích nhóm khách theo thời gian).
- A/B test có ý nghĩa thống kê.
- Bài tập: Phân tích 30 chiến dịch gần nhất, viết báo cáo "3 việc nên làm khác đi".

**Cấp độ 3 — NÂNG CAO (6–12 tháng):**

**Kỹ năng 7: Lifecycle Email Marketing**
- Hiểu hành trình khách hàng (Customer Journey).
- Thiết kế email theo từng giai đoạn: Awareness → Consideration → Purchase → Retention → Advocacy.
- Xây "email engine" tự bán hàng 24/7.

**Kỹ năng 8: Tích hợp đa kênh (Omnichannel)**
- Tích hợp email với SMS, push notification, retargeting ads.
- Đồng bộ với CRM (HubSpot, Salesforce).
- Đo lường ROI tổng (không chỉ ROI riêng email).

**Kỹ năng 9: Pháp lý & Tuân thủ**
- CAN-SPAM (Mỹ).
- GDPR (Châu Âu).
- Luật Việt Nam: Nghị định 91/2020 về chống thư rác.
- Quan trọng cho VN: Phải có cơ chế đăng ký rõ ràng và link hủy. Nếu không, phạt từ **10–80 triệu/lần vi phạm**.

---

### Lộ trình học 12 tháng (bảng gốc)

| Tháng | Trọng tâm | Việc làm | Cách đo thành công |
|---|---|---|---|
| 1 | Hạ tầng kỹ thuật | Cấu hình SPF/DKIM/DMARC, đăng ký Postmaster | Mail-tester ≥ 8/10 |
| 2 | Copywriting cơ bản | Viết 100 tiêu đề, học 4 framework | A/B test có kết quả rõ |
| 3 | Chuỗi 14 ngày | Xây chuỗi nuôi dưỡng đầu tiên | Open ≥ 30%, click ≥ 5% |
| 4 | List building | Lead magnet + form double opt-in | Thu 100 email/tháng |
| 5 | Segmentation | Phân list thành 5 nhóm | Open của nhóm phân khúc cao hơn 20% |
| 6 | Automation cơ bản | Welcome series + abandoned cart | 30% doanh số đến từ automation |
| 7 | Phân tích dữ liệu | Đọc cohort, RFM | Viết được báo cáo tháng |
| 8 | A/B testing nâng cao | Test tiêu đề, CTA, thời gian gửi | Tăng open 10% so với baseline |
| 9 | Tích hợp đa kênh | Đồng bộ email + SMS + retargeting | ROI tăng 30% |
| 10 | Lifecycle marketing | Bản đồ hành trình khách hàng đầy đủ | LTV tăng 25% |
| 11 | Pháp lý & deliverability | Tuân thủ luật, fix mọi lỗi spam | Inbox placement >95% |
| 12 | Chuyên môn hóa | Chọn 1 ngành/thị trường để chuyên sâu | Có 1 case study đỉnh để khoe |

---

### Nguồn học đề xuất (từ file gốc)

**Khóa học (Tiếng Anh):**
- CXL Email Marketing Fundamentals — tốt nhất về tư duy hệ thống.
- DigitalMarketer Email Marketing Mastery — tốt cho người làm thực tế.
- HubSpot Academy Email Marketing Certification — miễn phí, đủ dùng cho người mới.
- Google Digital Marketing Certificate (Coursera) — có module email marketing.

**Sách:**
- "Email Persuasion" — Ian Brodie.
- "$100M Offers" — Alex Hormozi.
- "Breakthrough Advertising" — Eugene Schwartz (5 cấp độ nhận thức — kinh điển).
- "Influence" — Robert Cialdini (6 nguyên tắc thuyết phục).

**Người nên theo dõi:**
- Justin Welsh — email-first solopreneur.
- Joanna Wiebe (Copyhackers) — chuyên copywriting cho email.
- Andrew Kamphey (Influence Weekly) — chuyên creator email.

---

### 5 đòn bẩy quan trọng nhất (nếu chỉ làm được 5 việc)

Từ file gốc:
1. Cấu hình SPF + DKIM + DMARC + BIMI (hạ tầng).
2. Bật Google Postmaster Tools (giám sát).
3. Double Opt-in + dọn list mỗi 3 tháng (chất lượng list).
4. Học 4 framework copywriting (PAS, AIDA, BAB, Star–Story–Solution).
5. Xây 1 chuỗi welcome 5 email tự động — chuỗi này có thể đóng góp **30–50% doanh thu email**.

---

### 5 bẫy thường gặp (từ file gốc)

1. **Bẫy "list to là tốt"** — list 3.000 active > 30.000 chết.
2. **Bẫy "viết hay là đủ"** — bỏ trống kỹ thuật, Gmail không tin domain.
3. **Bẫy "gửi nhiều = bán nhiều"** — tăng tần suất → spam complaint tăng → cả list rơi spam.
4. **Bẫy "1 email cho tất cả"** — không phân nhóm, gửi cùng nội dung cho khách mới và khách đã mua.
5. **Bẫy "tập trung vào email mà quên landing page"** — Email chỉ là cầu nối. Landing page mới là nơi bán. Đầu tư email 30%, landing page 70%.

---

## Áp dụng cho ngành TPCN

> Ghi chú: phần này chỉ ghi điều suy ra hợp lý từ nội dung gốc — không thêm số liệu hay case study ngoài file.

- **Segment theo hành vi mua TPCN**: khách mới chưa mua / khách đã mua 1 lần / khách tái mua / khách cũ im lặng.
- **Lead Magnet phù hợp ngành TPCN**: ebook "X ngày làm Y", checklist, quiz "bạn đang thiếu gì", video hướng dẫn.
- **Compliance quan trọng**: TPCN là sản phẩm y tế — nội dung email phải cẩn trọng, tránh khẳng định điều trị/chữa bệnh (vi phạm luật quảng cáo TPCN VN).
- **Kênh phối hợp**: Email + Zalo OA (đã xây ở [[Funnel Zalo OA cho TPCN]]) — hai kênh song song, không thay thế nhau.

---

## Câu hỏi mở

- Anh Chương hiện có list email chưa, hay cần xây từ đầu?
- Nền tảng ESP (Email Service Provider) dự định dùng? (Mailchimp / ActiveCampaign / GetResponse / công cụ VN?)
- Domain marketing đã cấu hình SPF/DKIM/DMARC chưa?
- Lead magnet cho TPCN của anh sẽ là gì?

---

## Trích dẫn gốc đáng nhớ

> "Email chỉ làm 1 việc: tạo cú click." — Khối 12, IPS

> "1.000 email tương tác > 10.000 email chết." — Khối 12, IPS

> "Đầu tư email 30%, landing page 70%." — Khối 12, IPS
