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
__Cách giải quyết:__  
![image](https://user-images.githubusercontent.com/45452245/120101553-bc9f8180-c170-11eb-8dba-63f136c64a7d.png)  
với việc thay đổi tên đơn giản này, sẽ rất dễ dàng để hiểu đoạn code này đang làm gì __đây là sức mạnh của việ sử dụng tên hay__
- __Tránh sử dụng tên bao gồm từ _list_ khi đề cập đến một tập hợp__ ngoại trừ trường hợp đang đề cập đến một danh sách. Danh sách có nghĩa là một cái gì đó cụ thể với lập trình viên. Ví dụ listAccount, Tài khoản thực sự không phải là một danh sách, nó là một tập hợp. Vì vậy sử dụng accountGroup, clusterOfAccount hoặc accounts sẽ tốt hơn.
- __Tránh sử dụng những tên khác nhau chỉ một chút nhỏ.__ Ví dụ __XYZControllerForEfficientHandlingOfStrings__ - __XYZControllerForEfficientStorageOfStrings__ => chúng có hình dạng giống nhau một cách kinh ngạc. 
### 3. Tạo nên sự khác biệt có ý nghĩa
- Nếu các tên khác nhau thì chúng phải có ý nghĩa khác nhau.
- Sự khác biệt của _account_ và _accountInfo_, _accountData_ là gì?. Việc sử dụng Info và Data là không cần thiết, cũng giống như _a_, _an_, _the_.
- Tránh sử dụng những tên dư thừa, ví dụ: name thay vì nameString
- từ _variable_ không nên xuất hiện trong đặt tên biến, từ _table_ không xuất hiện trong cách đặt tên table
### 4. Sử dụng tên có thể phát âm
![image](https://user-images.githubusercontent.com/45452245/120110644-8249da80-c198-11eb-92e8-cdab311652db.png)  
sử dụng genymdhms và modymdhms thì ta sẽ phát âm như thế nào?  
### 5. Sử dụng tên có thể tìm kiếm
- Nếu đặt tên với một ký tự đơn hoặc một số, như vậy khi tìm kiếm sẽ gặp rất nhiều khó khăn, nhưng từ như vậy sẽ xuất hiện rất nhiều trong project.
- vì vậy khi đặt tên, __tên phải phù hợp với kích thước và phạm vi của nó.__
### 6. Tránh mã hóa
- Việc mã hóa khi đặt tên sẽ trở thành một gánh nặng khi giải quyết một vấn đề. Chúng rất khó phát âm và dễ viết sai
#### 6.1. Ký hiệu Hungary
- Đặt tên theo ký hiệu Hungary là đặt tên biến kèm với kiểu dữ liệu, ví dụ phoneString. Với cách đặt tên Hungary và mã hóa khi cần thay đổi tên, kiểu dữ liệu, hàm, class sẽ rất khó khăn, đánh lừa người đọc.  
- ví dụ: phoneString, phoneNumber
#### 6.2 Tiền tố số
- Khi đọc code chúng ta sẽ không để ý tới tiền tố hay hậu tố của tên, vì vậy hãy đặt tên ngắn nhất có thể và mang ý nghĩa.
#### 6.3 Interface và Implements
- Để mã hóa 1 interface ta nên sử dụng Imp, ví dụ ShapeFactoryImp thay vì sử dụng IShapFactory, vì _Imp_ đề cập tới việc triền khai, còn _I_ nói tới việc mã hõa.
### 7. Tránh lập bản đồ tinh thần
- Hãy đặt tên để người khác đọc có thể hiểu, tránh việc sử dụng một suy nghĩ riêng để đặt tên.
### 8. Tên lớp
- Tên của lớp nên là danh từ hoặc là cụm danh từ, ví dụ Customer, WikiPage, Account,... Tránh những từ như Manager, Processor, Data và Info khi đặt tên lớp. Không nên đặt tên lớp là một động từ.
### 9. tên phương thức
- Tên của phương thức nên là động từ hoặc một cụm động từ, ví dụ PostPayment, DeletePage hoặc Save.
- Đặt tên theo tiêu chuẩn javabean với tiền tố _get_, _set_ và _is_.
### 10. Đừng dễ thương
- Ví dụ với mục đích xóa, chúng ta đặt tên HolyHandGrenade và DeleteIitem, cái tên HolyHandGrenade sẽ chẳng biết có mục đích gì, mặc dù nó cũng thực hiện cùng một chức năng với DeleteItem.
__Say what you mean. Mean what you say__
### 11. Chọn một từ cho mỗi khái niệm
- Hãy sử dụng một từ vựng nhất quán trong code của bạn. Sử dụng quá nhiều từ vựng cho một hoàn cảnh sẽ dễ gây nhầm lẫn và khó đọc hiểu.
### 12. Đừng chơi chữ
- Tránh sử dụng một từ giống nhau cho hai mục đích khác nhau, sử dụng cùng một thuật ngữ cho hai ý tưởng khác nhau là một cách chơi chữ.
- Để đảm bảo tính nhất quan, sử dụng tên có ngữ nghĩa khác nhau.
### 13. Sử dụng giải pháp tên miền
- Chọn tên kỹ thuật.
### 14. Sử dụng tên miền có vấn đề
- ?????
### 15. Thêm ngữ cảnh có ý nghĩa
### 16. Không thêm ngữ cảnh vô cớ

