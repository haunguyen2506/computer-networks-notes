# Định tuyến mạng máy tính qua ẩn dụ bảo vệ trường học

Bài viết này nhằm giúp sinh viên hiểu bản chất của định tuyến
trước khi đi vào các giao thức cụ thể.

## 1. Định tuyến thực chất là bài toán gì?

Trong mạng máy tính, định tuyến (routing) là quá trình quyết định gói tin nên được chuyển tiếp tới đâu tiếp theo để cuối cùng đến đúng đích.

Thay vì bắt đầu bằng bảng biểu hay thuật toán, ta hãy nhìn bài toán này thông qua một ẩn dụ đơn giản như sau.

## 2. Bài toán

Giả sử một trường học có n tòa nhà.
Mỗi tòa có một bảo vệ với các đặc điểm sau:

- Mỗi bảo vệ chỉ biết các tòa nhà kế bên mình

- Không ai có cái nhìn toàn bộ trường

- Khi có học sinh hỏi đường từ tòa A sang tòa B, bảo vệ phải quyết định chỉ học sinh đi hướng nào tiếp theo

Trong mạng máy tính:
- Tòa nhà <-> node
- Bảo vệ <-> router
- Chỉ đường <-> định tuyến

Điều quan trọng là:
    Bảo vệ không cần biết toàn bộ lộ trình, chỉ cần biết bước tiếp theo.

Đây chính là bản chất của định tuyến.

## 3. Định tuyến tĩnh
#### Khi mỗi bảo vệ được phát một bản đồ
Trong định tuyến tĩnh, ban quản lý phát cho mỗi bảo vệ một bản đồ toàn trường.
Trên bản đồ đã ghi sẵn:
- Muốn đi tới tòa nào thì rẽ hướng nào
- Mọi lộ trình đều được xác định trước
#### Ưu điểm
- Khi học sinh hỏi đường, bảo vệ chỉ cần nhìn bản đồ và trả lời ngay
- Không cần hỏi bảo vệ khác
- Quyết định nhanh, ổn định, dễ dự đoán

Nói ngắn gọn:
    Định tuyến tĩnh cho quyết định nhanh vì mọi thứ đã được xác định trước.