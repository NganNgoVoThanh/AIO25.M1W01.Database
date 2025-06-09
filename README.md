# AIO25.M1W01 - Blog
# THIẾT KẾ DATABASE HIỆU QUẢ
## 1. Giới thiệu
Database (Cơ sở dữ liệu) là thành phần cốt lõi của mọi hệ thống phần mềm, là nơi phần mềm lưu trữ hầu hết dữ liệu của doanh nghiệp.
Một database thiết kế tốt ngay từ đầu sẽ giúp hệ thống:
- Toàn vẹn dữ liệu: Các ràng buộc (primary key, foreign key, UNIQUE, CHECK) ngăn dữ liệu “rác” vào hệ thống -> giảm lỗi trùng lặp, sai lệch.
- Hiệu năng: Khi mô hình chuẩn, chỉ truy vấn đúng dữ liệu cần -> truy vấn nhanh, mở rộng dễ.
- Bảo trì & phát triển: Thay đổi lược đồ (thêm cột, tách bảng) ít ảnh hưởng ứng dụng.
- Bảo mật & tuân thủ: Phân tầng schema/bảng để xác định rõ ai được truy cập bảng/ cột nào.
--> Thiết kế database schema chắc chắn thì hệ thống dữ liệu mới bền.
## 2. Tiêu chí cần & đủ khi thiết kế Database
### 2.1. Tính toàn vẹn dữ liệu - Đảm bảo dữ liệu đúng & nhất quán
- Sử dụng primary key, foreign key, ràng buộc CHECK, UNIQUE.
- Áp dụng chuẩn hoá dữ liệu đến mức 3NF để loại bỏ dư thừa.
### 2.2. Hiệu năng truy vấn - Truy vấn nhanh, tiết kiệm tài nguyên
- Phân tích khối lượng truy cập đọc/ghi để quyết định index phù hợp.
- Cân nhắc partitioning bảng lớn.
### 2.3. Khả năng khai thác & mở rộng - Dễ thêm bảng mới, ít “đập đi xây lại”
- Dễ dàng viết query, BI, ETL.
- Phân tách modular schema.
- Áp dụng naming convention nhất quán.
### 2.4. Bảo mật & phân quyền - Giới hạn ai được đọc/ghi, bảo vệ dữ liệu nhạy cảm
- Phân quyền dữ liệu thành roles (reader, writer, admin).
- Mã hoá dữ liệu nhạy cảm.
### 2.5. Khả năng khôi phục - Không mất dữ liệu khi lỗi, downtime thấp
## 3. Khai thác & sử dụng Database tối ưu
## 4. Nâng cấp – Khác biệt so với thiết kế cũ
## 5. Triển khai
![AIO2025 drawio](https://github.com/user-attachments/assets/fef3b366-52d9-4727-924f-74c2b5bc8f6c)

## 6. Kết luận

