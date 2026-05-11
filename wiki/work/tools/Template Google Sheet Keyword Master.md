---
type: tool
tags: [keyword, template, google-sheet, ips, khoi-2]
created: 2026-05-09
updated: 2026-05-09
sources: ["[[Khối 2 - Cách tìm kiếm từ khoá]]"]
---

# 📊 Template Google Sheet Keyword Master

> Template Google Sheet để **quản lý toàn bộ keyword** của tiệm/công ty TPCN. Vận hành hằng ngày, review hằng tuần. Mọi quyết định content + ads đều bắt đầu từ file này.

## 🗂️ Cấu trúc Sheet

Tạo Google Sheet tên `Keyword Master List - TPCN`. Có **4 tab chính**:
1. **Master** — danh sách chính (20 cột)
2. **Negative Keywords** — keyword loại trừ cho ads
3. **Seed Library** — kho seed keyword chưa mở rộng
4. **Cluster Map** — sơ đồ cluster + pillar + supporting
5. **Monthly Review** — bảng review hằng tháng

---

## 📋 Tab 1 — Master (20 cột A→T)

| Cột | Tên | Kiểu dữ liệu | Ghi chú |
|---|---|---|---|
| A | Keyword | text | viết thường, không dấu thừa |
| B | Nhóm | dropdown | Chính / Liên quan / Người mua tìm |
| C | Intent | dropdown | Informational / Navigational / Commercial / Transactional |
| D | Funnel | dropdown | TOFU / MOFU / BOFU |
| E | Volume | number | từ Keyword Planner / Ahrefs |
| F | KD | number | từ Ahrefs / Mangools |
| G | CPC | number (VND) | từ Keyword Planner |
| H | Trend | dropdown | Tăng / Giảm / Phẳng / Mùa |
| I | SERP feature | text | featured snippet, map pack, video… |
| J | Cluster | text | tên cluster nội dung (vd: "collagen tuổi 35") |
| K | Kênh dự kiến | dropdown | Blog / YouTube / TikTok / Email / Ads… |
| L | Nội dung dự kiến | text | tên bài/video |
| M | Người phụ trách | text | tên nhân viên |
| N | Ngày dự kiến đăng | date | YYYY-MM-DD |
| O | Trạng thái | dropdown | Chưa làm / Đang làm / Đã đăng / Cần cập nhật |
| P | URL nội dung | URL | sau khi đã đăng |
| Q | Position hiện tại | number | cập nhật hàng tuần từ GSC |
| R | Click 30 ngày | number | từ GSC |
| S | Conversion 30 ngày | number | tự đếm hoặc từ GA |
| T | Ghi chú | text | lưu ý đặc biệt |

---

## 📋 Tab 2 — Negative Keywords

Danh sách keyword **loại trừ cho Google Ads / Facebook Ads**. Ngăn đốt tiền vào click rác.

**Cấu trúc:**
| Negative keyword | Lý do loại trừ | Campaign áp dụng | Ngày thêm |
|---|---|---|---|

**Ví dụ TPCN:**
| `miễn phí` | Khách không sẵn sàng trả | Tất cả | 2026-05-09 |
| `mẹo dân gian` | Đi ngược thông điệp brand (TPCN khoa học) | Conversion campaign | 2026-05-09 |
| `tự làm tại nhà` | Sản phẩm khác hẳn | TPCN sản phẩm | 2026-05-09 |
| `cho trẻ em dưới 1 tuổi` | Đối tượng không khớp | Tất cả | 2026-05-09 |

→ Mỗi chiến dịch ads cần **≥ 30 negative keyword**, cập nhật **hàng tuần** từ Search Term Report.

---

## 📋 Tab 3 — Seed Library

Kho **seed keyword chưa mở rộng**. Khi bí, mở Seed Library lấy seed mới đưa qua [[AI Prompts - Keyword Research|7 AI prompt]] mở rộng.

**Cấu trúc:**
| Seed | Nguồn (HSKH/đối thủ/voice/trend) | Persona liên quan | Đã mở rộng (Y/N) | Ngày thêm |
|---|---|---|---|---|

---

## 📋 Tab 4 — Cluster Map

Sơ đồ tổ chức **pillar + supporting** keyword.

**Cấu trúc:**
| Cluster name | Pillar keyword | Supporting keywords (5-10) | Persona | Funnel | Status |
|---|---|---|---|---|---|

**Ví dụ TPCN:**
| Collagen tuổi 35 | "collagen cho phụ nữ 35 tuổi" | "collagen loại nào tốt 35t / collagen có hại không / liều dùng collagen 35t / collagen kết hợp vitamin C" | Phụ nữ 35-45 lo lão hoá | MOFU | Đang triển khai |

---

## 📋 Tab 5 — Monthly Review

Review tổng hằng tháng — đánh giá performance từng cluster.

**Cấu trúc:**
| Cluster | Số bài đã đăng | Tổng impression | Tổng click | Avg position | Lead/Sale | Đánh giá | Hành động tháng sau |
|---|---|---|---|---|---|---|---|

---

## 👁️ 4 View Filter chuẩn (sau khi setup, lưu lại để dùng nhanh)

### View "Top priority"
- Filter: Rubric ≥ 8 (hoặc Volume ≥ 100 + KD ≤ 30 + Intent khớp)
- Sort: Volume DESC
- → Danh sách keyword làm trong 30 ngày

### View "Quick wins"
- Filter: KD ≤ 15 AND Volume ≥ 100
- → Keyword dễ rank, làm trước để có winning early

### View "Need update"
- Filter: Trạng thái = "Đã đăng" AND Position > 10
- → Nội dung cũ tụt rank, cần refresh

### View "Local"
- Filter: Keyword chứa "[tên thành phố]" hoặc "gần đây"
- → Local keyword cho Google Business Profile + Map Pack

---

## 📥 CSV Mẫu (copy paste vào Google Sheet)

```csv
Keyword,Nhóm,Intent,Funnel,Volume,KD,CPC,Trend,Kênh,Trạng thái
collagen cho phụ nữ tuổi 35 dạng nước,Liên quan,Commercial,MOFU,320,8,18000,Phẳng,Blog,Chưa làm
collagen có tác dụng phụ không,Liên quan,Informational,TOFU,1240,18,3500,Tăng,YouTube,Chưa làm
mua collagen chính hãng nhật,Người mua tìm,Transactional,BOFU,890,22,28000,Tăng,Landing,Đang làm
collagen loại nào tốt nhất 2026,Liên quan,Commercial,MOFU,720,28,12000,Tăng,Blog,Chưa làm
TPCN tăng đề kháng cho người già,Liên quan,Informational,TOFU,540,15,4200,Phẳng,Blog,Chưa làm
viên ngủ ngon cho người mất ngủ kinh niên,Liên quan,Commercial,MOFU,420,12,8500,Phẳng,Blog+TikTok,Chưa làm
TPCN giảm cân an toàn,Người mua tìm,Commercial,MOFU,2400,32,18000,Mùa,TikTok+Ads,Chưa làm
```

---

## 🔄 Tích hợp với Google Search Console

Cập nhật cột Q-R-S **mỗi thứ 2 hằng tuần**:

1. Vào search.google.com/search-console
2. Performance → 30 ngày qua
3. Filter Query trong master list → copy Position + Click + Impression
4. Paste vào Sheet (cột Q-R)
5. Cluster nào tụt rank > 5 vị trí → tạo task refresh content

---

## 🔗 Liên quan

- [[AI Prompts - Keyword Research]]
- [[Checklist Keyword Research]]
- [[Khối 2 - Cách tìm kiếm từ khoá]]
- [[Map keyword vào 7 kênh]]
