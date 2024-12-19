# Aes2
**Tiểu luận: Tìm hiểu về thuật toán AES (Advanced Encryption Standard)**  

Thuật toán AES (Advanced Encryption Standard) là một trong những chuẩn mã hóa phổ biến nhất hiện nay, được sử dụng rộng rãi trong các hệ thống bảo mật như giao dịch ngân hàng, bảo vệ dữ liệu cá nhân, và mạng viễn thông. AES nổi bật bởi tính bảo mật cao, tốc độ nhanh và khả năng ứng dụng linh hoạt.  

### **1. Lịch sử phát triển**  
AES được phát triển vào năm 1998 bởi hai nhà mật mã học người Bỉ, Vincent Rijmen và Joan Daemen, với tên gọi ban đầu là Rijndael. Năm 2001, Viện Tiêu chuẩn và Công nghệ Quốc gia Hoa Kỳ (NIST) đã chọn Rijndael làm chuẩn mã hóa chính thức thay thế cho DES (Data Encryption Standard), trở thành AES.  

### **2. Nguyên lý hoạt động**  
AES là thuật toán mã hóa khối đối xứng, tức là dùng chung một khóa để mã hóa và giải mã. Kích thước khối dữ liệu cố định là 128 bit, với các độ dài khóa phổ biến: 128, 192, và 256 bit.  

Quá trình mã hóa AES bao gồm:  
- **SubBytes:** Thay thế mỗi byte bằng một giá trị khác thông qua bảng S-box.  
- **ShiftRows:** Dịch chuyển các hàng trong khối dữ liệu.  
- **MixColumns:** Trộn dữ liệu giữa các cột (không áp dụng ở vòng cuối).  
- **AddRoundKey:** Kết hợp khối dữ liệu với khóa vòng (round key) thông qua phép XOR.  

Số vòng lặp phụ thuộc vào độ dài khóa: 10 vòng cho khóa 128-bit, 12 vòng cho khóa 192-bit và 14 vòng cho khóa 256-bit.  

### **3. Ưu điểm của AES**  
- **Bảo mật cao:** AES kháng được nhiều loại tấn công mật mã như brute force, linear cryptanalysis, và differential cryptanalysis.  
- **Hiệu suất tốt:** Thuật toán hoạt động hiệu quả trên cả phần cứng lẫn phần mềm, phù hợp với các thiết bị từ máy tính đến vi điều khiển.  
- **Linh hoạt:** Hỗ trợ nhiều độ dài khóa, đáp ứng các nhu cầu bảo mật khác nhau.  

### **4. Ứng dụng thực tế**  
AES hiện được sử dụng trong nhiều lĩnh vực như:  
- **Bảo mật giao dịch ngân hàng:** Bảo vệ thông tin khách hàng và giao dịch.  
- **Truyền thông mạng:** Sử dụng trong giao thức TLS/SSL để mã hóa dữ liệu trực tuyến.  
- **Thiết bị IoT:** Bảo vệ dữ liệu trong các hệ thống thông minh.  

### **Kết luận**  
Thuật toán AES không chỉ là chuẩn mực trong bảo mật thông tin hiện đại mà còn đặt nền tảng cho nhiều nghiên cứu và ứng dụng trong lĩnh vực mật mã học. Với khả năng chống lại các tấn công ngày càng tinh vi, AES vẫn sẽ tiếp tục đóng vai trò quan trọng trong việc bảo vệ dữ liệu toàn cầu trong tương lai.  
