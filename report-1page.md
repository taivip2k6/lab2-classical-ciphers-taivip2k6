# Report 1 Page – FIT4012 Lab 2

## 1. Mục tiêu
Mục tiêu của bài lab là cài đặt và hiểu cách hoạt động của hai thuật toán mã hóa cổ điển: Caesar Cipher và Rail Fence Cipher. Sinh viên cần thực hiện mã hóa, giải mã, xử lý đầu vào hợp lệ và kiểm tra chương trình với nhiều test case khác nhau.

## 2. Cách làm
Hoàn thiện Caesar Cipher:
Dịch chuyển ký tự chữ cái (cả chữ hoa và chữ thường).
Giữ nguyên dấu cách.
Thực hiện giải mã bằng cách đảo dấu shift.
Hoàn thiện Rail Fence Cipher:
Cài đặt giải mã.
Giữ nguyên dấu cách.
Kiểm tra đầu vào hợp lệ.
Đọc dữ liệu từ file.
Thực hiện chạy thử với nhiều test case để kiểm tra tính đúng đắn.

## 3. Kết quả chính
### 3.1 Caesar Cipher
| Input | Key | Ciphertext / Plaintext | Nhận xét |
|---|---:|---|---|
| I LOVE YOU | 3 |L ORYH BRX  | Mã hóa đúng, giữ khoảng trắng |
| hello world | 5 | mjqqt btwqi | Xử lý đúng chữ thường |
| LORYH BRX | 3 |I LOVE YOU  | Giải mã chính xác |

### 3.2 Rail Fence Cipher
| Input | Rails | Ciphertext / Plaintext | Nhận xét |
|---|---:|---|---|
| I LOVE YOU | 2 | I O E Y U L V O |Mã hóa đúng dạng zigzag  |
| I LOVE YOU | 4 | I Y O V E U L O |  Rails nhiều hơn → phân bố khác|
| IOEOLVYU | 2 | I LOVE YOU | Giải mã đúng |

### 3.3 Input validation / file input
Trường hợp đầu vào không hợp lệ:
Chứa số hoặc ký tự đặc biệt → chương trình báo lỗi.
Key âm hoặc không hợp lệ được xử lý bằng chuẩn hóa (mod 26).
Kết quả đọc từ data/input.txt:
Chương trình đọc đúng nội dung file.
Thực hiện mã hóa/giải mã chính xác theo từng dòng.

## 4. Kết luận
Qua bài lab, em hiểu rõ hơn cách hoạt động của các thuật toán mã hóa cổ điển, đặc biệt là cách xử lý ký tự và logic dịch chuyển trong Caesar Cipher cũng như cách sắp xếp zigzag trong Rail Fence Cipher. Khó khăn lớn nhất là phần giải mã Rail Fence vì cần xác định đúng vị trí ký tự. Bài lab giúp em nắm vững hơn về xử lý chuỗi và tư duy thuật toán.
