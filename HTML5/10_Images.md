# Images
- Hình ảnh có thể cải thiện về mặt thiết kế cũng như diện mạo của trang web

    <img src=https://i.imgur.com/S7R28sJ.png>
## **1) Hình ảnh trong HTML**
### **1.1) Cú pháp chèn ảnh**
- Để tạo hình ảnh trong HTML chúng ta sử dụng thẻ `<img>`.
- Cú pháp đơn giản nhất để tạo hình ảnh như sau:
    ```html
    <img src="image_url">
    ```
    - Thuộc tính `src` quy định đường dẫn của hình ảnh
- Thẻ `<img>` là một thẻ trống, chỉ chứa các thuộc tính, và không có tag đóng thẻ ..
### **1.2) Thuộc tính `src`**
- Giá trị của thuộc tính `src` có thể là một đường dẫn tương đối hoặc tuyệt đối .
- Nếu trang web hiện tại có cùng ***địa chỉ URL*** với hình ảnh thì khi tham chiếu tới ảnh cũng bắt đầu với cùng địa chỉ URL của code thì chúng có thể dùng **địa chỉ tương đối** như sau :
    - Cấu trúc thư mục code: 
    ```
    /var/www/html
    ├── img
    │   └── logo.png
    └── index.html
    ```
    ```html
    <img src="/img/logo.png" alt="Logo HTML">
    ```
- Ngoài ra, cũng có thể sử dụng ảnh từ website khác :
    ```html
    <img src="https://i.imgur.com/U704hHY.png">
    ```
### **1.3) Thuộc tính `alt`**
- Thuộc tính `alt` cung cấp đoạn text thay thế cho hình ảnh, trong trường hợp người dùng vì một lý do nào đó không thể load được hình ảnh ( do kết nối chậm , lỗi từ thuộc tính `src` ,....)
- **VD :**
    ```html
    <img src="/img/logo.png" alt="Logo HTML">
    ```
- Thuộc tính `alt` giúp các bộ máy tìm kiếm như `Google` , `Bing`... có thể biết xác định được ý nghĩa của hình ảnh khi chúng không thể hiểu được nội dung hình ảnh như con người . Ngoài ra với các thiết bị dành cho người khiếm thị cũng sử dụng giá trị của thuộc tính này để giúp người dùng biết được nội dung của hình ảnh .
### **1.4) Thuộc tính `title`**
- Thuộc tính `title` tương tự như `alt` dùng để cung cấp mô tả cho phần nội dung hình ảnh . 
- Nếu rê chuột lên ảnh trình duyệt sẽ hiển thị một hộp thoại tooltip nhỏ với nội dung là giá trị của thuộc tính này .
- **VD :**
    ```html
    <img src="/img/logo.png" title="Logo HTML">
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/EzSh0wP.png>

### **1.5) Kích cỡ ảnh (witdh và height)**