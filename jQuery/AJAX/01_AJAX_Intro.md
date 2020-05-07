# Giới thiệu về AJAX
- **AJAX** là viết tắt của **Asynchronous JavaScript And XML** .
- **AJAX** không phải một ngôn ngữ lập trình .
- **AJAX** chỉ sử dụng sự kết hợp của :
    - Trình duyệt tích hợp sẵn object `XMLHttpRequest` : để request dữ liệu từ Server )
    - **JavaScript** và **HTML DOM** : để hiển thị hoặc sử dụng dữ liệu .
- **AJAX** có thể sử dụng **XML** để vận chuyển dữ liệu, nhưng các hình thức phổ biến cũng không kém là vận chuyển dưới dạng thuần túy hoặc dưới dạng **JSON** .
- **AJAX** cho phép các trang web được cập nhật không đồng bộ bằng cách trao đổi dữ liệu với một Web Server khác phía sau . Điều này có nghĩa là có thể cập nhật các phần của trang web mà không cần load lại toàn bộ trang .
- Cách hoạt động của **AJAX** :
    - **B1 :** Một event xảy ra trong trang web ( trang được load, một button được click,...)
    - **B2 :** Một đối tượng `XMLHttpRequest` được tạo bởi **JavaScript**
    - **B3 :** Đối tượng `XMLHttpRequest` gửi request đến web server .
    - **B4 :** Server xử lý request 
    - **B5 :** Server gửi response về cho trang web
    - **B6 :** Response được đọc bởi **JavaScript**
    - **B7 :** Hành động cập nhật lại trang sẽ được **JavaScript** thực hiện

<p align=center><img src=https://i.imgur.com/XKt1EVM.png width=50%></p>

### **Liên kết giữa jQuery và AJAX**
- **jQuery** cung cấp một vài phương thức cho các tính năng **AJAX** .
- Với các phương thức **jQuery AJAX**,  bạn có thể request text, HTML, XML hoặc JSON từ một remote server sử dụng cả 2 phương thức `HTTP get` và `HTTP post` => Có thể load dữ liệu bên ngoài và đổ trực tiếp vào trang web .