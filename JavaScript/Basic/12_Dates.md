# Dates
## **1) JavaScript Date Output**
- Mặc định , **JavaScript** sẽ sử dụng time zone của trình duyệt và hiển thị thông tin ngày tháng ở dạng chuỗi :
    ```js
    Tue Dec 17 2019 00:49:13 GMT+0700 (Indochina Time)
    ```
## **2) Các cách khởi tạo một Date object**
- Một **date object** có thể được tạo ra qua cấu trúc `new Date()`
- Có 4 cách tạo **date object**  :
### **2.1) `new Date()`**
- Cấu trúc `new Date()` tạo ra một **date object** với giá trị là thời gian hiện tại .
- **Date object** là một dạng tĩnh . Nó chỉ nhận giá trị đúng thời gian nó chạy, sau đó sẽ không thay đổi cho dù thời gian trên máy tính có trôi đi .
- **VD :**
    ```js
    var d = new Date();
    ```
    => Kết quả : `d = Tue Dec 17 2019 00:57:26 GMT+0700 (Indochina Time)`
### **2.2) `new Date(`*`year, month, ...`*`)`**