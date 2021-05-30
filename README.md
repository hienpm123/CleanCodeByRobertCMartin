# CleanCodeByRobertCMartin

## Chương 1: Clean Code
## Chương 2: MeaningFull Name - Tên có ý nghĩa
Tên có ở khắp mọi nơi trong phần mềm, chúng ta đặt tên cho các biến, các hàm, lớp và gói. Chúng ta đặt tên cho tệp nguồn và thư mục của chúng ... Vì chúng ta sử dụng tên ở rất nhiều việc, nên chúng ta cần đặt tên tốt hơn. Sau đây là một số quy tắc đơn giản để tạo tên hay.
### 1. Sử dụng tên có chủ đích
Tại sao phải đặt tên có chủ đích?
- Mọi người đọc mã của bạn (bao gồm cả bạn) sẽ cảm thấy hạnh phúc hơn.
- Đọc code dễ dàng hơn và dễ thay đổi
- tạo ra sự rõ ràng của mã(không phải sự đơn giản của mã)<space><space>  
ví dụ: Thay vì sử dụng _int d; // elapsed time in days_ thì ta có thể sử dụng<space><space>  
_int elapsedTimeInDays;<space><space>  
int daysSinceCreation;<space><space>  
int daysSinceModification;<space><space>  
int fileAgeInDays;_<space><space>  

### 2. Tránh thông tin sai lệch
ví dụ:  
![image](https://user-images.githubusercontent.com/45452245/120101127-b7d9ce00-c16e-11eb-98de-e8bc1a07d46c.png)  
 chúng ta thấy rằng List<int> getFlagCells và gắn cờ cho cell thông qua STATUS_VALUE sẽ làm code khó hiểu.  
Cách giải quyết:
![image](https://user-images.githubusercontent.com/45452245/120101553-bc9f8180-c170-11eb-8dba-63f136c64a7d.png)  
với việc thay đổi tên đơn giản này, sẽ rất dễ dàng để hiểu đoạn code này đang làm gì __đây là sức mạnh của việ sử dụng tên hay__
