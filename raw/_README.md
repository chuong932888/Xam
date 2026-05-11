---
type: meta
---

# 📥 raw/ — Nguồn gốc

Thả tất cả nguồn anh muốn nạp vào đây:

- Bài viết clip từ web (dùng **Obsidian Web Clipper** → set output folder = `raw/`).
- File markdown anh tự viết.
- PDF, ảnh chụp màn hình, hình ảnh → để trong `raw/assets/` rồi link tới.
- File `.txt`, `.docx`, `.epub`...

## Quy tắc

- **LLM KHÔNG sửa file ở đây.** Đây là source of truth.
- Tên file = tên nguồn (ví dụ: `Sách - Đắc Nhân Tâm.md`, `Bài viết - Compounding Wiki.md`).
- Sau khi thả nguồn vào, nói với Claude: **"ingest [tên file]"** hoặc **"ingest mọi nguồn chưa xử lý"**.

## Tip Obsidian

- Settings → Files and links → Attachment folder path: `raw/assets/`
- Settings → Hotkeys → "Download attachments for current file" → bind `Ctrl+Shift+D`. Sau khi clip bài, hit hotkey để kéo ảnh về local.
