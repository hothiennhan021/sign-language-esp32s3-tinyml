# Hệ thống nhận diện ngôn ngữ ký hiệu tay ứng dụng TinyML trên ESP32-S3

Đồ án môn **CE340.R11 – Trí tuệ nhân tạo cho hệ thống nhúng** – Khoa Kỹ thuật Máy tính, ĐH Công nghệ Thông tin (UIT).
GVHD: **Phạm Minh Quân**

## Giới thiệu
Thiết bị nhúng nhỏ gọn nhận diện ký hiệu tay (34 lớp: 24 chữ cái A–Z trừ J/Z và 10 chữ số) ngay trên vi điều khiển,
hỗ trợ giao tiếp cho người khiếm thính. Suy luận chạy hoàn toàn on-device (không cần máy tính/đám mây).

## Phần cứng
- ESP32-S3 WROOM N16R8 (16MB Flash, 8MB PSRAM, dual-core LX7 @240MHz)
- Camera OV3660 (3MP, giao tiếp DVP)
- DFPlayer Mini + loa (xuất âm thanh)
- WiFi Access Point + web server nội bộ (hiển thị kết quả trên điện thoại/laptop)

## Phần mềm
- TensorFlow Lite for Microcontrollers (lượng tử hóa int8), huấn luyện bằng Edge Impulse / TensorFlow
- Kiến trúc phân lớp Driver / Service / Application

## Cấu trúc repo
```
docs/        Báo cáo đề tài (.docx) và sơ đồ minh họa (docs/images)
firmware/    Mã nguồn ESP32-S3 (sẽ bổ sung)
model/       Dữ liệu/huấn luyện/mô hình TFLite (sẽ bổ sung)
```

## Thành viên
| MSSV | Họ và tên |
| --- | --- |
| 23520011 | Nguyễn Hoàng An |
| 23521062 | Trần Phạm Phúc Nguyên |
| 23521633 | Trịnh Hùng Tráng |
| 23521073 | Hồ Thiện Nhân |

## Trạng thái
Giai đoạn đề tài (báo cáo đề tài hoàn thành). Thiết kế chi tiết và thi công: đang thực hiện.
