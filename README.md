# IELTS Coach 7.0 (PWA)

Ứng dụng tĩnh (không cần máy chủ, không cần build). Gồm: index.html, sw.js, manifest.webmanifest, thư mục icons.

## Đưa lên Netlify
Cách nhanh: vào https://app.netlify.com/drop, giải nén file zip rồi kéo thả cả thư mục vào trang.
Hoặc: đưa các file lên một repo GitHub, trong Netlify chọn "Add new site" → "Import an existing project", để trống Build command, Publish directory = `.` (file netlify.toml đã cấu hình sẵn).

## Đưa lên GitHub Pages
1. Tạo repo mới, tải toàn bộ file trong thư mục này lên nhánh `main` (giữ cả file .nojekyll).
2. Vào Settings → Pages → Source: "Deploy from a branch", chọn `main` và thư mục `/ (root)`, bấm Save.
3. Sau 1–2 phút, ứng dụng chạy tại https://<tên-bạn>.github.io/<tên-repo>/

Mọi đường dẫn trong app là đường dẫn tương đối nên chạy được cả ở thư mục con của GitHub Pages.

## Cài về thiết bị (cần mở bằng https)
- Android (Chrome): menu ⋮ → "Cài đặt ứng dụng" / "Thêm vào màn hình chính", hoặc bấm nút "Cài ứng dụng" trong app.
- iPhone/iPad (Safari): nút Chia sẻ → "Thêm vào Màn hình chính".
- Máy tính (Chrome/Edge): bấm biểu tượng cài đặt ở thanh địa chỉ, hoặc nút "Cài ứng dụng" trong app.

## Lưu ý
- Tiến độ lưu trong trình duyệt của từng thiết bị. Dùng nút "Sao lưu dữ liệu" / "Khôi phục" để chuyển sang thiết bị khác.
- Sau khi cập nhật file, đổi số phiên bản trong sw.js (ví dụ ielts-coach-v2) để thiết bị tải bản mới.
- App không gửi thông báo khi đã đóng; hãy đặt báo thức hằng ngày trên điện thoại.
