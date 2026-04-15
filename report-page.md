# Report 1 Page – FIT4012 Lab 1

## 1. Mục tiêu
Tóm tắt ngắn gọn mục tiêu của bài lab.
  Mục tiêu của bài lab là hiểu và cài đặt cách tính entropy để đo lượng thông tin của một chuỗi ký tự, từ đó tính được độ dư thừa thông tin (redundancy). Ngoài ra, bài lab giúp sinh viên hiểu và áp dụng thuật toán Euclid mở rộng để tìm nghịch đảo modulo trong số học.

## 2. Cách làm
- Đọc hiểu chương trình mẫu tính entropy.
- Cài đặt hàm tính redundancy dựa trên công thức R = log2(N) - H(X).
- Hoàn thiện hàm mod_inverse() bằng thuật toán Euclid mở rộng.
- Chạy thử chương trình với nhiều test case khác nhau để kiểm tra tính đúng đắn.

## 3. Kết quả chính
### 3.1 Entropy và redundancy
| Input        | Entropy | Redundancy | Nhận xét |
|-------------|--------:|-----------:|----------|
| aaaa        | 0       | 0          | Chuỗi chỉ có 1 ký tự nên không có độ bất định |
| abcd        | 2       | 0          | Các ký tự phân bố đều, entropy đạt tối đa |
| hello world | ~2.85   | ~0.61      | Chuỗi có phân bố không đều nên entropy trung bình |

### 3.2 Modulo inverse
| a | m  | Kết quả mong đợi | Kết quả chương trình |
|--:|---:|-----------------|----------------------|
| 3 | 7  | 5               | 5                    |
| 10| 17 | 12              | 12                   |
| 6 | 9  | Không tồn tại   | Không tồn tại        |

## 4. Kết luận
  Qua bài lab, em hiểu rõ hơn về cách tính entropy và ý nghĩa của nó trong việc đo lượng thông tin của dữ liệu. Em cũng học được cách tính độ dư thừa thông tin dựa trên entropy tối đa. Ngoài ra, em đã cài đặt thành công thuật toán Euclid mở rộng để tìm nghịch đảo modulo. Khó khăn lớn nhất là hiểu cách hoạt động của thuật toán và xử lý các trường hợp đặc biệt. Việc thực hành và test nhiều lần giúp em hiểu bài rõ hơn.