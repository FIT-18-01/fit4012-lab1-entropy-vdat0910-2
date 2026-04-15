# Report 1 Page – FIT4012 Lab 1

## 1. Mục tiêu
- Hiểu cách tính entropy của một chuỗi ký tự.
- Bổ sung hàm tính độ dư thừa thông tin từ entropy.
- Cài đặt nghịch đảo modulo bằng thuật toán Euclid mở rộng.
- Kiểm thử chương trình với các test case thực tế.

## 2. Cách làm
- Đọc hiểu chương trình entropy mẫu.
- Bổ sung hàm tính redundancy.
- Hoàn thiện hàm mod_inverse().
- Chạy thử trên nhiều test case.

## 3. Kết quả chính
### 3.1 Entropy và redundancy
| Input | Entropy | Redundancy | Nhận xét |
|---|---:|---:|---|
| aaaa | 0.00 | 8.00 | Entropy thấp vì chỉ có 1 ký tự, redundancy cao |
| abcd | 2.00 | 6.00 | Entropy cao hơn vì 4 ký tự khác nhau |
| hello world | 2.85 | 5.15 | Entropy trung bình với sự phân bố ký tự |

### 3.2 Modulo inverse
| a | m | Kết quả mong đợi | Kết quả chương trình |
|---:|---:|---|---|
| 3 | 7 | 5 | 5 |
| 10 | 17 | 12 | 12 |
| 6 | 9 | Không tồn tại | Không tồn tại |

## 4. Kết luận
Qua bài lab, tôi hiểu rõ hơn cách tính entropy của một chuỗi ký tự và cách xác định độ dư thừa thông tin dựa trên giá trị entropy. Bên cạnh đó, việc cài đặt thuật toán Euclid mở rộng để tìm nghịch đảo modulo giúp tôi thấy được sự liên hệ giữa lý thuyết toán học và ứng dụng trong lập trình. Khó khăn ban đầu là cách áp dụng công thức vào chương trình, nhưng nhờ thử nghiệm với nhiều dữ liệu khác nhau, tôi đã nắm vững hơn về ý nghĩa của entropy và redundancy.