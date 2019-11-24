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
    <img src="/img/logo.pg" alt="Logo HTML">
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/0Bt6ruR.png>
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

### **1.5) Kích cỡ ảnh ( `witdh` và `height` )**
#### **1.5.1) Thuộc tính `width`**
- Thuộc tính `width` dùng để thiết lập chiều rộng của ảnh ( đơn vị `px` - pixel )
- Đơn vị `px` là mặc định và có thể bỏ qua nếu muốn .
- **VD :**
    ```html
    <img src="/img/logo.png" title="Logo HTML" width=500px>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/GHPAKvu.png>
    
- Ngoài đơn vị là **pixel** , có thể sử dụng đơn vị `%` để tạo chiều rộng của ảnh tương đối với độ rộng của phần tử bao ngoài hình ảnh :
    ```html
    <img src="/img/logo.png" title="Logo HTML" width=50%>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/F12TQK7.png>

    - Ảnh trên sẽ hiển thị trên trang với `50%` kích thước chiều rộng của phần tử chứa phần tử hình ảnh (hay phần tử `body`) .

- Giá trị mặc định của thuộc tính `width` là `auto` ứng với `100%` chiều rộng của ảnh :
    ```html
    <img src="/img/logo.png" title="Logo HTML" width=auto>
    ```
#### **1.5.2) Thuộc tính `height`**
- Thuộc tính `height` dùng để thiết lập chiều cao của ảnh ( đơn vị `px` - pixel )
- Đơn vị `px` là mặc định và có thể bỏ qua nếu muốn .
- **VD :**
    ```html
    <img src="/img/logo.png" title="Logo HTML" height=500px>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/5eQ9fjd.png>
    
- Ngoài đơn vị là **pixel** , có thể sử dụng đơn vị `%` để tạo chiều cao của ảnh tương đối với độ cao của phần tử bao ngoài hình ảnh :
    ```html
    <img src="/img/logo.png" title="Logo HTML" height=50%>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/CmtTjNM.png>

    - Ảnh trên sẽ hiển thị trên trang với `50%` kích thước chiều cao của phần tử chứa phần tử hình ảnh (hay phần tử `body`) .

- Giá trị mặc định của thuộc tính `height` là `auto` ứng với `100%` chiều cao của ảnh :
    ```html
    <img src="/img/logo.png" title="Logo HTML" height=auto>
    ```
#### **1.5.3) Sử dụng `style` thay cho `width` và `height`**
- Có thể sử dụng thuộc tính style để quy định chiều rộng và chiều cao của ảnh thay vì `width` và `height` :
- **VD :**  
    ```html
    <img src="/img/logo.png" style="width: 50%; height: 50%;">
    ```
### **1.6) Sử dụng kết hợp các thuộc tính**
- Có thể kết hợp nhiều thuộc tính lại với nhau :
- **VD :**
    ```html
    <img src="/img/logo.png" title="Học HTML" width="100" height="100">
    ```
### **1.7) Ảnh động**
- **HTML** cũng cho phép hiển thị ảnh động `GIFS` .
- **VD :**
    ```html
    <img src=https://i.imgur.com/ZK5DVuN.gif width="100" height="100">
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/ZK5DVuN.gif width="100" height="100">
### **1.8) Đặt link vào ảnh**
- Để sử dụng hình ảnh như một link, chỉ cần đặt thẻ `<img>` trong cặp thẻ `<a>`
    ```html
    <a href="default.asp">
      <img src="smiley.gif" alt="HTML tutorial">
    </a>
    ```
## **2) Map hình ảnh**
- Với chức năng map, có thể click vào từng khu vực riêng biệt trong ảnh .
## **3) Ảnh nền (background)**
## **4) Phần tử `<picture>`**