# Manual Testing API with Postman

# I. Lý thuyết
## 1. Postman là gì

* Công cụ giao diện dùng để gọi các HTTP/GraphQL/gRPC requests
* Đóng vai trò là client, gọi đến server trong mô hình client-server
* Được sử dụng trong phát triển và kiểm thử phần mềm


## 2. cURL là gì

chữ viết tắt của “Client URL”, dùng để kiểm tra kết nối tới URL và curl command thường dùng để truyền tải dữ liệu.
* Là client trong mô hình client-server
* Là một CLI: Command Line Interface: giao diện dòng lệnh cho phép giao tiếp với server (kết nối, truyền dữ liệu), hỗ trợ các giao thức HTTP, FTP

## 3. Restful API request có các phương thức nào, mục đích của từng phương thức là gì

Triển khai các API RESTful bằng cách sử dụng Giao thức truyền siêu văn bản (HTTP). Phương thức HTTP cho máy chủ biết máy chủ cần làm gì với tài nguyên. Sau đây là 4 phương thức HTTP phổ biến:

### GET 
Lấy ra dữ liệu theo điều kiện chỉ định. VD: Lấy ra danh sách
### POST 
Tạo mới dữ liệu
### PUT 
Cập nhập các dữ liệu 
### DELETE 
Xóa các tài nguyên 
### PATCH 
Cũng gần giống put dùng để cập nhật một phần giá trị thay vì cập nhật đầy đủ các thông số 

## 4. Postman collection dùng để làm gì

Hiểu nôm na, nó chính là Folder, giúp đóng gói những request vào chung 1 chỗ
* Tập hợp các API có liên quan đến nhau
* Có thể dùng chung phương thức xác thực, URL tài nguyên

## 5. Postman request hỗ trợ phương thức xác thực phổ biến nào

### Basic Auth

HTTP Basic Authentication là kiểu xác thực cơ bản nhất của một WebServer yêu cầu client nhập username và password mỗi khi request. Client gửi tên người dùng và mật khẩu kiểu nối username và password theo dạng username:password trong tiêu đề khi yêu cầu. Client mã hóa những thông tin này bằng base64. Và có từ khoá Basic phía trước đó.

### Bearer Token

Thường được gọi là Token authentication. Đây là một hình thức xác thực HTTP liên quan đến token có tên là Bearer token. Như tên mô tả Bearer Token cấp quyền truy cập cho người dùng khi có token hợp lệ. Kiểu này thường dùng.
Bằng cách chúng ta sign in để nhận về một body chứa token, xong lấy token này gắn vào từng request để dùng sau đó.

## 6. Sử dụng Postman variable dùng để làm gì

* Tái sử dụng các giá trị
* Lưu trữ và bảo vệ các dữ liệu nhạy cảm (username, mật khẩu)

## 7. Sử dụng Postman environment dùng để làm gì

* Sử dụng Postman variable
* Quản lý các biến trên nhiều môi trường của phần mềm
* Tiết kiệm thời gian, công sức test khi thay đổi môi trường

