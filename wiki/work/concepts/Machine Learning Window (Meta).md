---
type: concept
tags: [facebook, meta-ads, machine-learning, paid-media, ads-optimization]
created: 2026-05-09
updated: 2026-05-09
sources: ["[[Khối 4 - Chiến lược Facebook Fanpage]]"]
---

# Machine Learning Window (Meta)

## Khái niệm

**Machine Learning Window** (còn gọi là **learning phase**) là giai đoạn Meta Ads tự học để phân phối quảng cáo tối ưu hơn. Khi một ad set mới được tạo hoặc có thay đổi đáng kể (ngân sách, audience, creative, bid), Meta cần thu thập đủ dữ liệu để hiểu ai là người có khả năng thực hiện sự kiện tối ưu hoá nhất.

Trong thời gian này, hệ thống phân phối **không ổn định** — chi phí cao hơn, kết quả dao động mạnh hơn so với sau khi thoát learning phase.

## Cơ chế hoạt động

**Ngưỡng tối thiểu:** Một ad set cần đạt **≥50 sự kiện tối ưu hoá/tuần** để thoát learning phase và chuyển sang phân phối ổn định.

- Nếu ad set tối ưu cho "purchase" → cần ≥50 purchase/tuần
- Nếu tối ưu cho "lead" → cần ≥50 lead/tuần
- Nếu tối ưu cho "video view" → threshold thấp hơn, dễ thoát hơn

**Trạng thái hiển thị trong Ads Manager:**

| Trạng thái | Ý nghĩa |
|---|---|
| Learning | Đang trong learning phase — chưa ổn định |
| Learning Limited | Thiếu dữ liệu — không đủ sự kiện để học |
| Active | Đã thoát learning phase — phân phối ổn định |

**Learning Limited** là trạng thái nguy hiểm nhất — ad set sẽ phân phối không hiệu quả vô thời hạn nếu không được xử lý.

## Hậu quả khi chưa thoát learning phase

- Meta phân phối **không ổn định** — một ngày tốt, một ngày xấu
- CPC (cost per click) và CPL (cost per lead) **cao hơn 30-50%** so với sau khi hệ thống học xong
- Không thể đọc số liệu để ra quyết định chính xác — kết quả tuần 1 chưa phản ánh thực tế
- Nếu cắt budget sớm khi thấy "đỏ" → vừa tốn tiền, vừa không thu được insight

## Nguyên nhân thường gặp khiến bị kẹt learning phase

1. **Ngân sách quá nhỏ** — không đủ volume sự kiện trong 7 ngày
2. **Audience quá hẹp** — tệp nhỏ, ít người được tiếp cận
3. **Quá nhiều ad set nhỏ rải rác** — ngân sách bị chia vụn, từng ad set không đủ 50 sự kiện
4. **Thay đổi liên tục** — mỗi lần edit ad set là reset lại learning phase từ đầu
5. **Sự kiện tối ưu quá khó** — chọn "purchase" khi conversion rate còn rất thấp

## Cách thoát learning phase

| Cách | Khi nào áp dụng |
|---|---|
| **Tăng ngân sách** (tăng ≤20%/lần để tránh reset) | Khi volume sự kiện không đủ |
| **Mở rộng audience** (bỏ targeting hẹp, dùng Advantage+) | Khi tệp quá nhỏ |
| **Gộp ad set** (consolidation) | Khi có nhiều ad set nhỏ cùng mục tiêu |
| **Chọn sự kiện tối ưu dễ hơn** (lead → video view → reach) | Khi conversion rate thấp — dùng upper funnel trước |
| **Không edit ad set** trong 7 ngày đầu | Mọi lúc — tránh reset không cần thiết |

## Quy tắc đọc số liệu

- **Không kết luận trong 7 ngày đầu** — đây là giai đoạn học, số liệu chưa ổn
- Đọc kết quả theo **cửa sổ 3-7 ngày** tối thiểu sau khi thoát learning phase
- Nếu sau 7 ngày vẫn "Learning Limited" → gộp ad set hoặc tăng budget hoặc chuyển sang sự kiện dễ hơn

## Áp dụng cho TPCN

**Lỗi phổ biến nhất khi bắt đầu chạy ads TPCN:**

Tạo 5-10 ad set nhỏ rải rác (ví dụ: "phụ nữ 30-40", "phụ nữ 40-50", "nam giới quan tâm sức khoẻ"...) mỗi ad set ngân sách $10-20/ngày → tổng ngân sách rải mỏng → không ad set nào đạt 50 sự kiện/tuần → toàn bộ bị "Learning Limited" → tốn tiền không ra kết quả.

**Cách làm đúng cho TPCN:**

1. Bắt đầu với **1-2 ad set** ngân sách đủ lớn (đủ để tạo ≥50 sự kiện tối ưu/tuần)
2. Dùng **Advantage+ audience** — để Meta tự tìm người phù hợp thay vì vi-targeting
3. Giai đoạn đầu, tối ưu cho sự kiện **dễ hơn** (video view, landing page view) trước khi chuyển sang lead/purchase
4. Sau khi có đủ dữ liệu và tệp retarget → mới tách ad set theo funnel stage

**Liên kết:** [[Conversions API (CAPI)]] | [[Blended MER]] | [[Khối 4 - Chiến lược Facebook Fanpage]]
