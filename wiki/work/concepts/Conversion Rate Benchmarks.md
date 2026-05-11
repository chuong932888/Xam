---
type: concept
tags: [tiktok, funnel, conversion, kpi, benchmarks]
created: 2026-05-09
updated: 2026-05-09
sources: ["[[Khối 5 - Chiến lược TikTok]]"]
---

# Conversion Rate Benchmarks — Ngưỡng chuyển đổi phễu TikTok

## Định nghĩa

**Conversion Rate Benchmarks** là bảng ngưỡng tham chiếu vận hành nội bộ — dùng để **chẩn đoán chỗ tắc trong phễu** và quyết định nên can thiệp ở bước nào. Đây là **target nội bộ đề xuất**, không phải benchmark chính thức của TikTok hay bất kỳ nền tảng nào.

**Khi nào dùng**: Hàng tuần, khi review dashboard, khi chuẩn bị scale hay khi doanh thu lệch forecast.

---

## Bảng 10 ngưỡng chuyển đổi

| # | Điểm đo trong phễu | Ngưỡng đề xuất | Đo bằng công cụ nào |
|---|---|---|---|
| 1 | **Profile visit / Video views** | 1% – 3% với video thắng | TikTok Analytics (video) |
| 2 | **Follow / Profile visit** | 15% – 30% | TikTok Analytics (profile) |
| 3 | **Lead opt-in / Profile visit** | 15% – 35% | Landing page / form tracking |
| 4 | **Lead → Low-ticket purchase** | 1% – 5% | CRM / email platform |
| 5 | **Low-ticket buyer → Mid-ticket** | 5% – 15% | CRM / order history |
| 6 | **Mid-ticket → High-ticket** | 1% – 3% | CRM / sales pipeline |
| 7 | **Repeat purchase rate** | 20% – 40% | Shopee/Shop analytics hoặc CRM |
| 8 | **LIVE viewer → Đặt hàng** | 3% – 8% | TikTok LIVE analytics + order data |
| 9 | **Email open rate** | 20% – 35% | Email platform (Mailchimp, AVADA...) |
| 10 | **Email CTR (click-through rate)** | 2% – 5% | Email platform |

---

## Khi nào nghi ngờ ngưỡng này

**Cẩn thận áp dụng máy móc trong 3 tình huống:**

### Volume thấp
Nếu sample size nhỏ (dưới 500 lần đo cho mỗi bước), tỷ lệ có thể dao động mạnh và chưa có ý nghĩa thống kê. Ví dụ: 3 profile visit → 1 follow = 33%, trông "cao" nhưng không có giá trị.
> **Quy tắc ngón tay cái**: cần tối thiểu 300-500 lần đo ở bước đầu mới tin con số ở bước sau.

### Niche đặc thù
- TPCN cao cấp (AOV lớn, quy trình tư vấn dài): follow/profile visit có thể thấp hơn (5-15%) nhưng mỗi follow = intent cao hơn nhiều
- Hàng tiêu dùng nhanh, giá thấp: chuyển đổi LIVE → đơn hàng có thể lên đến 10-15%
- B2B / coaching high-ticket: Lead → Low-ticket thấp nhưng Low → High có thể cao hơn

### Kênh đang trong giai đoạn test
30 ngày đầu: benchmark không áp dụng — đang tìm format, chưa đủ data. Bắt đầu đo nghiêm túc từ ngày 31 trở đi khi đã có 2 format thắng ổn định.

---

## Áp dụng TPCN — Chẩn đoán phễu chỗ nào tắc

### Cách đọc bảng để tìm điểm tắc

**Bước 1**: Điền số thực tế của kênh vào từng dòng.

**Bước 2**: So sánh với ngưỡng đề xuất.

**Bước 3**: Tìm bước đầu tiên bị lệch — đó là **nút cổ chai** cần xử lý trước.

### Ví dụ chẩn đoán thực tế — TPCN

```
Kịch bản: Kênh có view ổn nhưng doanh thu thấp

Điểm đo                          | Thực tế | Ngưỡng  | Nhận xét
Profile visit / Video views       | 2.1%    | 1-3%    | ✅ Bình thường
Follow / Profile visit            | 22%     | 15-30%  | ✅ Bình thường
Lead opt-in / Profile visit       | 8%      | 15-35%  | ⚠️ THẤP — đây là nút cổ chai
Lead → Low-ticket                 | —       | 1-5%    | Chưa đủ data vì lead quá ít

→ CHẨN ĐOÁN: Landing page/lead magnet chưa đủ hấp dẫn hoặc CTA chưa rõ.
→ HÀNH ĐỘNG: A/B test lead magnet (đổi offer, đổi headline, đổi CTA trong bio).
```

```
Kịch bản: Có lead nhưng không ra đơn

Điểm đo                          | Thực tế | Ngưỡng  | Nhận xét
Lead opt-in / Profile visit       | 25%     | 15-35%  | ✅ Tốt
Lead → Low-ticket                 | 0.3%    | 1-5%    | ⚠️ THẤP — nút cổ chai ở đây
Low-ticket → Mid-ticket           | —       | 5-15%   | Chưa đủ data

→ CHẨN ĐOÁN: Email sequence/follow-up sau opt-in yếu, hoặc offer low-ticket chưa match pain.
→ HÀNH ĐỘNG: Review email sequence 1-5, test offer khác, thêm testimonial vào sales page.
```

---

## Thứ tự ưu tiên khi phát hiện điểm tắc

1. **Luôn sửa điểm tắc đầu tiên trước** — không nhảy xuống sửa bước cuối khi bước đầu đang vỡ
2. **Một thay đổi tại một thời điểm** — để biết cái gì tạo ra sự khác biệt
3. **Chạy tối thiểu 7-14 ngày** trước khi kết luận thay đổi có hiệu quả hay không (trừ những test rõ ràng thất bại từ ngày 1-2)

---

## Liên kết

- [[Khối 5 - Chiến lược TikTok]]
- [[Offer Ladder]]
- [[TOFU-MOFU-BOFU]]
- [[Retention Curve Analysis]]
- [[Revenue Stack]]
