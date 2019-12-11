# Câu lệnh JavaScript & Chương trình JavaScript
## **1) Câu lệnh JavaScript**
- Câu lệnh **JavaScript** có thể tạm hiểu là một công việc sẽ được thực thi bởi trình duyệt .
- Mỗi câu lệnh cần phải được kết thúc bởi dấu chấm phẩy (`;`)
- **VD :**
    ```js
    var x, y, z;  // Statement 1
    x = 5;    // Statement 2
    y = 6;    // Statement 3
    z = x + y;  // Statement 4
    ```
## **2) Chương trình JavaScript**
- Chương trình **JavaScript** là một tập hợp gồm nhiều câu lệnh **JavaScript** .
- Trong một chương trình, các câu lệnh sẽ được thực thi lần lượt theo thứ tự từ trên xuống dưới ( câu lệnh phía trên phải thực thi xong thì câu lệnh bên dưới mới được thực thi ) .
- Nếu câu lệnh phía trên bị lỗi thì tất cả những câu lệnh còn lại ở bên dưới sẽ không được thực thi .
- **VD :**
    ```js
    var x, y, z;  // Statement 1
    x = 5;    // Statement 2
    y = 6;    // Statement 3
    z = x + y;  // Statement 4

    document.getElementById("demo").innerHTML =
    "The value of z is " + z + "."; 
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/ThR2hNk.png>

## **3) Một vài quy tắc khi viết code JavaScript**
### **3.1) Sử dụng dấu "`;`"**
- Mỗi dấu "`;`" ngăn cách 1 câu lệnh **JavaScript** .
- Cần phải chú ý thêm dấu "`;`" mỗi khi kết thúc một câu lệnh thực thi .
- **VD :**
    ```js
    var a, b, c;     // Declare 3 variables
    a = 5;           // Assign the value 5 to a
    b = 6;           // Assign the value 6 to b
    c = a + b;       // Assign the sum of a and b to c
    ```
- Khi sử dụng dấu "`;`", có thể code nhiều câu lệnh **JS** trên 1 dòng :
    ```js
    a = 5; b = 6; c = a + b;
    ```
### **3.2) Khoảng trắng giữa các toán tử**
- **JavaScript** không quan tâm đến ít hay nhiều khoảng trắng giữa các toán tử . Có thể thêm 1 dấu `space` giữa các toán tử cho dễ đọc hơn 
- **VD :** 3 câu lệnh sau hoàn toàn giống nhau :
    ```js
    var person         =            "Hege";
    var person = "Hege";      // Should
    var person="Hege";
    ```
### **3.3) Chiều dài dòng code**
- Để code dễ đọc nhất , người lập trình nên tránh để dòng code dài hơn `80` ký tự .
- Nếu một câu lệnh không thể fit vừa 1 dòng , nên xuống dòng (tốt nhất là sau một toán tử) :
    ```js
    document.getElementById("demo").innerHTML =
    "Hello Dolly!";
    ```
### **3.4) Code Block**
- Các câu lệnh **JavaScript** có thể được nhóm lại thành các khối code , đặt bên trong cặp dấu ngoặc nhọn `{}`
- Mục đích của việc tạo ra các **code block** là để định nghĩa các câu lệnh được thực hiện cùng lúc ( tương tự như việc tạo ra 1 hàm )
    ```js
    function myFunction() {
      document.getElementById("demo1").innerHTML = "Hello Dolly!";
      document.getElementById("demo2").innerHTML = "How are you?";
    }
    ```
### **3.5) Các keyword**
- Các câu lệnh **JavaScript** thường bắt đầu bằng 1 keyword để nhận định action sẽ được thực hiện .
- Một số các keyword thường gặp :
    
    | Keyword | Mô tả |
    |---------|-------|
    | `break` | Thoát khỏi vòng lặp |
    | `continue` | Nhảy ra khỏi vòng lặp để thực hiện câu lệnh đầu tiên của vòng lặp |
    | `debugger` | Dừng thực hiện đoạn code mà gọi hàm debugging |
    | `do...while` | Thực hiện lặp lại 1 khối lệnh , khi condition vẫn `true` |
    | `for` | Chọn khối code cần thực hiện khi condition vẫn `true` |
    | `function` | Khai báo 1 hàm |
    | `if...else` | Chọn khối code cần thực hiện dựa vào condition | 
    | `return` | Thoát khỏi vòng lặp |
    | `switch` | Chọn khối code cần thực hiện dựa vào các trường hợp khác nhau |
    | `try...catch` | Khai báo action xảy ra khi đoạn code bị lỗi |
    | `var` | Khai báo 1 biến |