# Layout
## **1) Các phần tử layout của HTML**
- Website thường hiển thị nội dung theo nhiều cột ( giống một tờ tạp chí hay 1 tờ báo ) .
- HTML cung cấp một số phần tử ngữ nghĩa xác định các phần khác nhau của trang web :

<p align=center><img src=https://i.imgur.com/uusvPvs.gif></p>

- Trong đó :
    - `<header>` - Định nghĩa phần header cho trang
    - `<nav>` - Định nghĩa container chứa các link điều hướng
    - `<section>` - Định nghĩa các section trong trang 
    - `<article>` - Định nghĩa các bài viết độc lập
    - `<aside>` - Định nghĩa phần nội dung hiển thị phía bên cạnh phần nội dung chính ( như 1 sidebar )
    - `<footer>` - Định nghĩa footer cho trang
    - `<details>` - Định nghĩa các thông tin thêm
    - `<summary>` - Định nghĩa tiêu đề cho phần tử `<details>`
## **2) Các kỹ thuật layout**
- Có 5 cách khác nhau để tạo ra một bố cục web . Mỗi cách lại có các ưu nhược điểm khác nhau .
### **2.1) HTML Tables (not recommended)**
- Phần tử `<table>` không được thiết kế để trở thành một công cụ layout . Mục đích của phần tử `<table>` là để hiển thị các dữ liệu dạng bảng . Vì vậy, không sử dụng `<table>` để bố trí trang! Chúng sẽ mang một mớ hỗn độn vào code. Và rất khó để sau này có thể thiết kết lại trang web
- **VD :**

    <img src=https://i.imgur.com/65ABMhp.png>

### **2.2) CSS Frameworks**
- Nếu muốn tạo layout một cách nhanh nhất , có thể sử dụng các framework, giống như **W3.CSS** hoặc **Bootstrap** .
### **2.3) CSS Floats**
- Khá phổ biến khi hiển thị bố cục web sử dụng **CSS float** .
- **Float** rất dễ học , chỉ cần nhớ cách hoạt động của thuộc tính **float and clear** . 
- Nhược điểm : các phần tử `float` được gắn liền với luồng code, không đảm bảo được tính linh hoạt .
### **2.4) CSS Flexbox**
- **Flexbox** là chế độ layout mới trong **CSS3** .
- Việc sử dụng **flexbox** đảm bảo rằng các phần tử hoạt động có thể dự đoán được khi layout của trang phải phù hợp với cá kích thước màn hình khác nhau và các thiết bị hiển thị khác nhau. 
- Nhược điểm : không hoạt động trên **IE10** trở về trước .
### **2.5) CSS Grid View**
- Module **CSS Grid** cung cấp hệ thống layout dựa trên lưới với các hàng và cột , giúp thiết kế trang web dễ dàng hơn .
- Nhược điểm : không hoạt động trên **IE** hoặc **Microsoft Edge** `15` trở về trước .
