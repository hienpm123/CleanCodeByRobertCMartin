# CleanCodeByRobertCMartin

# Chương 1: Clean Code
# Chương 2: MeaningFull Name - Tên có ý nghĩa
Tên có ở khắp mọi nơi trong phần mềm, chúng ta đặt tên cho các biến, các hàm, lớp và gói. Chúng ta đặt tên cho tệp nguồn và thư mục của chúng ... Vì chúng ta sử dụng tên ở rất nhiều việc, nên chúng ta cần đặt tên tốt hơn. Sau đây là một số quy tắc đơn giản để tạo tên hay.
# 1. Sử dụng tên có chủ đích
Tại sao phải đặt tên có chủ đích?
- Mọi người đọc mã của bạn (bao gồm cả bạn) sẽ cảm thấy hạnh phúc hơn.
- Đọc code dễ dàng hơn và dễ thay đổi
- tạo ra sự rõ ràng của mã(không phải sự đơn giản của mã)

ví dụ: Thay vì sử dụng _int d; // elapsed time in days

thì ta có thể sử dụng

_int elapsedTimeInDays;

_int daysSinceCreation;

_int daysSinceModification;

_int fileAgeInDays;

# 2. Tránh thông tin sai lệch
