---
type: concept
tags: [zalo, oa, push, broadcast, zns, mxh, crm, retention]
created: 2026-05-09
updated: 2026-05-09
sources: ["[[Khối 8 - MXH khác Zalo]]"]
qa: "2026-05-09 — đã fix bảng KPI bịa số benchmark chưa có trong nguồn gốc"
---

# Zalo OA Push Strategy

## Định nghĩa

Framework quản lý việc gửi tin nhắn chủ động từ Zalo Official Account đến follower — **đúng tầng, đúng thời điểm, đúng phân khúc** — nhằm tối đa conversion và LTV mà không vi phạm chính sách nền tảng hoặc luật bảo vệ dữ liệu cá nhân.

---

## Ba tầng tin nhắn OA

| Tầng | Loại tin | Vai trò | Thời gian gửi | Chi phí |
|---|---|---|---|---|
| **Tầng 1** | Tin tư vấn (chat 1:1) | Xử lý nhu cầu nóng, chốt hội thoại | 24/24 | Phụ thuộc gói OA |
| **Tầng 2** | Broadcast (tin truyền thông) | Nội dung cô đọng + CTA theo phân khúc | 6:00–19:59 | Theo quota gói |
| **Tầng 3** | ZNS / ZBS Template Message | Giao dịch: xác nhận đơn, nhắc lịch, payment request, tái kích hoạt | Ngay theo sự kiện | 200–300đ/tin thành công |

**Nguyên tắc phân tầng:**
- Không dùng broadcast để xử lý nhu cầu nóng
- Không dùng ZNS cho nội dung marketing thuần
- Không gửi broadcast ở giờ ngoài khung 6:00–19:59

---

## Push Schedule Framework

### Broadcast Timing A/B Test
```
Khung sáng:   7:30 — người dùng chuẩn bị đi làm, kiểm tra điện thoại
Khung trưa:  11:45 — nghỉ trưa, xem điện thoại nhiều
Khung chiều: 17:45 — tan ca, chuẩn bị về
```
→ A/B test 3 khung với cùng nội dung → chọn khung có open rate và click rate cao nhất theo từng phân khúc

### ZNS Trigger Timeline (đặc biệt quan trọng cho TPCN)
```
D+0:   Xác nhận đơn (ngay khi đặt hàng)
D+1:   Hướng dẫn sử dụng (khi dự kiến giao hàng)
D+30:  Xin đánh giá + hỏi kết quả ban đầu
D+75:  Nhắc bổ sung (cho chu kỳ 3 tháng) — "Còn ~15 ngày nữa hết hàng"
D+90:  Reorder CTA — "Đặt lại để không bị gián đoạn hiệu quả"
D+150: Nhắc bổ sung (cho chu kỳ 6 tháng)
D+180: Win-back nếu chưa mua lại
```

---

## Phân khúc Push theo RFM

| Phân khúc | Hành động push |
|---|---|
| **VIP** (R↑ F↑ M↑) | Broadcast ưu đãi sớm + ZNS nhắc gia hạn + invite sự kiện riêng |
| **Trung thành** (F≥2, M trung bình) | Broadcast chu kỳ 2x/tuần + ZNS nhắc tái mua |
| **Mới** (F=1) | Welcome flow 30 ngày: hướng dẫn → xin đánh giá → gợi ý thêm SP |
| **Ngủ quên** (R>60 ngày) | Win-back: 1 tin "Đã lâu chưa gặp" + cập nhật nhu cầu |
| **Lạnh** (R>180 ngày) | Retarget Ads + 1 tin win-back cuối → nếu không phản hồi → loại khỏi broadcast |

---

## Quy tắc chống spam và compliance

**Nền tảng:**
- Zalo OA có cơ chế phát hiện luồng gửi tin gây phiền → hạn chế tự động
- Broadcast bị giới hạn theo quota của gói OA
- Không bắn tin hàng loạt không phân khúc

**Pháp lý (sau 2026):**
- Luật Bảo vệ dữ liệu cá nhân VN (hiệu lực 1/1/2026): phải xin quyền tương tác đúng cách, lưu vết đồng ý
- Phải cung cấp lối thoát rõ ràng: [Tạm dừng nhận thông báo] [Hủy theo dõi ưu đãi]

**Cá nhân hóa an toàn:**
- Chỉ dùng dữ liệu khách đã chủ động cung cấp
- Không đoán hành vi từ dữ liệu bên thứ ba không có đồng ý
- Cá nhân hóa phải đứng sau đồng ý và chất lượng dữ liệu

---

## KPI theo dõi Push Strategy

> **Lưu ý:** Zalo OA chưa công bố benchmark chuẩn chính thức cho open rate/click rate/delivery rate. Các KPI dưới đây là chỉ số cần tự đo và tối ưu nội bộ — không phải con số benchmark ngành đã được kiểm chứng.

| KPI | Ghi chú theo dõi |
|---|---|
| Open rate broadcast | Đo A/B test 3 khung giờ; theo dõi xu hướng tăng/giảm theo tuần |
| Click rate broadcast | Đo theo từng phân khúc nhãn; nội dung phù hợp nhóm → click rate cao hơn |
| ZNS delivery rate | Theo dõi qua OA Analytics; số điện thoại không hợp lệ → cần clean data |
| ZNS conversion rate (tái mua) | Đo bằng cách gắn tracking: khách nào mua sau khi nhận ZNS nhắc bổ sung |
| Unsubscribe rate | Nếu tăng đột biến → kiểm tra nội dung broadcast gần nhất và tần suất gửi |
| Spam report rate | Chỉ số sức khỏe OA; nếu cao → Zalo tự động hạn chế quota broadcast |

---

## Sai lầm phổ biến

1. **Broadcast như email marketing cũ**: gửi cho tất cả follower cùng 1 nội dung → open rate thấp, spam rate cao, quota cạn nhanh
2. **Không set ZNS theo chu kỳ sản phẩm**: gửi nhắc bổ sung quá sớm hoặc quá muộn → mất cơ hội reorder
3. **Không cá nhân hóa tên và sản phẩm trong ZNS**: cảm giác robotic → conversion thấp
4. **Không đo từng trigger riêng**: không biết trigger nào sinh doanh thu, trigger nào gây unsubscribe
5. **Bỏ qua lối thoát cho khách**: không có nút "Tạm dừng" → khách block OA thay vì pause

---

## Liên quan

- [[Funnel Zalo OA cho TPCN]] — toàn bộ hành trình từ quan tâm → mua → tái mua
- [[Khối 8 - MXH khác Zalo]] — nguồn gốc framework
- [[Retention Curve Analysis]] — đo cohort retention theo thời gian
- [[LRM]] — logic phân phối nội dung theo nền tảng
