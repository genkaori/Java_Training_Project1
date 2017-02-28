Hệ thống phục vụ hoạt động quản lí đặt phòng của một khách sạn.
 
Trong đó:
- Nhân viên quản lí (ROLE_ADMIN) có thể :
 Quản lí thông tin phòng, xem các báo cáo, quản lí các tài khoản người dùng hệ thống.
- Nhân viên lễ tân (ROLE_USER) có thể :
Đặt phòng, thay đổi và hủy đặt phòng, làm thủ tục checkin, checkout và thanh toán cho khách hàng.
- Khi thanh toán có thể xuất hóa đơn theo yêu cầu của khách hàng, bao gồm
tiền phòng và chi phí các dịch vụ của khách sạn mà khách hàng đã dùng.

* QUAN HỆ GIỮA CÁC THỰC THỂ:
- Một Hotel có nhiều Room, một Room phải thuộc vào một Hotel nhất định
- Một Room có thể đặt bởi nhiều Client, một Client lại có thể đặt nhiều Room tại nhiều thời điểm khác nhau
→ Đề xuất thêm một lớp Booking
- Một Booking có thể dùng nhiều Service khác nhau,
một Service lại có thể được sử dụng bởi nhiều Booking khác nhau → Đề xuất thêm lớp UsedService
- Một Booking có thể được thanh toán nhiều lần khác nhau nên có thể có nhiều Bill
- Mỗi Bill có tối đa một User lập và nhận thanh toán.
- Một User có thể lập nhiều Bill.
