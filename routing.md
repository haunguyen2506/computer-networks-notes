# Định tuyến mạng máy tính qua ẩn dụ bảo vệ trường học

Bài viết này nhằm giúp sinh viên hiểu bản chất của định tuyến
trước khi đi vào các giao thức cụ thể.

## 1. Định tuyến thực chất là bài toán gì?

Trong mạng máy tính, định tuyến (routing) là quá trình quyết định gói tin nên được chuyển tiếp tới đâu tiếp theo để cuối cùng đến đúng đích.

Thay vì bắt đầu bằng bảng biểu hay thuật toán, ta hãy nhìn bài toán này thông qua một ẩn dụ đơn giản.

## 2. Bài toán

Giả sử một trường học có n tòa nhà.
Mỗi tòa có một bảo vệ với các đặc điểm sau:

- Mỗi bảo vệ chỉ biết các tòa nhà kế bên mình

- Không ai có cái nhìn toàn bộ trường

- Khi có học sinh hỏi đường từ tòa A sang tòa B, bảo vệ phải quyết định chỉ học sinh đi hướng nào tiếp theo