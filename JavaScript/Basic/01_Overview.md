# Tổng quan về JavaScript
## **1) Giới thiệu**
- **JavaScript** ( viết tắt là **JS** ) là một ngôn ngữ lập trình kịch bản, mã lệnh được thực thi bởi trình duyệt của người dùng.
- **JavaScript** được sử dụng rộng rãi trong việc kết hợp với **HTML/CSS** để thiết kế web động .
- **JavaScript** có thể :
    - Thay đổi content HTML
    - Thay đổi thuộc tính HTML
    - Thay đổi style HTML (CSS)
    - Ẩn phần tử HTML
    - Hiện phần tử HTML
## **2) Cách sử dụng JavaScript**
### **2.1) Sử dụng code script**
- Trong **HTML**, có thể đặt code **JavaScript** trong cặp thẻ `<script>` .
- Một **JavaScript function** là một khối code **JavaScript** , có thể được thực thi khi được gọi . **VD :** khi user click vào button, một **event** xảy ra , một **function** sẽ được gọi .
- **Script** có thể được đặt ở trong thẻ `<body>`, ở `<head>` của trang HTML hoặc ở cả hai .
- **VD :**
    ```html
    <script>
    function myFunction() {
      document.getElementById("demo").innerHTML = "Paragraph changed.";
    }
    </script>
    ```
### **2.2) Sử dụng file `.js` - internal**
- Có thể gọi 1 file script ngoài và lồng vào trong trang HTML để xử lý .
- File **JavaScript** có định dạng `.js`
- Để sử dụng 1 file javascript , khai báo đường dẫn file qua thuộc tính `src` của thẻ `<script>` .
- **VD :** Có cấu trúc thư mục sau :
    ```
    /var/www/html
    ├── img
    │   └── logo.png
    ├── index.html
    ├── myscript.js
    └── styles.css
    ```
    - Để gọi file `myscript.js` trong trang `index.html` :
        ```html
        <script src="myscript.js"></script>
        ```
### **2.3) Sử dụng file `.js` - external**
- File **JavaScript** cũng có thể được gọi từ một đường dẫn tuyệt đối trên Internet .
- **VD :**
    ```html
    <script src="https://www.w3schools.com/js/myScript1.js"></script>
    ```