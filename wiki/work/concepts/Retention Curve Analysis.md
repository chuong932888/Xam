---
type: concept
tags: [youtube, analytics, retention, avd, hook, editing, algorithm]
created: 2026-05-09
updated: 2026-05-09
sources: ["[[Khối 3 - Chiến lược YouTube]]"]
---

# Retention Curve Analysis — Đọc và Xử lý 5 Dạng Curve

## Tại sao retention curve quan trọng hàng đầu

Retention curve là **tín hiệu trực tiếp nhất** mà LRM (Large Recommender Model) đọc để quyết định có push video hay không:

- Retention 60s mark **≥ 55%** → algorithm gần như luôn promote.
- Retention 60s mark **< 40%** → gần như luôn stop push.
- MrBeast đạt **70% retention** xuyên suốt toàn bộ video dài — đây là benchmark đỉnh ngành.

**Xem retention curve ở đâu:** YouTube Studio → Analytics → chọn video → Engagement → Audience Retention.

---

## Benchmark retention các điểm chốt

| Điểm đo | Mức threshold |
|---|---|
| **30 giây** | ≥ 60% strong; ≥ 70% excellent; < 40% = hook failure (must fix) |
| **50% thời lượng video** | ≥ 45-55% |
| **Cuối video** | ≥ 30% healthy; ≥ 50% xuất sắc |

**AVD benchmark theo độ dài:**

| Độ dài video | Target AVD |
|---|---|
| < 5 phút | ≥ 60-70% |
| 5-10 phút | ≥ 50-60% |
| 10-15 phút | ≥ 40-50% |
| 15-25 phút | ≥ 35-45% |
| 25+ phút | ≥ 25-35% |

---

## 5 Dạng Retention Curve Điển hình

### Dạng 1: Spike > 100% — Viral Moment

```
Retention %
120% |    ████
     |   ██████
100% |  ████████
 80% |██████████████████
     |____________________ Thời gian
```

**Ý nghĩa:** Người xem **tua lại / rewind** đoạn đó — nội dung quá hay, shock, hoặc cần nghe lại.

**Hành động:**
- ✅ **Trích thành Short ngay** — đây là viral moment cao nhất của video.
- ✅ Pin comment về Short đó để direct traffic.
- ✅ Note lại format/content type của đoạn đó → replicate trong video tiếp theo.
- Không cần fix gì trong video gốc.

**Ví dụ:** Đoạn anh reveal số doanh thu thực tế → người xem tua lại để nghe chắc → đây là nội dung Social Blade / proof cực mạnh → trích thành Short 30-60 giây.

---

### Dạng 2: Skip-ahead Spike — Viewer dùng Chapters

```
Retention %
100% |████           ████
 80% |     ████ ████
 60% |          ▼▼▼▼
     |     (jump forward)
     |____________________ Thời gian
```

**Ý nghĩa:** Người xem đang **nhảy chapter** — họ muốn xem phần cụ thể, bỏ qua phần khác.

**Hành động:**
- Cấu trúc lại chapter — đặt nội dung quan trọng nhất ở chương đầu, không chôn cuối video.
- Đặt tên chapter keyword-rich và cụ thể: "Cách chọn nhà cung cấp collagen VN" thay vì "Phần 2".
- Check: liệu phần bị skip có value không? Nếu không → cắt bỏ trong video tương lai.
- ✅ Chapters được surface trong Google AI Overview → SEO benefit thêm.

---

### Dạng 3: Drop sớm (30 giây đầu) — Hook Fail

```
Retention %
100% |█
 80% |  ██
 60% |    ████████████████
 40% | (cliff drop trong 30s đầu)
     |____________________ Thời gian
```

**Ý nghĩa:** Người xem rời ngay từ đầu — **hook thất bại**.

**Hành động — ưu tiên FIX NGAY:**
- Đổi opening 3-7 giây đầu: start mid-action, show result first, bold contradictory claim.
- **Tránh hoàn toàn:** "Hey guys, welcome back to my channel", slow zoom/fade in, channel intro animation.
- Test lại với 3 formula hook: (1) Show payoff trước, (2) Đặt câu hỏi bất ngờ, (3) Số liệu shock.
- Trong YouTube Studio → A/B test bản hook mới.

**Check list hook 30 giây:**
- [ ] 7 giây đầu có establish value rõ ràng không?
- [ ] Có tránh long intro, sponsor-heavy cold open không?
- [ ] Outcome đã được show đầu video, process giải thích sau?

---

### Dạng 4: Linear Decline — Retention Tự nhiên

```
Retention %
100% |████████
 80% |        ████████
 60% |                ████████
 40% |                        ████████
     |____________________ Thời gian
```

**Ý nghĩa:** Người xem rời dần theo thời gian — **bình thường hoàn toàn** với video dài. Không phải tín hiệu xấu.

**Hành động:**
- ✅ Không cần fix gì nếu retention cuối ≥ 30%.
- Nếu muốn improve: thêm pattern interrupt mỗi 25-40s từ phút 3-7.
- Thêm cliffhanger / teaser cho điều sẽ đến sau (episodic style).

---

### Dạng 5: Cliff Drop giữa Video — Transition Tệ

```
Retention %
100% |████████████████
 80% |
 60% |                (cliff drop đột ngột)
 40% |                ████████████████████
     |____________________ Thời gian
```

**Ý nghĩa:** Đoạn giữa video có **transition tệ, boring stretch, hoặc sudden topic change** làm người xem thoát hàng loạt.

**Hành động:**
- Identify chính xác timestamp xảy ra cliff → xem lại đoạn đó.
- Nguyên nhân thường gặp: (1) sponsor đọc dài, (2) chuyển topic không smooth, (3) cảnh quay nhàm, (4) không có visual change.
- **Cắt/edit đoạn đó** nếu video còn chỉnh sửa được.
- Cho video tiếp theo: thêm pattern interrupt tại vị trí đó (cut angle, graphic, B-roll, music drop).
- Không link card/end screen tại điểm retention drop — chỉ đặt khi retention đang cao.

---

## Cách cải thiện retention — Checklist thực chiến

### Hook (0-30 giây)
- [ ] Start mid-action hoặc show result trước.
- [ ] Bold contradictory claim hoặc specific number question.
- [ ] Pattern interrupt ngay giây 15 (re-hook).
- [ ] Tránh logo intro, "subscribe first", "in today's video".

### Thân video (30s - hết)
- [ ] Pattern interrupt mỗi **10-15s** trong 3 phút đầu.
- [ ] Pattern interrupt mỗi **25-40s** từ phút 3-7.
- [ ] Sound design: whoosh, pop, coin drop tại impact moments.
- [ ] B-roll mỗi 7-10s, cut to data/graphic cho stats.
- [ ] Music tone shift = emotional reset.
- [ ] Không bao giờ link off-platform TRONG video (kết thúc session = penalty).

### Ending (60-70 giây cuối)
- [ ] Verbal CTA trước end screen (giây 60-70 trước cuối).
- [ ] End screen CLick CTR target: 5-15% healthy, >15% xuất sắc.
- [ ] Teaser "video tiếp theo" để session continue.

---

## Áp dụng TPCN — Workflow review hàng tuần

**Mỗi tuần, review retention curve cho top 5 video:**

**Thứ 2 (30 phút):**
1. Vào YouTube Studio → Analytics → Content.
2. Sort by Views, chọn top 5 video trong 28 ngày.
3. Mỗi video: check retention curve — note dạng curve nào (1-5 ở trên).
4. Identify 1 điểm cần fix hoặc 1 viral moment cần trích thành Short.

**Thứ 3:**
- Nếu có Spike >100% → trích Short trước 48h.
- Nếu có Hook Fail (drop 30s đầu) → outline hook mới, test A/B.
- Nếu có Cliff Drop → mark timestamp, edit hoặc note cho video tiếp theo.

**Tracking sheet đơn giản:**

| Video | AVD | Retention 30s | Dạng curve | Hành động |
|---|---|---|---|---|
| Video A | 48% | 72% | Linear | ✅ OK |
| Video B | 31% | 38% | Hook Fail | 🔴 Đổi hook |
| Video C | 55% | 68% | Spike 105% tại 2:30 | ✅ Trích Short |

---

## Liên kết

- [[Large Recommender Model (LRM)]] — LRM đọc retention curve là signal chính để rank
- [[Outlier Score]] — Spike >100% thường correlate với outlier score cao
- [[Playbook 24-48h sau upload]] — Check retention trong 24h đầu để decide next action
- [[Packaging YouTube]] — Packaging tốt giúp đúng người xem → retention tự nhiên cao hơn
- [[Khối 3 - Chiến lược YouTube]]

---

## Tóm tắt 1 câu

> Đọc retention curve hàng tuần: spike >100% = trích Short, cliff drop = cắt/fix transition, hook fail = đổi opening — linear decline là bình thường, đừng over-engineer.
