# Report 1 Page – FIT4012 Lab 1

##1. Mục tiêu

Hiểu cách tính entropy của một chuỗi, từ đó suy ra redundancy, đồng thời nắm được cách tìm nghịch đảo modulo (modular inverse) bằng thuật toán phù hợp.

##2. Cách làm
Đọc và phân tích chương trình mẫu tính entropy.
Bổ sung hàm tính redundancy dựa trên entropy.
Hoàn thiện hàm mod_inverse() (dùng thuật toán Euclid mở rộng).
Chạy thử với nhiều test case để kiểm tra tính đúng đắn.
##3. Kết quả chính
3.1 Entropy và Redundancy
Input	Entropy	Redundancy	Nhận xét
aaaa	0	1	Chuỗi lặp hoàn toàn → không có thông tin mới
abcd	2	0	Các ký tự xuất hiện đều → thông tin tối đa
hello world	≈ 2.85	≈ 0.11	Phân bố ký tự không đều → entropy trung bình

Ghi chú:

Entropy tối đa với bảng chữ cái 4 ký tự là log
2
	​

(4)=2
Redundancy = 1 − (Entropy / Entropy tối đa)
3.2 Modulo Inverse
a	m	Kết quả mong đợi	Kết quả chương trình
3	7	5	5
10	17	12	12
6	9	Không tồn tại	Không tồn tại

Điều kiện tồn tại: gcd(a, m) = 1

##4. Kết luận

Qua bài lab, em hiểu rõ hơn về cách đo lượng thông tin bằng entropy và ý nghĩa của redundancy trong dữ liệu. Đồng thời, em nắm được cách tìm nghịch đảo modulo và điều kiện tồn tại của nó.

Khó khăn lớn nhất là hiểu công thức entropy và cài đặt thuật toán Euclid mở rộng. Việc thử nhiều test case và so sánh kết quả giúp em hiểu sâu hơn về bản chất của hai khái niệm này.
