## Chương 9: Unit Tests

### 1. The Three Laws of TDD
- First Law: Bạn không được viết mã sản xuất cho tới khi bạn viết một bài kiểm tra không đạt  
- Luật thứ hai Bạn không được viết nhiều bài kiểm tra đơn vị hơn mức đủ để không đạt, và không biên dịch sẽ không thành công.  
- Luật thứ ba Bạn không được viết nhiều mã sản xuất hơn số lượng đủ để vượt qua bài kiểm tra hiện đang thất bại  
### 2. Blocks and Intending - Khối và ý định
- Các hàm không nên đủ lớn để chứa các cấu trúc lồng nhau.
- Mức thụt lề của một hàm không nên lớn hơn một hoặc hai.
- Tất nhiên, điều này làm cho các hàm dễ đọc và dễ hiểu hơn.
### 3. Do one thing - làm một việc
- __"FUNCTIONS SHOULD DO ONE THING. THEY SHOULD DO IT WELL. THEY SHOULD DO IT ONLY"__
- Viết hàm để phân rã một hàm lớn hơn thành một tập hợp các bước tại cấp độ trìu tượng tiếp theo.
- Các hàm làm một việc không thể phân chia thành các phần được
### 4. One Level of abstraction per function - một mức trừu tượng cho mỗi hàm
