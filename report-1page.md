# Report 1 Page – FIT4012 Lab 2

## 1. Mục tiêu
Mục tiêu của bài lab là hoàn thiện và kiểm thử hai thuật toán mã hóa cổ điển là Caesar Cipher và Rail Fence Cipher, bao gồm cả mã hóa, giải mã, xử lý dấu cách, kiểm tra đầu vào và đọc dữ liệu từ file.

## 2. Cách làm
- Hoàn thiện Caesar Cipher cho chữ thường, giữ nguyên dấu cách và bổ sung chức năng giải mã.
- Hoàn thiện Rail Fence Cipher cho giải mã, giữ nguyên dấu cách, kiểm tra đầu vào hợp lệ và đọc dữ liệu từ file.
- Chạy chương trình với nhiều test case khác nhau để kiểm tra tính đúng đắn.

## 3. Kết quả chính
### 3.1 Caesar Cipher
| Input | Key | Ciphertext / Plaintext | Nhận xét |
|---|---:|---|---|
| I LOVE YOU | 3 | L ORYH BRX | Mã hóa đúng, giữ nguyên dấu cách |
| hello world | 5 | mjqqt btwqi | Hỗ trợ chữ thường tốt |
| LORYH BRX | 3 | ILOVE YOU | Giải mã đúng với khóa 3 |

### 3.2 Rail Fence Cipher
| Input | Rails | Ciphertext / Plaintext | Nhận xét |
|---|---:|---|---|
| I LOVE YOU | 2 | ILV O OEYU | Mã hóa đúng theo dạng zigzag 2 hàng |
| I LOVE YOU | 4 | I EYLVOOU | Mã hóa đúng, vẫn giữ dấu cách |
| IOEOLVYU | 2 | ILOVEYOU | Giải mã đúng với 2 rails |

### 3.3 Input validation / file input
- Trường hợp đầu vào không hợp lệ:chương trình kiểm tra các lỗi như khóa âm, số rails nhỏ hơn 2, chuỗi rỗng hoặc dữ liệu không đúng định dạng trước khi xử lý.
- Kết quả đọc từ `data/input.txt`:chương trình đọc dữ liệu thành công từ file và thực hiện mã hóa/giải mã đúng theo nội dung đầu vào.

## 4. Kết luận
Qua bài lab, em hiểu rõ hơn cách hoạt động của Caesar Cipher và Rail Fence Cipher, đặc biệt là sự khác nhau giữa cách dịch ký tự và cách sắp xếp theo zigzag. Khó khăn lớn nhất là cài đặt phần giải mã Rail Fence Cipher và xử lý dấu cách đúng cách. Việc chạy nhiều test case giúp em kiểm tra logic chương trình và hiểu rõ hơn nguyên lý của từng thuật toán.
