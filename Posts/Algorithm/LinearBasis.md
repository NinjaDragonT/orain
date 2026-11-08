<a href="../BaiViet.html" class="back-btn">← Quay lại </a>

# Ứng dụng của Linear Basis
Sử dụng trong các bài toán về tập hợp con và các tính chất của phép XOR.

Thuật toán sẽ nén một mảng khổng lồ có $N$ phần tử (Có thể tạo ra $2^N$ tập con) thành tối đa $\log(N)$ phần tử mà vẫn bảo toàn tính chất tạo giá trị.

# Thuật toán hoạt động ra sao?
Gọi một mảng `basis[60]` trong đó `basis[i]` lưu trữ một số có bit cao nhất là bit thứ $i$

Khi muốn thêm một số `x` vào mảng:  
1. Duyệt bit $i$ từ 60 về 0.  
2. Nếu bit $i$ của `x` bằng 1:  
 * Nếu `basis[i]` bằng 0: Gán `basis[i] = x` và kết thúc.  
 * Nếu `basis[i]` khác 0: Ta triệt tiêu bit thứ $i$ của `x` bằng cách gán `x = x ^ basis[i]`.  
3. Khi `x` giảm về 0: Cho biết `x` không còn đóng góp một giá trị mới nào, bản thân `x` đã có thể được tạo ra bằng cách `xor` các phần tử trong `basis`.
