WedService_Nhom3
================

AAA
Đề tài: Thiết kế webservice bán Giày Patin
Sinh viên: 	Nguyễn Văn Thơm		3110410144
               	Trần Hà Phước Trường	3110410166
               	Lê Nguyễn Trung Tính	3110410153


I. Giới thiệu
 Project WebGiayPatin được xây dựng nhằm cung cấp các chức năng để quản lý cho người dùng là Admin và người dùng là người mua hàng online.
 Trong đó các chức năng quản lý sử dụng Winform, các chức năng cho người dùng sử dụng ASP.NET MVC 4 và xây dựng webservice dựa trên WCF, 
 database được cài đặt trên SQL Server 2008.

II. Thiết kế, các chức năng
1. Thiết kế
 - WCF: xây dựng web service.
 - Winform: sử dụng xây dựng các chức năng quản lý.
 - ASP.NET MVC 4: sử dụng thiết kế website bán hàng.
2. Các chức năng // Tất cả các chức năng là do tự viết hoặc đẵ được chỉnh sửa để phù hộp với bài
 Chức năng trên Winform: WindowsFormGiayPatin
 - Quản lý Sản phẩm: WindowsFormGiayPatin/AllUserControl/Main_SanPham.cs
 + Thêm sản phẩm: 	 WindowsFormGiayPatin/AllUserControl/Main_SanPham.cs
 + Xóa sản phẩm:	 WindowsFormGiayPatin/AllUserControl/Main_SanPham.cs
 + Sửa sản phẩm:	 WindowsFormGiayPatin/AllUserControl/Main_SanPham.cs
 + Tìm kiếm sản phẩm:	 WindowsFormGiayPatin/AllUserControl/Main_SanPham.cs
 - Quản lý Người dùng: WindowsFormGiayPatin/AllUserControl/Main_NguoiDung.cs
 + Thêm người dùng:	     WindowsFormGiayPatin/AllUserControl/Main_NguoiDung.cs
 + Xóa người dùng:	     WindowsFormGiayPatin/AllUserControl/Main_NguoiDung.cs
 + Sửa người dùng:	     WindowsFormGiayPatin/AllUserControl/Main_NguoiDung.cs
 + Tìm kiếm người dùng:     WindowsFormGiayPatin/AllUserControl/Main_NguoiDung.cs
 - Quản lý Hóa đơn bán: WindowsFormGiayPatin/AllUserControl/Main_HoaDonBan.cs
 + Thêm hóa đơn bán:	      WindowsFormGiayPatin/AllUserControl/Main_HoaDonBan.cs
 + Sửa hóa đơn bán (cập nhật trạng thái): WindowsFormGiayPatin/AllUserControl/Main_HoaDonBan.cs
 + Tìm kiếm hóa đơn bán:    WindowsFormGiayPatin/AllUserControl/Main_HoaDonBan.cs
 - Quản lý Hóa đơn nhập: WindowsFormGiayPatin/AllUserControl/Main_HoaDonNhap.cs
 + Thêm hóa đơn nhập:          WindowsFormGiayPatin/AllUserControl/Main_HoaDonNhap.cs
 + Tìm kiếm hóa đơn nhập:     WindowsFormGiayPatin/AllUserControl/Main_HoaDonNhap.cs
 - Quản lý Phân loại: WindowsFormGiayPatin/AllUserControl/Main_PhanLoai.cs
 + Thêm phân loại:	WindowsFormGiayPatin/AllUserControl/Main_PhanLoai.cs
 + Sửa phân loại:	WindowsFormGiayPatin/AllUserControl/Main_PhanLoai.cs
 + Xóa phân loại:	WindowsFormGiayPatin/AllUserControl/Main_PhanLoai.cs
 + Tìm kiếm phân loại:	WindowsFormGiayPatin/AllUserControl/Main_PhanLoai.cs
 - Quản lý Thống kê:		  WindowsFromGiayPatin/AllUserControl/Main_ThongKe.cs
 + Thống kê hóa đơn bán theo ngày:  WindowsFromGiayPatin/AllUserControl/Main_ThongKe.cs
 + Thống kê hóa đơn bán theo tháng: WindowsFromGiayPatin/AllUserControl/Main_ThongKe.cs
 + Thống kê hóa đơn bán theo năm:   WindowsFromGiayPatin/AllUserControl/Main_ThongKe.cs
 + Tìm kiếm thống kê:		  WindowsFromGiayPatin/AllUserControl/Main_ThongKe.cs
Chức năng trên website:WebGiayPatin
 - Hiện sản phẩm theo loại, sản phẩm nổi bật, sản phẩm mới: WebGiayPatin/Controllers/DefaultController.cs
 - Tìm kiếm: tìm kiếm cơ bản, tìm kiếm nâng cao:	 WebGiayPatin/Controllers/DefaultController.cs
 - Giỏ hàng: thêm sản phẩm vào giỏ hàng, xóa sản phẩm trong giỏ hàng, cập nhật số lượng sản phẩm trong giỏ hàng, thanh toán hóa đơn: WebGiayPatin/Controllers/GioHangController.cs
 - Người dùng quản lý hóa đơn: tìm kiếm hóa đơn, sửa trạng thái hóa đơn (hủy hóa đơn): WebGiayPatin/Controllers/UserController.cs
 - Tài khoản người dùng: người dùng đăng ký tài khoản, người dùng đăng nhập, đổi mật khẩu, đổi thông tin người dùng: WebGiayPatin/Controllers/UserController.cs
Chức năng trên WCF: 
- Thực hiện các chức năng của winform yêu cầu WedService/AdminWinform.svc 
+ Người dùng:
	Tìm kiếm tất cả người dùng
	Tìm kiếm người dùng theo tên đăng nhập
	Ktra đăng nhập
	Thêm người dùng
	Xóa người dùng
	Sửa người dùng
+ Sản Phẩm:
	Tìm kiếm tất cả sản phẩm
	Tìm kiếm sản phẩm theo tên
	Tìm kiếm sản phẩm theo mã
	Thêm số lượng sản phẩm
	Xóa số lượng sản phẩm
	Thêm sản phẩm
	Xóa sản phẩm
	Sửa sản phẩm
+ Phân loại
	Tìm tất cả phân loại
	Tìm phân loại theo mã
	Thêm phân loại
	Xóa phân loại
	Sửa phân loại
+ Hóa đơn bán
	Tìm tất cả hóa đơn bán
	Tìm hóa đơn bán theo mã
	Thêm hóa đơn bán
	Sửa hóa đơn bán
+ Chi tiết hóa đơn bán
	Tìm chi tiết hóa đơn bán theo mã hóa đơn
	Thêm chi tiết hóa đơn bán	
+ Hóa đơn nhập
	Tìm tất cả hóa đơn nhập
	Tìm hóa đơn bán theo mã
	Thêm hóa đơn nhập
+ Chi tiết hóa đơn nhập
	Tìm chi tiết hóa đơn nhập theo mã hóa đơn
	Thêm chi tiết hóa đơn nhập
+ Thống kê
	Thống kê theo ngày
	Thống kê theo tháng
	Thống kê theo năm
- Thực hiện các chức năng của wedsite yêu cầu WedService/UserWed.svc
+ Người dùng:
	Tìm kiếm tất cả người dùng
	Tìm kiếm người dùng theo tên đăng nhập
	Ktra đăng nhập
	Thêm người dùng
	Sửa người dùng (thông tin đăng nhập)
	Sửa người dùng (thông tin cá nhân)
+ Sản Phẩm:
	Tìm kiếm tất cả sản phẩm
	Tìm kiếm sản phẩm theo sản phẩm mới
	Tìm kiếm sản phẩm theo sản phẩm nổi bậc
	Tìm kiếm sản phẩm theo mã
	Tìm kiếm sản phẩm theo khuyến mãi
	Tìm kiếm sản phẩm theo phân loại
	Thêm số lượng sản phẩm
	Xóa số lượng sản phẩm
+ Phân loại
	Tìm tất cả phân loại
	Tìm phân loại theo mã
+ Hóa đơn bán
	Tìm tất cả hóa đơn bán
	Tìm hóa đơn bán theo mã
	Thêm hóa đơn bán
	Sửa hóa đơn bán
+ Chi tiết hóa đơn bán
	Tìm chi tiết hóa đơn bán theo mã hóa đơn
	Thêm chi tiết hóa đơn bán	
+ tìm kiếm
	Tìm kiếm cơ bản
	Tìm kiếm năng cao
