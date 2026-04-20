# Website-Buy-food

Dự án Website-Buy-food là một ứng dụng web thương mại điện tử chuyên cung cấp nền tảng đặt và mua đồ ăn trực tuyến. Dự án được xây dựng dựa trên nền tảng Java Web, tích hợp giao diện người dùng bằng CSS và JavaScript.

## Công nghệ sử dụng

- Ngôn ngữ lập trình chính: Java
- Giao diện (Frontend): HTML/JSP, CSS, JavaScript
- Cơ sở dữ liệu: SQL (tệp demosql.sql)
- Môi trường phát triển (IDE): NetBeans
- Công cụ Build: Apache Ant (build.xml)

## Cấu trúc thư mục

- src/: Chứa toàn bộ mã nguồn Java (Controllers, Models, DAO, kết nối DB,...).
- web/: Chứa các tài nguyên giao diện người dùng (file JSP, HTML, CSS, JavaScript) và thư mục WEB-INF.
- lib/: Chứa các thư viện .jar cần thiết (như JDBC Driver) để dự án hoạt động.
- build/: Thư mục được tự động sinh ra khi build dự án, chứa các file đã được biên dịch.
- nbproject/: Chứa các file cấu hình dự án của NetBeans IDE.
- demosql.sql: File script chứa cấu trúc bảng và dữ liệu mẫu dùng để khởi tạo cơ sở dữ liệu.
- build.xml: File cấu hình dùng để build dự án thông qua Apache Ant.

## Hướng dẫn cài đặt và chạy dự án

### Yêu cầu hệ thống

- JDK (Java Development Kit): Phiên bản 8 trở lên.
- IDE: Khuyến nghị sử dụng NetBeans IDE để tương thích tốt nhất với thư mục nbproject.
- Server: Apache Tomcat.
- Hệ quản trị CSDL: Hệ quản trị tương thích với file demosql.sql (thường là SQL Server hoặc MySQL).

### Các bước cài đặt

**Bước 1: Tải dự án về máy**
Tải mã nguồn từ kho lưu trữ về máy tính của bạn và giải nén.

**Bước 2: Thiết lập Cơ sở dữ liệu**
- Mở hệ quản trị cơ sở dữ liệu của bạn.
- Mở và thực thi (run) file demosql.sql có trong thư mục gốc của dự án để tạo CSDL và các bảng dữ liệu cần thiết.

**Bước 3: Mở dự án trong NetBeans**
- Khởi động NetBeans IDE.
- Chọn File > Open Project và trỏ đường dẫn tới thư mục dự án vừa tải về.

**Bước 4: Cấu hình kết nối CSDL và thư viện**
- Truy cập vào các class chứa cấu hình Database (thường nằm trong thư mục src) để chỉnh sửa lại thông tin URL, Username và Password sao cho khớp với CSDL trên máy của bạn.
- Kiểm tra xem các thư viện trong thư mục lib/ (đặc biệt là JDBC driver) đã được nhận diện chưa. Nếu chưa, hãy chuột phải vào phần Libraries trong NetBeans > Chọn Add JAR/Folder và thêm các file .jar từ thư mục lib/ vào.

**Bước 5: Cấu hình Server và Chạy ứng dụng**
- Chuột phải vào tên dự án trong NetBeans, chọn Properties > Run.
- Trong mục Server, hãy chọn Apache Tomcat.
- Nhấn nút Run (hoặc phím tắt F6) để bắt đầu chạy dự án. Trình duyệt sẽ tự động mở trang chủ của ứng dụng.
