---
type: tool
tags: [ai, prompt, keyword, ips, khoi-2]
created: 2026-05-09
updated: 2026-05-09
sources: ["[[Khối 2 - Cách tìm kiếm từ khoá]]"]
---

# 🤖 AI Prompts — Keyword Research (7 prompt mẫu)

> **Copy nguyên văn, thay phần `[trong ngoặc vuông]`, paste vào ChatGPT / Claude / Gemini.** 7 prompt từ thầy [[Phạm Thành Long]] (Khối 2 IPS).
>
> ⚠️ AI **KHÔNG có data volume thật** → luôn cross-check kết quả bằng Google Keyword Planner / Ahrefs trước khi quyết định đầu tư content.

---

## Prompt 1 — Mở rộng seed thành 50 long-tail

```text
Bạn là chuyên gia SEO ngành [Thực phẩm chức năng]. Tôi có seed keyword: "[seed keyword]".

Hãy sinh ra 50 biến thể long-tail keyword (4-8 từ mỗi cái) mà khách hàng VIỆT NAM thật sự sẽ gõ vào Google.

Yêu cầu:
- Phân thành 3 nhóm: informational (10), commercial (20), transactional (20)
- Dùng tiếng Việt tự nhiên, có dấu, đúng cách người Việt gõ (chứ không phải dịch máy)
- Mỗi keyword kèm intent (1 từ) và funnel stage (TOFU/MOFU/BOFU)
- Tránh trùng lặp ý

Format: bảng markdown 4 cột (keyword | nhóm | intent | funnel)
```

**Ví dụ TPCN — seed phù hợp dùng:**
- "collagen", "thực phẩm chức năng", "viên ngủ", "vitamin tổng hợp", "đông trùng hạ thảo", "men vi sinh", "thực phẩm chức năng giảm cân", "tăng đề kháng"

---

## Prompt 2 — Phân loại keyword theo intent

```text
Tôi có danh sách [số] keyword sau:

[paste danh sách, mỗi keyword 1 dòng]

Hãy phân loại mỗi keyword vào:
1. Search intent: informational / navigational / commercial investigation / transactional
2. Funnel stage: TOFU / MOFU / BOFU
3. Loại content phù hợp nhất: blog / video / landing page / podcast / infographic

Trả về bảng markdown 4 cột.
```

**Cách dùng:** Sau khi Prompt 1 ra 50 keyword, paste cả danh sách vào Prompt 2 để verify intent + map kênh.

---

## Prompt 3 — Sinh People Also Ask

```text
Khi người Việt gõ "[keyword]" vào Google, họ thường tự hỏi thêm những câu nào?

Hãy sinh 15 câu hỏi liên quan, theo cấu trúc:
- 5 câu bắt đầu bằng "Có/Không/Phải" (yes/no questions)
- 5 câu bắt đầu bằng "Làm thế nào / Như thế nào"
- 5 câu bắt đầu bằng "Bao nhiêu / Bao lâu / Khi nào / Ở đâu / Tại sao"

Mỗi câu kèm 1 dòng lý do tại sao người tìm "[keyword]" lại hỏi thêm câu đó.
```

**Mục đích:** 15 câu hỏi này → outline cho phần FAQ trong landing page hoặc blog. PAA = mỏ vàng nội dung TOFU.

---

## Prompt 4 — Sinh outline blog từ cluster

```text
Tôi đang viết blog về cluster keyword sau:

Pillar keyword: "[pillar]"
Supporting keywords:
- "[kw 1]"
- "[kw 2]"
- "[kw 3]"
... [thêm nếu có]

Persona: [mô tả persona 2-3 câu]
Funnel stage: [TOFU/MOFU/BOFU]
Mục tiêu: [mục tiêu — opt-in email / đặt lịch / mua…]

Hãy sinh outline blog 2.500 từ với:
- Title 6-9 từ chứa pillar keyword
- Meta description 150 ký tự
- 7-9 H2 (mỗi H2 cover 1 supporting keyword)
- Mỗi H2 có 2-3 H3
- CTA cuối bài khớp với mục tiêu
- Internal link gợi ý

Trả về dạng markdown.
```

**Ví dụ TPCN persona để chèn:**
> "Phụ nữ 35-45 tuổi, lo lắng về lão hóa da và sức khỏe sau 35, đang tìm giải pháp TPCN có khoa học chứng minh, không tin sản phẩm thị trường vô danh, ngân sách 2-5 triệu/tháng cho TPCN."

---

## Prompt 5 — Title + Meta description

```text
Cho keyword chính: "[keyword]"
Search intent: [intent]
USP của brand mình: [1-2 câu]

Hãy sinh:
- 5 phương án title (50-60 ký tự, chứa keyword chính trong nửa đầu)
- 5 phương án meta description (150-160 ký tự, có CTA)
- Đánh giá 1-10 cho mỗi phương án về tiềm năng CTR

Trả về bảng markdown.
```

---

## Prompt 6 — Hashtag TikTok / Instagram

```text
Cho video / post nói về: "[chủ đề]"
Keyword chính: "[keyword]"
Đối tượng: [persona]

Hãy sinh hashtag mix 15 cái cho:
- TikTok: 5 hashtag (1 large >1M video, 2 medium 100K-1M, 2 niche <100K)
- Instagram: 10 hashtag (mix đủ size)

Mỗi hashtag kèm ước tính độ phổ biến + lý do chọn.
```

---

## Prompt 7 — Phân tích keyword đối thủ

```text
Đối thủ của tôi là: [tên website/brand]
Họ đang rank top cho các keyword:
- "[kw 1]" — position [x]
- "[kw 2]" — position [y]
- "[kw 3]" — position [z]
... [paste 10-30 keyword]

Tôi là [mô tả brand mình + USP].

Hãy phân tích:
1. Đâu là keyword đối thủ mạnh nhưng tôi không nên đụng (vì lệch USP / KD quá cao)
2. Đâu là keyword đối thủ rank mà tôi NÊN đụng (gap về USP / nội dung yếu)
3. Đâu là keyword đối thủ chưa cover mà tôi nên chiếm trước
4. Đề xuất 5 cluster nội dung tôi nên ưu tiên trong 90 ngày
```

**Cách lấy keyword đối thủ:** Dùng Ahrefs Site Explorer → Organic keywords. Nếu không có Ahrefs, dùng Ubersuggest (free 3 lượt/ngày) hoặc Mangools KWFinder (rẻ nhất).

---

## 🎯 Workflow gợi ý dùng 7 prompt

1. **Tuần 1**: Prompt 1 cho 5-10 seed → ra 250-500 long-tail
2. **Tuần 1**: Prompt 2 phân loại — verify intent
3. **Tuần 1**: Áp [[Rubric 10 điểm lọc keyword]] → còn 30 keyword vàng
4. **Tuần 2**: Prompt 3 cho top 5 keyword → 15 câu PAA/keyword (75 câu)
5. **Tuần 2**: Prompt 4 sinh outline cho 3-5 cluster ưu tiên
6. **Tuần 3**: Prompt 5 + 6 cho mỗi nội dung sắp đăng
7. **Mỗi quý**: Prompt 7 với đối thủ — tìm gap mới

## 🔗 Liên quan

- [[Khối 2 - Cách tìm kiếm từ khoá]]
- [[Template Google Sheet Keyword Master]]
- [[Checklist Keyword Research]]
- [[Search Intent]], [[TOFU-MOFU-BOFU]], [[Rubric 10 điểm lọc keyword]]
