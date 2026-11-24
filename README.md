# ĐỌC TRUYỆN OFFLINE ULTRA V8

Website đọc truyện cá nhân dạng **một file HTML**, ưu tiên lưu trữ cục bộ và sử dụng offline.

## Nội dung repository

- `index.html` — website Đọc Truyện Ultra V8.
- `.github/workflows/deploy.yml` — tự động triển khai lên GitHub Pages khi push lên `main`.
- `.nojekyll` — tắt xử lý Jekyll mặc định cho website tĩnh.

## Tính năng chính

- Thư viện truyện cá nhân, tìm kiếm, yêu thích và lọc truyện.
- Trình đọc, mục lục chương, dấu trang, ghi chú và đánh giá.
- Lưu tiến độ đọc, cấp bậc, XP và thống kê.
- Giọng đọc trình duyệt và danh sách phát.
- Thư viện video cục bộ (IndexedDB).
- Thùng rác truyện, khôi phục và xóa vĩnh viễn.
- Quản lý bộ truyện, thứ tự tập và danh sách nhân vật.
- Tóm tắt nhanh và gợi ý tên riêng bằng xử lý văn bản cục bộ.
- Sao lưu/khôi phục JSON; xuất TXT, HTML, EPUB; in/lưu PDF.
- Giao diện tối, hiệu ứng 3D và chế độ tập trung.

## Triển khai GitHub Pages

1. Tạo repository GitHub mới.
2. Tải các tệp trong gói này lên repository, giữ nguyên cấu trúc thư mục.
3. Đảm bảo `index.html` nằm ở thư mục gốc của repository.
4. Đẩy nội dung lên nhánh `main`.
5. Mở **Settings → Pages**.
6. Trong **Build and deployment → Source**, chọn **GitHub Actions**.
7. Mở tab **Actions** để theo dõi workflow `Deploy Đọc Truyện Ultra to GitHub Pages`.
8. Khi workflow hoàn tất, mở **Settings → Pages** để lấy địa chỉ website.

Workflow có thể chạy lại thủ công từ tab **Actions** bằng `workflow_dispatch`.

## Cập nhật website

Mỗi lần cập nhật `index.html` hoặc nội dung repository, commit và push lên nhánh `main`. GitHub Actions sẽ tự triển khai lại website.

## Lưu ý về dữ liệu và quyền riêng tư

- GitHub Pages là website công khai trên Internet. Không đưa truyện riêng tư, dữ liệu nhạy cảm hoặc bản sao lưu thư viện cá nhân vào repository công khai.
- Website lưu dữ liệu truyện trong bộ nhớ trình duyệt của thiết bị. Dữ liệu đó không tự đi theo repository và không tự đồng bộ giữa các thiết bị.
- Hãy xuất bản sao thư viện từ website trước khi đổi trình duyệt, xóa dữ liệu trình duyệt hoặc chuyển thiết bị.
- PIN trong website chỉ khóa giao diện cục bộ, không mã hóa nội dung đã lưu.
- Một số tính năng phụ thuộc trình duyệt; nhập PDF có thể cần tải PDF.js từ Internet, còn giọng đọc phụ thuộc giọng đọc hệ điều hành/trình duyệt.
- Tóm tắt và gợi ý nhân vật trong bản này là xử lý văn bản cục bộ, không phải dịch vụ AI đám mây.

## Công nghệ

HTML, CSS và JavaScript thuần; không cần cài Node.js hay chạy bước build để xuất bản GitHub Pages.

## Giấy phép

Chưa chỉ định giấy phép. Nếu muốn cho phép người khác sử dụng, sửa đổi hoặc phân phối mã nguồn, hãy chọn và thêm một tệp `LICENSE` phù hợp.
