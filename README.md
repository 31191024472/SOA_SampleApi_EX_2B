Kết Quả Đạt Được 

Tổng Quan Dự Án

- Cài đặt MongoDB và Mongo Compass.
- Tạo database và thêm dữ liệu mẫu (hai document).
- Cài đặt MongoDB Driver trong dự án .NET Core.
- Triển khai các tác vụ CRUD (Create, Read, Update, Delete).
- Tạo Swagger UI để thực thi và kiểm tra API.

Kết Quả Chi Tiết

1. Thiết Lập Cơ Sở Dữ Liệu
Cài đặt MongoDB: Đã hướng dẫn tải và cài đặt MongoDB từ trang chính thức.
Cài đặt Mongo Compass: Hỗ trợ quản lý và thao tác cơ sở dữ liệu một cách trực quan.
Thêm dữ liệu mẫu: Tạo hai document ban đầu:

[
  {
    "Name": "Design Patterns",
    "Price": 54.93,
    "Category": "Computers",
    "Author": "Ralph Johnson"
  },
  {
    "Name": "Clean Code",
    "Price": 43.15,
    "Category": "Computers",
    "Author": "Robert C. Martin"
  }
]

2. Triển Khai API

Cài đặt MongoDB Driver: Thêm thư viện MongoDB.Driver qua NuGet Package Manager.
Tạo Model:
- Book: Đại diện cho dữ liệu mỗi quyển sách.
- BookStoreDatabaseSettings: Cấu hình kết nối MongoDB.
Tạo Service:
- Lớp BooksService cung cấp các tác vụ CRUD.
Sử dụng Dependency Injection để truyền đối tượng cấu hình.

3. Tạo Controller

- BooksController: Quản lý các request HTTP gửi đến.
- Đã xây dựng các endpoint:
- GET /api/books: Lấy danh sách tất cả sách.
- GET /api/books/{id}: Lấy thông tin chi tiết của một quyển sách.
- POST /api/books: Thêm sách mới.
- PUT /api/books/{id}: Cập nhật sách.
- DELETE /api/books/{id}: Xóa sách.

4. Triển Khai Ứng Dụng

Cài đặt Swagger:
Kết nối Swagger UI để truy cập và thực thi các API.
Chạy Ứng Dụng:
Dòng https://localhost:7295/swagger/index.html để kiểm tra API.
Tác Động
Dự án cung cấp một hệ thống API linh hoạt, dễ sử dụng, cho phép quản lý dữ liệu sách một cách hiệu quả. Thực thi thành công các tác vụ CRUD và cung cấp giao diện Swagger trực quan.

