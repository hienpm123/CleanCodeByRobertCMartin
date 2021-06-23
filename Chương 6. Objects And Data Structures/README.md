## Chương 6: Objects And Data Structures

### 1. Data Abstraction (Trừu tượng giữ liệu)
- Sự trừu tượng dữ liệu là việc cho phép người dùng thao tác với bản chất của dữ liệu mà không cần phải biết việc triển khai nó.
### 2. Data/Object Anti-Symmetry (chống đối xứng dữ liệu/đối tượng)
- Mã thủ tục (mã sử dụng cấu trúc dữ liệu) giúp dễ dàng thêm các chức năng mới mà không cần thay đổi cấu trúc dữ liệu hiện có.  
Mặt khác, mã OO giúp dễ dàng thêm các lớp mới mà không cần thay đổi các chức năng hiện có.  
- Mã thủ tục gây khó khăn cho việc thêm cấu trúc dữ liệu mới vì tất cả các chức năng phải thay đổi.  
Mã OO gây khó khăn cho việc thêm các chức năng mới vì tất cả các lớp phải thay đổi.
### 3. Do one thing - làm một việc
- __"FUNCTIONS SHOULD DO ONE THING. THEY SHOULD DO IT WELL. THEY SHOULD DO IT ONLY"__
- Viết hàm để phân rã một hàm lớn hơn thành một tập hợp các bước tại cấp độ trìu tượng tiếp theo.
- Các hàm làm một việc không thể phân chia thành các phần được
### 4. One Level of abstraction per function - một mức trừu tượng cho mỗi hàm
