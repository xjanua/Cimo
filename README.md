📌 1. Yêu cầu trước khi bắt đầu
Để chạy dự án mượt mà, hãy chắc chắn bạn đã cài đặt đầy đủ các công cụ sau:

✅ .NET 8 SDK (Tải tại dotnet.microsoft.com)
✅ MySQL 8.0 trở lên (Tải tại mysql.com)
✅ Visual Studio Code (hoặc IDE yêu thích của bạn)
✅ MySQL Workbench (hoặc bất kỳ công cụ quản lý MySQL nào bạn thích)
✅ Postman (Dùng để kiểm tra và trải nghiệm API)


📌 2. Tải mã nguồn dự án
Clone dự án về máy bằng lệnh:
git clone https://github.com/xjanua/BE_Cimo


📌 3. Thiết lập Database
Tạo một cơ sở dữ liệu mới trong MySQL với tên là Cimo.
Mở file appsettings.json trong thư mục dự án.
Cập nhật thông tin kết nối cơ sở dữ liệu bằng cách chỉnh sửa đoạn mã sau sao cho phù hợp với cấu hình của bạn:
{
  "AllowedHosts": "*",
  "ConnectionStrings": {
    "DefaultConnection": "Server=localhost;Port=3306;Database=Cimo;User=tên_người_dùng_của_bạn;Password=mật_khẩu_của_bạn;"
  }
}
Hãy thay tên_người_dùng_của_bạn và mật_khẩu_của_bạn bằng thông tin tài khoản MySQL của bạn để kết nối thành công!


📌 4. Start dự án.
Mở terminal.

dotnet ef migrations add InitialCreate

dotnet ef database update

dotnet run

📌 5. Kiểm tra các api hiện có.
http://localhost:5020/swagger/index.html

Localhost+cổng tuỳ thuộc vào cổng bạn setup
