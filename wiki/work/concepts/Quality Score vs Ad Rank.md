---
type: concept
tags: [ads, google, quality-score, ad-rank, ips, khoi-14]
created: 2026-05-09
updated: 2026-05-09
sources: ["[[Khối 14b - ADS Google]]", "[[Khối 14e - Phân tích chỉ số ads]]"]
---

# Quality Score vs Ad Rank — 2 khái niệm hay nhầm nhất

> **Định nghĩa thẳng** *(theo PTL — Khối 14b dòng 69)*:
> - **Quality Score** (Search): điểm chất lượng cho từng từ khoá, thang **1-10**. Cấu thành từ **Expected CTR + Ad Relevance + Landing Page Experience**.
> - **Ad Rank**: cơ chế quyết ad có hiển thị + đứng đâu trên SERP. Cấu thành **6 yếu tố**: bid + chất lượng ad/landing page + thresholds + cạnh tranh auction + ngữ cảnh truy vấn + impact assets/ad formats.

## 🎯 Phân biệt — bảng so sánh

| | Quality Score | Ad Rank |
|---|---|---|
| **Cấp độ** | Mỗi **từ khoá** (keyword) | Mỗi **auction** (real-time) |
| **Phạm vi** | Search Ads | Mọi loại campaign Google |
| **Hiển thị** | Trong UI Google Ads (1-10) | KHÔNG hiển thị trực tiếp |
| **Tần suất tính** | Cập nhật chậm (giờ/ngày) | Real-time mỗi auction |
| **Mục đích** | Tham khảo cho người chạy | Quyết định ad có serve không + vị trí |
| **Thay đổi nhanh** | Không | Có (theo từng truy vấn) |

## 🧱 Quality Score — 3 thành phần (gốc 14b dòng 69)

### 1. Expected CTR

- Google dự đoán keyword này sẽ có CTR bao nhiêu so với cùng vị trí.
- **3 mức**: Above average / Average / Below average.

**Cách cải thiện**:
- Dùng keyword có ý định cao (long-tail, specific).
- Match type chặt hơn (phrase/exact thay vì broad).
- Loại bỏ irrelevant keywords (negative keywords).

### 2. Ad Relevance

- Ad copy có khớp với keyword + intent của người tìm không.
- **3 mức**: Above average / Average / Below average.

**Cách cải thiện**:
- Mỗi ad group chỉ chứa **1 chủ đề chặt** (theme tight).
- Ad copy có chứa **keyword chính**.
- Tách brand vs non-brand vào campaign khác.

### 3. Landing Page Experience

- Trải nghiệm trên landing page sau khi click.
- **3 mức**: Above average / Average / Below average.

**Cách cải thiện**:
- Tốc độ ≤2.5s mobile.
- Khớp thông điệp với ad (headline, offer).
- 1 CTA chính rõ ràng.
- Không pop-up spam.
- Mobile-friendly.

## 🏆 Ad Rank — 6 yếu tố (đầy đủ theo Google chính thức)

> ⚠️ Tài liệu gốc PTL đơn giản hoá thành `Ad Rank = Max CPC × Quality Score (+ yếu tố khác)` — em (agent) bổ sung đầy đủ 6 yếu tố theo Google Help chính thức:

1. **Bid** (Max CPC hoặc bid Smart Bidding tự đặt).
2. **Chất lượng ad + landing page** (gồm Quality Score + landing page experience).
3. **Ad Rank thresholds** — ngưỡng tối thiểu để được hiển thị trên 1 vị trí.
4. **Mức cạnh tranh auction** — bao nhiêu ad đang cạnh tranh cùng truy vấn.
5. **Ngữ cảnh truy vấn** — device, location, time, browsing history, audience.
6. **Tác động kỳ vọng của assets/ad formats** — có sitelinks, callouts, structured snippets...

## 💰 Lợi ích Quality Score cao

> Theo PTL: "Chất lượng tốt hơn không chỉ tăng vị trí mà còn có thể **giảm CPC thực tế** + **tăng khả năng hiển thị assets**."

| Quality Score | Tác động |
|---|---|
| **8-10** | CPC giảm đáng kể, assets hiển thị thường xuyên |
| **5-7** | Chấp nhận được, không lợi thế |
| **<5** | CPC tăng cao + assets ít hiển thị + cần tối ưu gấp |

→ **Quality Score 10 có thể trả ít hơn ~50% so với Quality Score 5** cho cùng vị trí *(theo industry data — không có trong PTL gốc nhưng là pattern Google đã công bố qua Help docs)*.

## 🎯 Cách build ad group có Quality Score cao

### 1. Theme tight — 1 chủ đề/ad group

❌ **Sai**: 1 ad group "TPCN" với 50 keywords từ "collagen" đến "vitamin tổng hợp" đến "men tiêu hoá".

✅ **Đúng**: tách thành 5 ad group:
- "Collagen cho phụ nữ 35+"
- "Vitamin tổng hợp cho người văn phòng"
- "Men tiêu hoá cho người ăn uống thất thường"
- ...

### 2. Ad copy chứa keyword chính

❌ "Chăm sóc sức khoẻ chuyên nghiệp"
✅ "Collagen cho phụ nữ 35+ — Cải thiện đàn hồi da sau 8 tuần"

### 3. Landing page khớp ad

- Headline ad: "Collagen cho phụ nữ 35+"
- Headline LP: "Collagen cho phụ nữ 35+: Hướng dẫn lựa chọn"

→ KHÔNG dẫn về homepage chung.

### 4. RSA + assets đầy đủ

- ≥**2 RSA/ad group**.
- ≥**4 sitelinks** (kể về features, social proof, FAQ, contact).
- Callouts (USP ngắn).
- Structured snippets (cho dòng sản phẩm).
- Image extensions.

### 5. Negative keywords thường xuyên

- Review search terms hàng tuần.
- Loại bỏ truy vấn không liên quan (vd: "free", "DIY", "tự làm").

## 📊 Đọc Quality Score trong Google Ads

| Trong UI | Ý nghĩa |
|---|---|
| Tab **Keywords** → cột **Qual. score** | Điểm 1-10 cho từng keyword |
| Hover vào điểm | Xem 3 thành phần (Expected CTR, Ad Relevance, Landing Page Experience) |
| Status **Below first page bid** | Bid + Quality Score quá thấp để serve |

## 🚨 5 sai lầm Quality Score / Ad Rank

1. **Đổ lỗi cho Quality Score thấp khi CPC cao** — đôi khi chỉ là cạnh tranh tăng (yếu tố 4 Ad Rank), không phải QS giảm.
2. **Tăng bid để bù QS thấp** — đốt tiền. Phải sửa gốc: ad copy, landing page, theme tightness.
3. **Dùng broad match cho mọi keyword** → Expected CTR thấp.
4. **Landing page chậm** → Landing Page Experience thấp dù ad copy tốt.
5. **Không dùng RSA + assets** → Ad Rank thấp ở yếu tố 6 (impact assets).

## 🎯 Hành động cho anh Chương — TPCN

📎 *Em đề xuất*:

1. **Trước launch ads** — setup mỗi cluster TPCN từ [[Khối 9 - SEO Blog 2026]] thành **1 ad group**.
2. **Mỗi ad group**:
   - 2 RSA chứa keyword chính.
   - ≥4 sitelinks.
   - Landing page = bài Trụ cluster (đã chuẩn E-E-A-T).
3. **Quality Score mục tiêu** ≥7 sau 30 ngày, ≥8 sau 60 ngày.
4. **Hàng tuần**: review search terms → thêm negatives → tăng QS.
5. **PageSpeed Mobile ≥90** cho mọi landing page (Landing Page Experience = "Above average").

## 🔗 Liên quan

- [[Khối 14b - ADS Google]] — phần 2 bản đồ yếu tố
- [[Smart Bidding (Google)]] — bid là yếu tố 1 của Ad Rank
- [[Khối 9 - SEO Blog 2026]] — landing page chuẩn E-E-A-T = LP Experience cao
- [[Khối 13 - SEO sản phẩm Website]] — landing page sản phẩm chuẩn SEO + CRO
