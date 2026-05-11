---
type: concept
tags: [email, deliverability, kỹ-thuật, domain, spam, infrastructure]
created: 2026-05-09
updated: 2026-05-09
sources: ["[[Khối 12 - Email marketing]]"]
---

# Email Deliverability Framework

> Nguồn: [[Khối 12 - Email marketing]] — IPS của Phạm Thành Long.

## Khái niệm cốt lõi

Email không phải "gửi đi" là xong. Mỗi email bị **Gmail/Outlook chấm điểm** và quyết định đưa vào: Hộp chính / Quảng cáo / Spam / Chặn.

## 3 trụ cột quyết định email vào đâu

| Trụ cột | Trọng số | Nội dung |
|---|---|---|
| Kỹ thuật | 30% | SPF, DKIM, DMARC, IP/domain reputation |
| Hành vi danh sách | 50% | Mở, click, báo spam, hủy đăng ký |
| Nội dung | 20% | Tiêu đề, từ khóa, tỉ lệ chữ/hình |

**Hành vi danh sách chiếm 50%** — đây là lý do list sạch quan trọng hơn content hay.

## Hạ tầng kỹ thuật bắt buộc

- **SPF**: Khai báo máy chủ nào được gửi với danh nghĩa domain.
- **DKIM**: Chữ ký số trên mỗi email.
- **DMARC**: Quy tắc xử lý email không xác thực.
- **BIMI**: Hiện logo trong Gmail (cần DMARC enforcement). Tăng open rate 10–15%.
- **rDNS**: IP gửi tra ngược ra đúng domain.
- Kiểm tra: `mxtoolbox.com` — cả 4 bản ghi phải xanh.

## Công cụ giám sát

- **Google Postmaster Tools**: Điểm uy tín domain với Gmail.
- **Microsoft SNDS**: Điểm với Outlook/Hotmail.
- **MXToolbox Blacklist Monitor**: Báo động blacklist.
- **Mail-tester.com**: Test điểm spam — ≥ 8/10 mới gửi.
- **GlockApps**: Test inbox placement.

## Dấu hiệu khủng hoảng & xử lý

Dấu hiệu: Open tụt >30%, spam complaint >0.3%, Postmaster báo "Low".

7 bước xử lý:
1. DỪNG mọi chiến dịch đại trà.
2. Kiểm tra blacklist tại MXToolbox.
3. Xem Google Postmaster Tools.
4. Phân tích chiến dịch gần nhất.
5. Chỉ gửi cho "list vàng" (tương tác trong 30 ngày).
6. Quay lại quy trình warm-up.
7. Sau 3–4 tuần điểm tốt mới mở rộng.

## Áp dụng vào việc nào

Bất kỳ dự án nào dùng email marketing — kể cả TPCN — phải thiết lập hạ tầng này trước khi gửi 1 email nào.
