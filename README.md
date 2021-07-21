# Task
+ Tìm hiểu về Golang & HTTP Request/Response 
**Keyword**
+ Client-Server, Web Development, Request / Response
## Golang 

1. syntax basic 
2. variables
3. function
4. for if else 
5. struct, slices , map
6. pointer 

## HTTP Request/Response 

+ Mô hình của ứng dụng web ( web application) là mô hình client-server

1. Client
Là phần cứng hoặc phần mềm đóng vai trò gửi request cho server và nhận response từ server trả về. Mỗi lần gửi yêu cầu qua một giao thức kết nối (HTTP/HTTPS) 
1 request bao gồm: 
+ URL
+ method(GET, POST, PUT, DELETE) 
+ Request header
+ Form Data(Request cơ bản: POST)
+ Query String parameters(Request cơ bản: GET)

2. Server là máy chủ , lưu trữ dữ liệu, cài đặt các webservice thực hiện các yêu cầu từ phía client và trả về response thông qua giao thức http request. 
1 respone : 
HTML

Mô hình client-server
+ Khi vào một trang web bất kỳ thông qua một tên miền. Browser đi tới DNS(Domain name system) tìm ra địa chỉ IP thực tế của tên miền đó. Sau đó IP được gửi về Browser. Trình duyệt sử dụng địa chỉ IP đó gửi request đến cái webserver của IP tìm được qua giao thức TCP/IP. 
+ Sau đó server trả về status code nếu status code là 200 thì server trả về dữ liệu HTML của trang web đó Browser sẽ tệp HTML hiển thị ra trang web đó cho người dùng

**status code cơ bản** 
404 Not Found.
500 Internal Server Error.
502 Bad Gateway.
503 Service Unavailable.
504 Gateway Timeout.

## Web development
+ Website vận hành : 
### Website tĩnh
+ Là website có source code được xây dựng sẵn bao gồm (html, css, js). Các website này không có sự tương tác với cơ sở dữ liệu phía server. 
### Website động
+ Các website này tương tác với cơ sở dữ liệu phía server.Chúng ta có thể thay đổi và quản lý các user ( Backend+ Frontend).Các website được xử lý run time. Được xây dựng bởi các ngôn ngữ kịch bản như PHP, C#, Java...

### Backend-Frontend
+ Frontend - Sử dụng html , css , js để thiết kế giao diện ( UX/UI ) , ngoài ra sử dụng các framework để tương tác với người dùng , làm các sự kiện của người dùng trở nên dễ dàng. 
+ Backend - là những công việc đằng sau của 1 trang web , tất cả những hoạt động không được nhìn thấy trên trình duyệt, thiết kế những cấu trúc cốt lõi của website như tính logic , thiết kế database , tối ưu các request từ phía client gửi về ...
+ Frontend thì sẽ thường sẽ nhận dữ liệu từ phía backend và render ra giao diện cho người dùng có thể nhìn thấy và tương tác.Và frontend tương tác với Backend qua các request. Và Backend sẽ nhận những request từ phía frondend để xử lý và gửi đi những dữ liệu cho frontend thông qua API.Backend và Frontend có mối quan hệ chặt chẽ với nhau. 
## Liên quan
1. API - RESTfull API- WEB API , JSON
API là  Web API  là một phương thức dùng để cho phép các ứng dụng khác nhau có thể giao tiếp, trao đổi dữ liệu qua lại. Dữ liệu được Web API trả lại thường ở dạng  JSON hoặc XML thông qua giao thức HTTP hoặc HTTPS.
RESTfulAPI là chuẩn dùng trong việc thiết kế API cho các webservices . để các ứng dụng web có thể giao tiếp với nhau. 
2. Kiến trúc microservice & Monolithic
- Monolithic
Chỉ phát triển, triển khai và quản lý của một khối duy nhất. Bao gồm cơ sở dữ liệu , giao diện phía client , ứng dụng phía server . tất cả các phần mềm được gộp là và các chức năng đc quản lý tại 1 nơi . 
- Microservice
Là chia thành từng phần riêng biệt rồi tổng hợp của nhiều services nhỏ và độc lập có thể chạy riêng biệt, phát triển và triển khai độc lập, từng nghiệp vụ khác nhau . Và mỗi 1 services sẽ giao tiếp với nhau qua API . vì vậy có thể làm độc lập và có thể dùng công nghệ riêng biệt không liên quan đến nhau. 
+ Khi một service trong mạng lưới Microservice gặp vấn đề thì hệ thống có thể vẫn hoạt động tiếp. Còn đối với Monolithic, khi một thành phần của hệ thống gặp vấn đề thì hệ thống sẽ dừng hoạt động.  
4. Mô hình MVC
Là mô hình model view controller
Trong đó mỗi đối tượng (model,view,controller) sẽ chịu trách nhiệm và quản lý từng nhiệm vụ riêng biệt. View là để tương tác với người dùng, Xử lý các dữ liệu của người dùng nhập vào hay yêu cầu là controller. Model có chức năng là tương tác với cơ sở dữ liệu. 
 
