BÀI TOÁN :
 
Hệ thống phục vụ hoạt động quản lí đặt phòng của một khách sạn.
Trong đó, nhân viên quản lí (ROLE_ADMIN) có thể 
quản lí thông tin phòng, xem các báo cáo, quản lí các tài khoản người dùng hệ thống.
Nhân viên lễ tân (ROLE_USER) có thể đặt phòng,
thay đổi và hủy đặt phòng, làm thủ tục checkin, checkout và thanh toán cho khách hàng.
Khi thanh toán có thể xuất hóa đơn theo yêu cầu của khách hàng, bao gồm
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


REDMINE: 

1. Design database
2. Add task on redmine
3. Init project,  Create static page (header, footer, body layout)
4. Sign in, sign out
5. [Admin] Create user
6. [Admin] show list users and delete user  - (Security)
7. [Admin] create room (thêm thông tin phòng mới) - (Security)
8. [Admin] update room - (Security)
9. [Admin] show list rooms and delete room - (Security)
10. [Admin] create service (thêm mới một lại dịch vụ của khách sạn, vd : capuchino nhanh,...) - (Security)
11. [Admin] update service - (Security)
12. [Admin] show list services and delete service - (Security)
13. [Admin] view statistical - (Security)
14. [User] - show profile 
15. [User] - update profile
16. [User] - booking 
17. [User] - update info booking
18. [User] - show list bookings and destroy booking
19. [User] - create bill
20. [User] - show list bill details
21. Fix bug
22. Edit layout
23. Deploy on heroku
