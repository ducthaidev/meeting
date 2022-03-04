
# Meeting

  

* Hoạt động với kong.

  

* Giải quyết bài toán authentication, authorization, token.

  

* Xử lý peek tại điểm 1.000.000 ccu(hiện tại đã đạt khoảng x00.000).

  

* Xử lý check out voucher.

  

* Đang bị deadlock.

  

* Thưởng voucher theo điều kiện(tuổi, thời gian sử dụng ứng dụng...), thời gian và địa điểm.

  

* Đáp ứng lượng tại lớn ngay lập tức(ví dụ sử dụng xong hoá đơn rồi tích điểm).

  

* Có service gọi vào để chấm điểm.

  

* Đang có dữ liệu trong mariabdb chứa thông tin tiêu thụ điện của người dùng (khoảng 2 triệu bản ghi). Cần phải đảm bảo toàn vẹn dữ liệu. Thiết kế endpoint phải đảm bảo trả về dữ liệu trong 0.5s(hiện tại đang 1.5s).

  

# MySQL
1. Isolation level
    - 4 MODE.
    - Mặc định REPEATABLE READ.
2. Locking Read
    - SELECT...FOR SHARE | FOR UPDATE