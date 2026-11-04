# Session10 - Bài 1: Thiết kế tài nguyên theo Naming Convention

## Tài nguyên Bác sĩ

Sử dụng danh từ số nhiều `doctors` và tiền tố phiên bản API `/api/v1`.

| STT | Thao tác | HTTP Method | URL |
| --- | --- | --- | --- |
| 1 | Lấy danh sách toàn bộ bác sĩ | GET | `/api/v1/doctors` |
| 2 | Lấy thông tin chi tiết một bác sĩ theo ID | GET | `/api/v1/doctors/{id}` |
| 3 | Thêm mới một bác sĩ | POST | `/api/v1/doctors` |
| 4 | Cập nhật thông tin bác sĩ | PUT | `/api/v1/doctors/{id}` |
| 5 | Xóa bác sĩ khỏi hệ thống | DELETE | `/api/v1/doctors/{id}` |

`{id}` là mã bác sĩ cụ thể, ví dụ `/api/v1/doctors/1`.

URL dùng chữ thường và danh từ số nhiều. HTTP Method xác định hành động, vì vậy không đặt các động từ như getAllDoctors, createDoctor, updateDoctor hoặc deleteDoctor vào URL.

POST và PUT gửi thông tin bác sĩ trong request body dạng JSON. PUT dùng để cập nhật đầy đủ thông tin của bác sĩ theo ID.
