Markdown
# 📚 Booknest - Website Bán Sách

**Booknest** là một dự án website bán sách trực tuyến được xây dựng nhằm cung cấp không gian mua sắm sách tiện lợi, giao diện thân thiện và quản lý hiệu quả.

---

## 🛠️ Công nghệ sử dụng
Dự án được phát triển dựa trên các công nghệ phổ biến sau:
* **Backend Framework:** Laravel (PHP)
* **Database:** MySQL
* **Frontend:** Bootstrap, HTML, CSS, JavaScript

---

## 👨‍💻 Chức năng chính

### 👤 Dành cho người dùng (Client)
* **Hệ thống tài khoản:** Đăng ký, đăng nhập và quản lý thông tin tài khoản cá nhân.
* **Khám phá sách:** Xem danh sách sản phẩm, chi tiết từng cuốn sách.
* **Tìm kiếm thông minh:** Tìm kiếm sách nhanh chóng theo từ khóa.
* **Yêu thích:** Thêm các cuốn sách yêu thích vào danh sách lưu trữ riêng.

### 👑 Dành cho quản trị viên (Admin)
* **Quản lý hệ thống:** Giao diện Admin trực quan để quản lý, thêm, sửa, xóa sản phẩm (sách) và các danh mục liên quan.

---

## 💻 Hướng dẫn chạy Project dưới máy cục bộ (Local)

Để khởi chạy dự án này trên máy tính của bạn, hãy thực hiện lần lượt các bước sau:

### 1. Clone project về máy
Mở terminal hoặc git bash và chạy lệnh:
```bash
git clone [https://github.com/haquangha/Booknest.git](https://github.com/haquangha/Booknest.git)
cd Booknest
2. Cài đặt các thư viện liên quan
Sử dụng Composer để cài đặt các package của Laravel:

Bash
composer install
3. Cấu hình môi trường (Environment)
Tạo file .env từ file mẫu cấu hình sẵn:

Bash
cp .env.example .env
(Lưu ý: Bạn cần mở file .env vừa tạo lên và cấu hình lại các thông số kết nối Database DB_DATABASE, DB_USERNAME, DB_PASSWORD cho đúng với máy của bạn).

4. Tạo Application Key
Bash
php artisan key:generate
5. Tạo cấu trúc bảng (Migrate Database)
Chạy lệnh sau để Laravel tự động tạo các bảng vào MySQL Database của bạn:

Bash
php artisan migrate
6. Khởi chạy Server
Cuối cùng, khởi động local development server:

Bash
php artisan serve
Sau khi chạy lệnh thành công, bạn mở trình duyệt và truy cập vào đường dẫn http://127.0.0.1:8000 để xem website.
