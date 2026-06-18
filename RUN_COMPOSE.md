# Hướng dẫn khởi chạy hệ thống đa dịch vụ (Lab 05)

Dưới đây là các bước để khởi chạy toàn bộ stack (API, AI Service, Database) bằng Docker Compose.

**Yêu cầu:** Máy tính đã cài đặt Docker Desktop và hỗ trợ Compose v2.

### Bước 1: Khởi động hệ thống
Mở terminal tại thư mục gốc và chạy lệnh:
`docker compose up -d --build`

### Bước 2: Kiểm tra trạng thái (Readiness)
Đảm bảo cả 3 container đều có trạng thái `Up` hoặc `healthy`:
`docker compose ps`

### Bước 3: Dừng hệ thống
Khi không còn sử dụng, tắt toàn bộ stack và gỡ network:
`docker compose down`