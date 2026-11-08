# BOY7X AI STUDIO — bản thử nghiệm độc lập

## Tính năng đang có
- Chọn một hoặc nhiều ảnh từ thiết bị.
- Khung hình dọc 9:16, ngang 16:9 hoặc vuông 1:1.
- Hiệu ứng zoom, zoom-out, pan và drift.
- Thêm một dòng chữ và nhạc nền (tùy khả năng trình duyệt).
- Ghi hình từ canvas và tải video xuống ngay trong trình duyệt.
- Không cần tài khoản, không gửi ảnh lên máy chủ.

## Cách chạy
Ứng dụng là PWA tĩnh. Để cài lên màn hình chính iPhone, cần xuất bản thư mục này lên một host HTTPS tĩnh (ví dụ GitHub Pages). Sau đó mở URL bằng Safari > Chia sẻ > Thêm vào Màn hình chính.

## Giới hạn quan trọng
- Đây là MVP dựng video chuyển động từ ảnh, KHÔNG phải mô hình AI sinh chuyển động vật lý thật.
- Phần AI Image-to-Video hiện là điểm chờ tích hợp. Muốn tạo chuyển động người/cảnh bằng AI cần một endpoint inference, API key và thường có hạn mức/chi phí. Không nhúng API key bí mật vào mã chạy trên trình duyệt.
- Khả năng xuất MP4/WebM và ghép âm thanh phụ thuộc trình duyệt/phiên bản iOS. Nếu Safari không hỗ trợ định dạng xuất, thử trình duyệt mới nhất hoặc dùng máy tính.
- Chạy local file có thể không bật PWA/offline; cần HTTPS để cài như ứng dụng.

## Triển khai miễn phí bằng GitHub Pages
1. Tạo repository GitHub mới, ví dụ `boy7x-ai-studio`.
2. Tải toàn bộ file trong thư mục này lên repository.
3. Vào Settings > Pages > Deploy from a branch > chọn `main` và `/root`.
4. Mở URL HTTPS do GitHub Pages cung cấp trên Safari iPhone.
5. Chọn Chia sẻ > Thêm vào Màn hình chính.

Không có backend, không có analytics, không có quảng cáo.
