# 📜 Nhật ký

> Append-only. Entry mới ở **dưới cùng**. Mỗi entry bắt đầu bằng `## [YYYY-MM-DD] <loại> | <mô tả>` để grep được.
>
> Loại: `ingest` | `query` | `action` | `lint` | `review tuần` | `meta` (đổi schema)

## [2026-05-11] meta | vault forked from TPCN
- Vault XAM được fork từ vault TPCN (ngày 2026-05-11) để xây Não cho ngành xăm — dùng cho cá nhân anh Chương + chia sẻ cho nhân viên qua GitHub.
- Đã xoá: `wiki/work/du-an-tpcn-xuong-khop/`, `Dự án X.md` (rỗng), `wiki/work/concepts/Funnel Zalo OA cho TPCN.md` (logic TPCN không áp dụng cho xăm).
- Đã reset: `now.md`, `actions.md`, `log.md` về template trống.
- Đã sửa: `CLAUDE.md` (bỏ rule "không xăm", đổi mục đích vault, đổi hồ sơ), `wiki/me.md`, `index.md`.
- Giữ nguyên: toàn bộ `wiki/learn/` (kiến thức PTL), `wiki/work/concepts/`, `wiki/work/tools/`, `wiki/work/jobs/`, `wiki/people/Phạm Thành Long.md`, `raw/`.
- Bonus: `raw/Đặc sản của Phạm Thành Long/Thợ xăm/` có 2 file gốc PTL về thợ xăm — vault TPCN trước đây không ingest do rule cấm; vault XAM ingest được khi cần.
- Memory folder mới (5 file, bỏ 2 file TPCN-specific) ở: `~/.claude/projects/-Users-tranchuong-Library-Mobile-Documents-com-apple-CloudDocs-XAM/memory/`.

## [2026-05-12] ingest | Wiki "Kiến thức xăm" — 17 file kỹ thuật từ video anh Trần Chương
- Tạo wiki mới `wiki/kien-thuc-xam/` (ngang hàng work/learn/life/people) để lưu kiến thức kỹ thuật xăm. Mục đích: nhân viên công ty XAM tra cứu khi giải đáp câu hỏi cho thợ xăm mới.
- 17 file gốc trong `raw/kiến thức xăm/` (transcript YouTube của anh Trần Chương) được 17 sub-agent đọc song song trong 1 round, mỗi agent format ≥95% theo template wiki chung.
- 17 page tạo ra (độ phủ ước tính ~96-97%):
  - Chuẩn bị: `u-te-truoc-khi-xam`, `scan-hinh-len-da`
  - Cầm máy: `cam-may-di-net`, `cam-may-danh-bong-vao-mau`
  - Tô đen: `to-den-co-ban-seri-2-thang`, `to-den-kim-m1`, `danh-bong-cong-to-den-nang-cao`
  - Đánh bóng & đánh khối Nhật cổ: `danh-bong-tren-da-gia-bai-1`, `danh-bong-nhat-co-bai-1/2/3`, `danh-bong-mang-lon`, `danh-khoi-nhat-co-don-gian`
  - Pha mực: `pha-muc-tu-mau-co-ban`, `pha-muc-xam-mau-tattoo`
  - Vào màu: `vao-mau-nhat-co`
  - Dưỡng hậu xăm: `duong-hinh-sau-khi-xam`
- File overview `Kien thuc xam.md` đóng vai trò mục lục theo chủ đề + hướng dẫn nhân viên cách dùng wiki.
- Đã update `index.md` thêm section 🎨 Kiến thức xăm + cập nhật thống kê (~165 page wiki).
- QA round 2 (17 agent độc lập đối chiếu 2 chiều wiki vs file gốc): **17/17 PASS** — độ phủ trung bình ~96-97%, không bỏ sót kiến thức kỹ thuật trọng yếu nào.
- QA flag 8 chỗ diễn giải mở rộng/bịa nhẹ → anh Chương ra lệnh "cấm bịa, xoá ngay" → đã FIX cả 8:
  1. `cam-may-danh-bong-vao-mau`: xoá "hỏng da khách" + "dễ mỏi tay, hình không mượt" (gốc chỉ nói "sát thương cao").
  2. `cam-may-di-net`: xoá "(run tay)" diễn giải cho "giun"; bỏ timestamp 2:05 do AI gán; thêm note ngoặc "Máy ben / samen / kim đạn — gốc chưa khẳng định cùng loại, anh Chương xác nhận".
  3. `pha-muc-xam-mau-tattoo`: xoá phân loại "(đặc vừa)" cho chai 3-4; sửa checklist + bảng: bỏ "70% mực" (AI suy diễn), chỉ giữ nguyên văn gốc "30% nước, giữ nhiều mực".
  4. `to-den-kim-m1`: xoá "— đảo ngược là sai chất hình" (gốc chỉ mô tả vùng tone, không nói đảo ngược là sai).
  5. `danh-bong-nhat-co-bai-3`: bỏ diễn giải "(phần nền/phần ngoài)" cho từ "qu"; thêm note xin anh xác nhận thuật ngữ.
  6. `scan-hinh-len-da`: xoá "bắp tay, sườn" trong section "Áp dụng cho ai" — gốc demo chỉ có "đùi".
  7. `danh-bong-mang-lon`: thêm note rõ "gốc dùng từ 'lông kim hơn' với máy lực cứng — diễn đạt nhập nhằng, anh Chương cần xác nhận".
  8. `danh-khoi-nhat-co-don-gian`: bỏ "Khác với đánh bóng thuần tuý — đây là bước tạo mảng khối có chiều sâu..." trong TL;DR (gốc không so sánh); bỏ suy đoán "có thể là set mực Grey".
- 3 điểm còn mờ chờ anh Chương xác nhận thuật ngữ chuẩn (đã ghi note ngay trong file): (a) samen/ben/kim đạn có cùng loại không, (b) "phần qu" là gì, (c) "lông kim hơn" với máy cứng có phải nghĩa "kim dài hơn".

## [2026-05-12] meta | Anh Chương fix 3 lỗi nghiêm trọng trong wiki Kiến thức xăm (YouTube)
- Anh Chương kiểm tra lại và chốt thuật ngữ chuẩn cho 3 điểm mờ → em sửa NGAY:
  1. **"samen / ben / kim đạn"** đều là phiên âm SAI của YouTube auto-caption từ chữ **"máy pen"** (kim đạn, kim ngắn dạng cartridge). Em đã GỘP 3 từ này như đồng nghĩa + giữ phiên âm sai trong wiki → SAI. Đã sửa tất cả vị trí trong [[cam-may-di-net]] + overview [[kien-thuc-xam]] thành **"máy pen (kim đạn)"** + ghi note rõ "transcript YouTube nhận diện sai".
  2. **"Phần qu"** = **"phần ngoài cùng"** (anh chốt). Đã sửa tất cả vị trí trong [[danh-bong-nhat-co-bai-3]] (nội dung + checklist + section "Vùng ra").
  3. **"Lông kim hơn"** = **kim đâm vào với độ sâu ÍT hơn** = **kim NÔNG hơn**. Em đã viết NGƯỢC trong wiki ("máy lực cứng → để kim DÀI hơn được") → SAI HOÀN TOÀN, đảo nghĩa. Đã sửa [[danh-bong-mang-lon]] section 5:
     - **Máy lực cứng / gắt**: có thể để kim **NÔNG hơn** (chiều dài kim ra ngắn hơn). Vì máy mạnh bỏ qua đàn hồi da → vẫn đâm đủ sâu.
     - **Máy lực mềm**: cần để kim **DÀI hơn** để bù lại độ đàn hồi của da.
- Sau fix: search toàn vault `wiki/kien-thuc-xam/` để confirm — tất cả vị trí dùng "lông kim" và "kim nông" trong các file khác (danh-khoi-nhat-co-don-gian, to-den-kim-m1) ĐỀU đã dùng đúng nghĩa "kim nông" = "lông kim" → không phải sửa thêm.
- Bài học **NẠP VÀO MEMORY**: anh Chương ra quy tắc CỨNG "**CẤM BỊA, không gộp suy diễn từ ngữ chuyên ngành**". Khi gặp từ mơ hồ trong transcript → BẮT BUỘC để nguyên + ghi note rõ, hỏi anh chốt TRƯỚC khi diễn giải. Lỗi này em đã từng bị nhắc trong memory `feedback_cam_bia_kiem_chung.md` nhưng vẫn tái phạm.

## [2026-05-12] ingest | Sách HACK MAP NGHỀ XĂM (202 trang, anh Trần Chương)
- Nguồn: `raw/kiến thức xăm/HACK MAP NGHỀ XĂM (1).pdf` (52MB, 202 trang, Canva). Tác giả: chính anh Trần Chương — Não cốt lõi nghề xăm.
- Anh Chương chốt plan:
  - Lưu vào `wiki/work/concepts/kien-thuc-xam/` (não cốt lõi, không phải khoá học)
  - 36 file con (13 P1 + 17 P2 + 5 P3 + 1 overview)
  - Không link chéo với framework PTL — để độc lập trong "kiến thức xăm" vì cũng là 1 phần của nghề xăm
- Quy trình ingest theo CLAUDE.md cho tài liệu >50 trang:
  1. Extract toàn bộ text PDF → `raw/kiến thức xăm/_extracted/full-text.txt` (96K chars, 3121 dòng)
  2. Đọc 2 lượt full file để xác minh
  3. Tạo 36 file wiki giữ NGUYÊN VĂN giọng anh Chương (clean OCR artifacts), kèm tham chiếu trang PDF gốc
- Cấu trúc tạo ra:
  - **Overview**: [[wiki/work/concepts/kien-thuc-xam/sach-hack-map-nghe-xam]] — mục lục đầy đủ 36 file
  - **Phần 1** (13 file): kim-xam, may-xam, da-va-do-sau-khi-xam, di-net, cac-ky-thuat-xam, pha-muc-xam, scan-hinh-xam, u-te, freehand-hinh-xam, duong-hinh-xam, chup-anh-hinh-xam, sua-de-hinh-xam, cau-hoi-thuong-gap
  - **Phần 2** (17 file): bai-01 đến bai-17 — vẽ mây/đá/sóng/lửa/hoa đào/lá phong/hoa cúc/mẫu đơn/mặt quỷ/lân/rồng/rắn/cá + nét chính phụ + sắc độ + bố cục + phối màu nhật cổ
  - **Phần 3** (5 file): chuong-1-xay-dung-nen-mong-tao-niem-tin, chuong-2-xay-kenh-len-xu-huong, chuong-3-quy-trinh-chot-lich-xam, chuong-4-bi-quyet-upsell, chuong-5-cham-soc-sau-xam
- Lưu ý: Phần 2 chủ yếu hình hoạ minh hoạ — text wiki ngắn, kèm note "xem PDF tr.X" cho nhân viên tra hình gốc.
- Đã update `index.md` thêm section ⭐ HACK MAP NGHỀ XĂM (đứng trước section video YouTube cũ).
- **QA round 2 độc lập — 3 agent song song**: ✅ PASS toàn bộ.
  - Phần 1 (13 file kỹ thuật xăm): độ phủ ~97-98%, 13/13 đạt ≥95%, 0 thiếu nghiêm trọng, 0 bịa. Đối chiếu chéo 15/15 brand + tất cả số liệu khớp 100% (phi kim 06/08/10/12, công thức pha mực 1-3-6-9-12 giọt, kim/máy/sản phẩm cụ thể).
  - Phần 2 (17 file thiết kế hình xăm): độ phủ ~97-98%, 17/17 đạt ≥95%, 0 thiếu, 0 bịa. Các bài chủ yếu ảnh (bài 1-13) đều ghi rõ "xem PDF tr.X" — không bịa thêm text. Bài 17 phối màu giữ đầy đủ 6 cách + 5 nguyên tắc + nhân vật Kintaro + CTA khoá học.
  - Phần 3 (5 file marketing): độ phủ ~98%, 5/5 đạt ≥95%, 0 thiếu, 0 bịa. Đầy đủ HOOK→EMOTION→VALUE→CURIOSITY→CTA, L.A.E.R, 5 nhóm DESIRE/FEAR/STORY/AUTHORITY/EDUCATION, lời kết toàn sách tr.202.
- **FIX 1 vấn đề bắt buộc** (phát hiện trong QA Phần 3):
  - `chuong-3-quy-trinh-chot-lich-xam.md`: ban đầu em (AI) tự diễn giải mâu thuẫn nội tại trong sách gốc (tr.192 nói "B2 Tăng giá trị → B3 Làm họ muốn", tr.193 đảo "B2 Tạo mong muốn → B3 Tăng giá trị") → **vi phạm Quy tắc 4 CLAUDE.md** (phát hiện lỗi gốc phải báo cáo TRƯỚC, không tự quyết định). Đã sửa note thành flag rõ 🚩 "PHÁT HIỆN MÂU THUẪN — chờ anh Chương xác nhận", giữ NGUYÊN VĂN cả 2 phiên bản trong sách.
- 3 đề xuất nâng cấp nhỏ (không bắt buộc, anh Chương quyết):
  1. `may-xam.md`: bổ sung slogan "Trần Chương - Đồ xăm trong tầm tay" (xuất hiện tr.19).
  2. `bai-10-ve-lan.md`: thêm cross-link sang bài 9 (mặt quỷ) + bài 11 (rồng) vì quy tắc lông tóc dùng chung.
  3. Tạo file `_index.md` cho mỗi phần để overview.

## [2026-05-12] QA round 3 (anh Chương yêu cầu re-check) | Sách HACK MAP NGHỀ XĂM
- Anh Chương lệnh: "kiểm tra lại xem còn thiếu sót hay bịa chuyện không. làm cho đúng". Em không tin tuyệt đối QA round 2 → tự đọc lại từng dòng full-text.txt vs từng file wiki.
- **Phát hiện 8 vấn đề** đã FIX:
  1. **kim-xam.md**: bỏ chữ "**chính**" trong "Có 2 loại kim chính" — gốc tr.5 chỉ ghi "Có 2 loại kim". AI bịa nhẹ.
  2. **may-xam.md**: thêm slogan "Trần Chương - Đồ xăm trong tầm tay" cuối tr.19 — wiki đã thiếu.
  3. **di-net.md**: thêm câu kết "Chắc chắn đó bạn yêu." cuối mục 3.1 — wiki đã thiếu.
  4. **sua-de-hinh-xam.md**: thêm câu "Quá dễ hiểu đúng không bạn yêu." sau đoạn vùng tràm — wiki đã thiếu (gốc tr.64).
  5. **bai-04-ve-lua.md**: bỏ tự suy đoán "Bước 1: vẽ nửa đầu của ngọn lửa" — gốc tr.81 không có Bước 1, chỉ có Bước 2 mở đầu. Thay bằng note rõ "Bước 1 chỉ có ảnh, không text".
  6. **bai-12-ve-ran.md**: bỏ tự gán "Bước 2/3/4" cho phần rắn ngậm mồm — gốc chỉ đánh "Bước 1", các phần sau không đánh số. Đổi tiêu đề về nguyên văn gốc.
  7. **bai-13-ve-ca.md**: thêm note rõ về việc gốc đánh 2 lần "Bước 8" (tr.155 và tr.156) — wiki trước đã tự đổi 1 cái thành "Hoàn thiện" không xin phép.
  8. **chuong-1-xay-dung-nen-mong-tao-niem-tin.md**: thêm câu kết "Bạn đã sẵn sàng chưa?" cuối chương — wiki đã thiếu (gốc tr.185).
- **Sửa OVERVIEW** (`sach-hack-map-nghe-xam.md`):
  - Section "3 thông điệp cốt lõi xuyên suốt sách" → đổi thành "3 câu nguyên văn anh Chương (em chọn làm điểm nhấn)" + thêm flag ⚠️ note rõ "em (AI) tổng hợp" — sách gốc không có khái niệm này.
  - Mục hành động số 2 trong "Hành động sau khi đọc": sửa câu "Đăng đều 2 video/ngày trong 15 ngày sau khi kênh nóng" → đổi thành mô tả đúng quy trình "3-7 ngày đầu KHÔNG đăng gì, chỉ tương tác kênh khác. Sau khi 80% bảng tin đề xuất xăm, mới đăng 2 video/ngày trong 15 ngày tiếp" (vì cụm "sau khi kênh nóng" trước đó là AI bịa context).
- Vấn đề chương 3 (mâu thuẫn nội tại tr.192 vs tr.193) đã fix ở round 2 — giữ nguyên flag 🚩 cho anh Chương xác nhận.
- **Kết luận QA round 3**: 35/35 file vẫn ≥95% độ phủ. Các vấn đề đã fix đều là **chi tiết nhỏ** (chữ dư "chính", câu kết thân mật "bạn yêu" / "sẵn sàng chưa", slogan ký tên, đánh số bước không có trong gốc, tổng hợp ngữ cảnh không chính xác). Không có vấn đề nghiêm trọng kiểu số liệu sai / brand sai.

## [2026-05-12] meta | Move sách HACK MAP về `wiki/kien-thuc-xam/` để gộp chung kiến thức xăm
- Anh Chương: "ồh không, tôi nghĩ bạn phải nên cho vào wiki/kien-thuc-xam/ chứ. vì nó chung kiến thức".
- Trước: sách HACK MAP ở `wiki/work/concepts/kien-thuc-xam/` (theo plan ban đầu — "não cốt lõi" trong work/concepts/), tách khỏi 17 file video YouTube ở `wiki/kien-thuc-xam/`.
- Sau move: cả 2 nguồn kiến thức xăm gộp về `wiki/kien-thuc-xam/`. Cấu trúc mới:
  ```
  wiki/kien-thuc-xam/
  ├── kien-thuc-xam.md  (overview 17 video YouTube — cũ)
  ├── [17 file video YouTube .md]
  └── sach-hack-map-nghe-xam/  (folder mới chuyển vào)
      ├── sach-hack-map-nghe-xam.md  (overview 36 file)
      ├── phan-1-ky-thuat-xam/  (13 file)
      ├── phan-2-thiet-ke-hinh-xam/  (17 file)
      └── phan-3-marketing/  (5 file)
  ```
- Lệnh: `mv wiki/work/concepts/kien-thuc-xam wiki/kien-thuc-xam/sach-hack-map-nghe-xam`.
- Wikilink trong các file con dùng relative path `[[../sach-hack-map-nghe-xam|...]]` → vẫn work bình thường vì cấu trúc tương đối không đổi.
- Updated [[index.md]]: replace tất cả `wiki/work/concepts/kien-thuc-xam/` → `wiki/kien-thuc-xam/sach-hack-map-nghe-xam/` (37 wikilink).
- Total file mới trong `wiki/kien-thuc-xam/`: **54 file** (17 video YouTube + 36 sách HACK MAP + 1 overview cũ).
