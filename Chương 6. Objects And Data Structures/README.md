## Chương 6: Objects And Data Structures

### 1. Data Abstraction (Trừu tượng giữ liệu)
- Sự trừu tượng dữ liệu là việc cho phép người dùng thao tác với bản chất của dữ liệu mà không cần phải biết việc triển khai nó.
### 2. Data/Object Anti-Symmetry (chống đối xứng dữ liệu/đối tượng)
- Mã thủ tục (mã sử dụng cấu trúc dữ liệu) giúp dễ dàng thêm các chức năng mới mà không cần thay đổi cấu trúc dữ liệu hiện có.  
Mặt khác, mã OO giúp dễ dàng thêm các lớp mới mà không cần thay đổi các chức năng hiện có.  
- Mã thủ tục gây khó khăn cho việc thêm cấu trúc dữ liệu mới vì tất cả các chức năng phải thay đổi.  
Mã OO gây khó khăn cho việc thêm các chức năng mới vì tất cả các lớp phải thay đổi.
### 3. The Law of Demeter (định luật Demeter)
- Một đối tượng cần phải ẩn đi cấu trúc bên trong của nó, nếu không cần chi tiết thì nên ẩn nó đi, tất cả xử lý liên quan tới cấu trúc bên trong dối tượng nên đc xử lý bên trong đối tượng.  
- định Luật Law nói rằng, một phương thức _f_ của lớp _C_ chỉ nên gợi phương thức:  
+ trong lớp _C_  
+ một đối đượng được tạo bởi _f_  
+ một đối tượng được truyền vào _f_ dưới dạng đối số.  
+ một đối tượng được giữ trong biến thể hiện của lớp _C_
#### 3.1. Train Wrecks (Xác tàu hỏa)
#### 3.2. Hybirds
- Không lên sử dụng cấu trúc nửa đối tượng, nửa cấu trúc dữ liệu
#### 3.3. Hiding structures

