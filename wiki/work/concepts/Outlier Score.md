---
type: concept
tags: [youtube, analytics, outlier, format, paddy-galloway, ideation]
created: 2026-05-09
updated: 2026-05-09
sources: ["[[Khối 3 - Chiến lược YouTube]]"]
---

# Outlier Score — Công thức đo video vượt trội

## Định nghĩa

**Outlier Score** là chỉ số đo một video đang perform tốt hơn baseline kênh ở mức nào:

```
Outlier Score = Views của video / Median views của kênh
```

Dùng **median** (trung vị) thay vì average (trung bình) vì average bị kéo lên bởi các video outlier trước đó.

---

## Thang đánh giá

| Outlier Score | Mức độ | Hành động |
|---|---|---|
| **< 2x** | Noise — có thể do luck, thời điểm, external traffic | Không kết luận |
| **2x** | Noise — theo dõi thêm | Ghi nhận nhưng chưa replicate |
| **3x+** | Signal đáng nghiên cứu | Phân tích kỹ: title / thumbnail / hook / format |
| **5x** | Strong outlier | Series hoá format ngay |
| **10x+** | Breakout | Đây là format engine của kênh — đào sâu |
| **100x+** | Anomaly | ⚠️ KHÔNG replicate blindly — có thể do viral accident, external spike, không sustainable |

**Paddy Galloway "29 lessons" (tháng 3/2025):** "90%+ growth của kênh đến từ 1 ý tưởng outlier. Great channels turn 1 outlier idea into a repeatable format."

---

## Cách tìm outlier để học

### 1. Tìm outlier trong kênh của mình

Vào YouTube Studio → Analytics → Content → Sort by Views. So sánh với median:
- Video nào 3x+ median → phân tích sâu: cái gì đã khác biệt?
- Format đó có thể Series hoá không?

### 2. Tìm outlier trong niche và adjacent niches

**Tools:**

| Tool | Giá | Cách dùng |
|---|---|---|
| **OutlierKit** | $9/tháng | Detect video 3x+ outlier trong niche — clone format |
| **VidIQ Outliers** | Pro/Max $7.5-39/tháng | Find outlier thumbnails trong adjacent niches |
| **1of10** | Trả phí | "1 in 10" outlier finder — videos performing unexpectedly well |
| **YouTube native search** | FREE | Niche term → filter Long videos → sort Most Viewed → study top 20-30 |

### 3. Quy trình nghiên cứu outlier

**Bước 1:** Tìm video outlier (3x+ median kênh đó).

**Bước 2:** Trả lời 3 câu hỏi phản chiếu:
- **"What made this UNIQUE?"** — điều gì khác biệt so với 1.000 video khác cùng topic?
- **"Why this title vs 1000 others?"** — title có yếu tố gì (curiosity gap, số, claim bất ngờ)?
- **"Could I model this for MY niche?"** — format có portable không?

**Bước 3:** "Copy with taste, not copy and paste" (MrBeast) — adapt format, không clone y nguyên.

---

## Ideation Machine — Train đến 100 ideas/tuần

**Paddy Galloway:** "Brainstorm 100 ideas/tuần để train idea evaluation muscle."

Không phải để thực hiện 100 ý tưởng — mà để **train khả năng nhận diện ý tưởng tốt vs tệ**. Sau vài tuần làm 100/tuần, anh sẽ biết ngay "cái này có đất không" trong 10 giây.

**Quy trình thực tế:**

**Phiên brainstorm 1 giờ/tuần:**
1. Set timer 20 phút — viết 50+ ideas (không filter, không judgement).
2. Set timer 10 phút — xem lại, gạch chân 10 ideas tiềm năng nhất.
3. Set timer 10 phút — với 10 ideas đó, thử viết title theo formula VN.
4. Set timer 10 phút — ideas nào title hay + có thể làm thumbnail ấn tượng → vào "pipeline".
5. Cuối tuần: chọn 1-2 idea tốt nhất để thực hiện.

**Lưu ý:** Không bao giờ bắt đầu quay trước khi có title tốt. "If you can't design a compelling thumbnail, the idea isn't worth filming."

---

## Pre-production — 20% better title = exponential view

**Phân bổ thời gian theo Paddy Galloway:**
- Top creators: **30% time** cho ideation + packaging.
- Small creators: chỉ **5% time** cho ideation + packaging, 95% cho production.

→ Đây là lý do kênh lớn grow nhanh hơn dù content không nhất thiết tốt hơn về production.

**Spend 50%+ time trên pre-production** (idea + title + thumbnail) trước khi quay 1 shot nào.

---

## Áp dụng TPCN — Series hoá format thắng

### Bước 1: Identify outlier format

Sau 20-30 video đầu, track outlier score mỗi video:

```
Video 1 — "Hành trình từ xăm sang TPCN" → 1.5x median (noise)
Video 5 — "Lỗi 1: Tôi chọn nhà cung cấp TPCN sai — mất 50 triệu" → 4.2x median (SIGNAL)
Video 8 — "Lỗi 2: Pricing TPCN sai hoàn toàn" → 3.8x median (signal)
Video 12 — "Lỗi 3: Tôi không biết YMYL là gì..." → 5.1x median (STRONG)
```

→ Format "Lỗi X: Tôi đã sai về Y trong TPCN" là format thắng → Series hoá.

### Bước 2: Series hoá

```
Series: "10 Lỗi Tôi Gặp Khi Xây Doanh Nghiệp TPCN"
→ Lỗi 1, Lỗi 2, ... Lỗi 10
→ Playlist → autoplay → session time tăng
→ Gemini nhận diện cluster rõ hơn
```

### Bước 3: Tìm outlier trong adjacent niche

Dùng OutlierKit → tìm outlier trong niche sức khoẻ VN, CEO vlog VN → identify format portable sang TPCN.

---

## Cảnh báo — Anomaly 100x+

Video viral quá mức (100x+ median) thường do:
- Được share trên Facebook/Zalo theo cách không kiểm soát
- Được algorithm push vì coincidence (right topic right time)
- Viral accident — không phải vì format

**Replicate blindly → thất vọng.** Thay vào đó: phân tích *tại sao* viral, rút element có thể portable, không copy nguyên xi.

---

## Liên kết

- [[CCN Framework]] — outlier thường là video appeal được cả 3 nhóm CCN
- [[Large Recommender Model (LRM)]] — LRM reward outlier format vì nó tạo strong satisfaction signal
- [[Packaging YouTube]] — outlier thường bắt đầu từ packaging khác biệt
- [[Retention Curve Analysis]] — outlier thường có retention curve đặc biệt tốt
- [[Khối 3 - Chiến lược YouTube]]

---

## Tóm tắt 1 câu

> Outlier Score = views / median views của kênh — 3x+ là signal đáng nghiên cứu, 5x+ là format cần series hoá ngay, 100x+ là anomaly không replicate blindly.
