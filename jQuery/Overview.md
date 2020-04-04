# Tổng quan về jQuery
## **1) Giới thiệu**
- **jQuery** là một thư viện **JavaScript** nhẹ, viết ít, làm nhiều .
- Mục đích của **jQuery** là giúp người lập trình sử dụng **JavaScript** dễ hơn trên trang web .
- **jQuery** có rất nhiều tác vụ phổ biến đòi hỏi nhiều dòng code **JavaScript** để thực hiện, sau đó kết hợp chúng thành các phương thức mà người lập trình có thể gọi bằng 1 dòng code .
- **jQuery** cũng giúp đơn giản hóa nhiều thứ phức tạp từ **JavaScript**, như **AJAX**, các thao tác **DOM**, ...
- Thư viện **jQuery** chứa các tính năng sau :
    - Các thao tác **HTML/DOM**
    - Các thao tác **CSS**
    - Các phương thức **HTML** event
    - Hiệu ứng và animation
    - **AJAX**
    - Các tiện ích khác .
- Có rất nhiều các thư viện **JavaScript**, nhưng **jQuery** được sử dụng phổ biến nhất .
## **2) Thêm jQuery vào trang web**
- Có 2 cách để sử dụng **jQuery** cho trang web :
    - Tải về thư viện **jQuery** từ trang chủ : jQuery.com
    - Include **jQuery** từ CDN
### **2.1) Download jQuery**
- Có 2 phiên bản **jQuery** có thể download :
    - ***Production*** - tốt nhất cho trang web vì đã được thu nhỏ và nén lại .
    - ***Development*** - dành cho testing và development , là phần code đọc được và chưa được nén .
> Cả 2 phiên bản đều có thể download từ `jQuery.com`

<img src=https://i.imgur.com/K2tQneN.png>

- Thư viện **jQuery** về cơ bản là 1 file **JavaScript**, vì vậy sẽ lồng nó vào trong thẻ `<script>` khi sử dụng ( đặt thẻ `<script>` trong section `<head>` ) :
    ```html
    <head>
      <script src="jquery-3.4.1.min.js"></script>
    </head>
    ```
### **2.2) Sử dụng CDN**
- Nếu không muốn download **jQuery** về host, có thể include nó từ một **CDN - Content Delivery Network** .
- Cả **Google** và **Microsoft** đề có CDN của **jQuery**
    - **Google CDN** :
        ```html
        <head>
          <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.4.1/jquery.min.js"></script>
        </head>
        ```
    - **Microsoft CDN** :
        ```html
        <head>
          <script src="https://ajax.aspnetcdn.com/ajax/jQuery/jquery-3.4.1.min.js"></script>
        </head>
        ```
