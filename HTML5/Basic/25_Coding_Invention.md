# HTML5 Style Guide and Coding Conventions
### **1) Sử dụng đúng `DOCTYPE!`**
- Luôn khai báo `DOCTYPE!` ở dòng đầu tiên trong đoạn code .
    ```html
    <!DOCTYPE html>
    ```
### **2) Sử dụng chữ thường cho tên phần tử HTML**
- **HTML5** không phân biệt chữ hoa – chữ thường cho tên các phần tử. 
- Khuyến nghị sử dụng chữ thường cho tên các phần tử, vì:
    - Kết hợp cả chữ hoa và chữ thường sẽ không đẹp mắt, nhiều khi dẫn tới rối mắt trong lúc code .
    - Sử dụng chữ viết thường gần giống chuẩn XHTML hơn.
    - Viết thường nhìn đoạn code mạch lạc, rõ ràng hơn.
    - Viết chữ thường nhanh hơn.
- **VD :**
    - Không nên :
        ```html
        <SECTION>
          <p>This is a paragraph.</p>
        </SECTION>
        ```
    - Cực kỳ không nên :
        ```html
        <Section>
          <p>This is a paragraph.</p>
        </SECTION>
        ```
    - Nên :
        ```html
        <section>
          <p>This is a paragraph.</p>
        </section>
        ```
### **3) Luôn nhớ đóng thẻ cho tất cả các phần tử HTML**
- Trong **HTML5** , không nhất thiết sử dụng thẻ đóng cho tất cả các phần tử ( **VD :** thẻ `<p>` )
- Nhưng để code chuẩn, nên sử dụng thẻ đóng cho các phần tử .
- **VD :**
    - Không nên :
        ```html
        <section>
          <p>This is a paragraph.
          <p>This is a paragraph.
        </section>
        ```
    - Nên :
        ```html
        <section>
          <p>This is a paragraph.</p>
          <p>This is a paragraph.</p>
        </section>
        ```
### **4) Đóng thẻ rỗng cho các phần tử HTML**
- Trong HTML5, có thể tùy ý đóng các phần tử rỗng .
- **VD :**
    - Cách 1 :
        ```html
        <meta charset="utf-8">
        ```
    - Cách 2 :
        ```html
        <meta charset="utf-8" />
        ```
    > ***Chú ý :*** Cách này là bắt buộc trong **XHTML** và **XML**
### **5) Sử dụng chữ thường cho tên các thuộc tính**
- Giống tên thẻ, tên thuộc tính bạn cũng nên sử dụng chữ thường .
- **VD :**
    ```html
    <div class="menu">
    ```
### **6) Sử dụng nháy kép cho các giá trị thuộc tính**
- **HTML5** cho phép gán giá trị cho các thuộc tính mà không cần dấu ngoặc kép .
- Nhưng nên sử dụng dấu nháy kép cho các giá trị thuộc tính :
    - Cần sử dụng dấu nháy kép nếu giá trị chứa dấu cách .
    - Lúc dùng dấu nháy kép, lúc không dùng sẽ tạo một thói quen không tốt cho người lập trình, lập trình phải có tính đồng nhất nhất quán.
    - Để giá trị trong dấu ngoặc sẽ dễ đọc và phân biệt hơn.
- **VD :**
    - Sai :
        ```html
        <table class=table striped>
        ```
    - Đúng :
        ```html
        <table class="table striped">
        ```
### **7) Thuộc tính trong thẻ `<img>`**
- Luôn sử dụng thuộc tính `alt` với các ảnh chèn vào trang web . Đây là việc rất quan trọng khi hình ảnh chèn không hiển thị và cũng là cách để các công cụ tìm kiếm có thể dễ dàng tìm được nội dung ảnh định nói gì .
- Nên xác định kích thước các bức ảnh . Nó sẽ không làm trang web bị nhấp nháy vì trình duyệt có thể giữ chỗ không gian cho bức ảnh trước khi nó được nạp .
- **VD :**
    - Không nên :
        ```html
        <img src="html5.gif">
        ```
    - Nên :
        ```html
        <img src="html5.gif" alt="HTML5" style="width:128px;height:128px">
        ```
### **8) Khoảng trắng (`space`) và dấu "`=`"**
- **HTML5** cho phép khoảng trắng ở trước và sau dấu "`=`" . Tuy nhiên nếu không có thì sẽ dễ đọc và dễ nhóm các thực thể với nhau hơn .
- **VD :**
    - Không nên :
        ```html
        <link rel = "stylesheet" href = "styles.css">
        ```
    - Nên :
        ```html
        <link rel="stylesheet" href="styles.css">
        ```
### **9) Tránh để 1 dòng code quá dài**
- Khi sử dụng một trình soạn thảo **HTML**, nếu có một dòng code quá dài sẽ phải trượt thanh cuộn sang phải hoặc sang trái để có thể đọc hết dòng code đó . <br>
=> Cố gắng tránh những dòng code dài hơn `80` ký tự .
### **10) Thụt đầu dòng và cách dòng**
- Không thêm các dòng trống và thụt đầu dòng không cần thiết .
- Để dễ đọc hơn, thêm dòng trống vào các đoạn code dài hoặc các khối code logic .
- Để dễ đọc hơn, thụt đầu dòng cho mỗi tag con là `2-spaces` . Không sử dụng `tab` .
- **VD :**
    - Không nên :
        ```html
        <body>

          <h1>Famous Cities</h1>

          <h2>Tokyo</h2>

          <p>
            Tokyo is the capital of Japan, the center of the Greater Tokyo Area .
          </p>

        </body>
        ```
    - Nên :
        ```html
        <body>

        <h1>Famous Cities</h1>

        <h2>Tokyo</h2>
        <p>Tokyo is the capital of Japan, the center of the Greater Tokyo Area .</p>

        </body>
        ```
    - Table :
        ```html
        <table>
          <tr>
            <th>Name</th>
            <th>Description</th>
          </tr>
          <tr>
            <td>A</td>
            <td>Description of A</td>
          </tr>
          <tr>
            <td>B</td>
            <td>Description of B</td>
          </tr>
        </table>
        ```
    - List :
        ```html
        <ul>
          <li>London</li>
          <li>Paris</li>
          <li>Tokyo</li>
        </ul>
        ```
### **11) Có cần thẻ `<html>` và `<body>`?**
- Trong **HTML5**, thẻ `<html>` và thẻ `<body>` có thể bỏ qua .
- **VD :** Đoạn code sau vẫn được chấp nhận :
    ```html
    <!DOCTYPE html>
    <head>
      <title>Page Title</title>
    </head>

    <h1>This is a heading</h1>
    <p>This is a paragraph.</p>
    ```
- Tuy nhiên, **không khuyến khích việc bỏ đi thẻ `<html>` và thẻ `<body>`** .
- Thẻ `<html>` là thẻ `root` của file HTML . Nó được khuyến nghị sử dụng để khai báo ngôn ngữ của code :
    ```html
    <!DOCTYPE html>
    <html lang="en-US">
    ```
- Khai báo một ngôn ngữ rất quan trọng đối với các ứng dụng trợ năng (**screen readers**) và các công cụ tìm kiếm .
- Bỏ đi thẻ `<html>` và `<body>` có thể gây crash .
- Bỏ đi thẻ `<body>` có thể gây lỗi với các trình duyệt cũ (**IE9**)
### **12) Có cần thẻ `<head>`?**
- Trong **HTML5**, thẻ `<head>` có thể bỏ qua .
- Mặc định , trình duyệt sẽ add tất cả các phần tử trước thẻ `<body>` thành 1 phần tử `<head>` .
- Có thể giảm đi sự phức tạp của code bằng việc bỏ đi thẻ `<head>` :
    ```html
    <!DOCTYPE html>
    <html>
    <title>Page Title</title>

    <body>
      <h1>This is a heading</h1>
      <p>This is a paragraph.</p>
    </body>

    </html>
    ```
- Tuy nhiên, **không khuyến khích việc bỏ đi thẻ `<head>`** .
### **13) Meta Data**
- Phần tử `<title>` là bắt buộc trong **HTML5** . Nên làm cho title rõ nghĩa nhất có thể .
- **VD :**
    ```html
    <title>HTML5 Syntax and Coding Style</title>
    ```
- Các phần tử metadata quan trọng cần chú ý khai báo đầu tiên là `lang` và `charset` :
    ```html
    <!DOCTYPE html>
    <html lang="en-US">
    <head>
      <meta charset="UTF-8">
      <title>HTML5 Syntax and Coding Style</title>
    </head>
    ```
### **14) Viewport**
- **HTML5** giới thiệu một phương thức cho phép các web designer kiểm soát **viewport**, thông qua thẻ `<meta>` .
- **Viewport** là khu vực mà người dùng có thể nhìn thấy của trang web . Nó sẽ rất đa dạng trên các loại thiết bị , trên smartphone thì sẽ nhỏ hơn là trên máy tính .
- Nên bao gồm phần tử `<meta>` **viewport** trên tất cả các trang web :
    ```html
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    ```
- Phần tử `<meta>` **viewport** chỉ dẫn cho trình duyệt cách để kiểm soát kích thước và tỷ lệ của trang .
- Phần thông số `width=device-width` đặt độ rộng của trang phụ thuộc vào độ rộng màn hình của thiết bị .
- Phần thông số `initial-scale=1.0` đặt mức thu phóng ( **zoom** ) khi trang được load lần đầu bởi trình duyệt .
- **VD :** Trường hợp có và không có **viewport** :

    <img src=https://i.imgur.com/YmV6X3p.png>
 
### **15) Comment**
- Các comment ngắn nên được viết trên 1 dòng :
    ```html
    <!-- This is a comment -->
    ```
- Các comment dài nên được tách thành nhiều dòng :
    ```html
    <!--
      This is a long comment example. This is a long comment example.
      This is a long comment example. This is a long comment example.
    -->
    ```
### **16) File `.css`**
- Sử dụng công thức để link đến file `.css` riêng biệt .
    ```html
    <link rel="stylesheet" href="styles.css">
    ```
- Khai báo trong file `index.html` :
    - Nếu rule quá ngắn thì có thể gói gọn trong 1 dòng :
        ```css
        p.intro {font-family: Verdana; font-size: 16em;}
        ```
    - Nếu rule dài thì sẽ được viết thành nhiều dòng :
        ```css
        body {
          background-color: lightgrey;
          font-family: "Arial Black", Helvetica, sans-serif;
          font-size: 16em;
          color: black;
        }
        ```
### **17) JavaScript**
- Sử dụng công thức để link đến file `.js` :
    ```html
    <script src="myscript.js">
    ```
### **18) Đặt tên file bằng chữ thường**
- Một số web server ( **Apache**, **Unix** ) phân biệt chữ hoa và chữ thường ( "`london.jpg`" >< "`London.jpg`")
- Một số các web server khác ( **Microsoft**, **IIS** ) không phân biệt chữ hoa chữ thường ( "`london.jpg`" = "`London.jpg`")
- Nếu sử dụng kết hợp chữ hoa và chữ thường, cần có quy tắc cụ thể .
- Nếu chuyển từ một web server không phân biệt chữ hoa chữ thường sang 1 web server có phân biệt thì những lỗi nhỏ thôi cũng sẽ làm hỏng trang web .
- Để tránh các vấn đề này , nên sử dụng chữ thường cho tên file .
### **19) File Extension**
- File **CSS** có extension là `.css`
- File **JavaScript** có extension là `.js` 
- File **HTML** có extension là `.html` hoặc `.htm`
    - Không có sự khác biệt giữa định dạng `.htm` và `.html` . Cả 2 đều có thể sử dụng trên bất cứ trình duyệt và web server nào .
    - Sự khác biệt là do :
        - `.htm` là định dạng dành cho các hệ thống **DOS** xuất hiện từ sớm, giới hạn đuôi extension chỉ có 3 ký tự
        - `.html` là định dạng đến sau cho các hệ thông **Unix** không giới hạn ký tự đuôi extension




