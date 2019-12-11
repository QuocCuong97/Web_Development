# Biến trong JavaScript
- Biến **JavaScript** là các container chứa các giá trị .
- **VD :**
    ```js
    var x = 5;
    var y = 6;
    var z = x + y;
    ```
## **1) Quy tắc đặt tên biến**
- Tên biến có thể gồm 1 hoặc nhiều ký tự .
- Tên biến có thể chứa ký tự, số, dấu gạch dưới ( `_` ) , dấu đô la ( `$` ) .
- Tên biến phải bắt đầu bằng 1 ký tự .
- Tên biến có thể bắt đầu bằng dấu "`$`" và dấu "`_`" ( nâng cao )
- Tên biến phân biệt chữ hoa và chữ thường ( `y` và `Y` là 2 biến khác nhau )
- Tên biến nên đặt tránh các keyword của **JavaScript** .
## **2) Cách khai báo biến**
### **2.1) Khai báo một biến**
- Để khai báo một biến , sử dụng cú pháp :
    ```js
    var <name>;
    ```
- **VD :**
    ```js
    var hoten;
    ```
### **2.2) Gán giá trị cho biến**
- Sau khi khai báo , nếu biến vẫn chưa được gán giá trị cụ thể thì mặc định nó sẽ có giá trị là `undefined` .
- Để gán giá trị cho biến , sử dụng cú pháp :
    ```js
    <var_name> = <value>
    ```
- **VD :**
    ```html
    <head>
      <meta charset="UTF-8">
    </head>
    <body>
    <script>
      var hoten;
      document.write("Giá trị của biến hoten là: " + hoten);
      hoten = "Ngo Quoc Cuong";
      document.write("<br>Giá trị của biến hoten là: " + hoten);
    </script>
    </body>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/6BcM7hj.png>

### **2.3) Cập nhật giá trị biến**
- Sau khi một biến đã được gán giá trị, nếu muốn cập nhật cho nó một giá trị mới thì sử dụng cú pháp :
    ```js
    <var_name> = <new_value>;
    ```
- **VD :**
    ```js
    <script>
      var hoten;
      hoten = "Ngo Quoc Cuong";
      hoten = "Phung Thuy Trang";
    </script>
    ```
### **2.4) Khai báo biến và giá trị đồng thời**
- Sử dụng cú pháp :
    ```js
    var <varname> = <value>;
    ```
- **VD :**
    ```js
    var hoten = "Ngo Quoc Cuong";
    ```
### **2.5) Khai báo đồng thời nhiều biến**
- Có thể khai báo nhiều biến cùng lúc , phân cách nhau bằng dấu "`,`"
- **VD :** 
    ```js
    var x = 1, y = 1, z = 2;
    ```
    hoặc
    ```js
    var x = 1,
    y = 1,
    z = 2;
    ```
## **3) Giá trị của biến**
- Giá trị của biến rất đa dạng, có thể là: một chuỗi ký tự, một số, một biến khác, một biểu thức, undefined, ....
### **3.1) Giá trị của biến là 1 chuỗi ký tự**
- Nếu giá trị của biến là một chuỗi ký tự thì ta phải đặt chuỗi ký tự đó bên trong cặp dấu nháy kép `""` hoặc cặp dấu nháy đơn `''` .
- **VD :**
    ```js
    var ho = "Ngo",
    name = 'Quoc Cuong';
    ```
### **3.2) Giá trị của biến là 1 số**
- Nếu giá trị của biến là 1 số thì không cần đặt trong dấu ngoặc .
- **VD :**  
    ```js
    var x = 1;
    ```
### **3.3) Giá trị của biến là biến khác**
- Giá trị của biến có thể là một biến khác, khi đó nó sẽ lấy giá trị của biến mà nó được gán .
- **VD :**
    ```js
    var x = 5,
    y = x;
    ```
### **3.4) Giá trị của biến là 1 biểu thức**
- Giá trị của biến có thể là một biểu thức . Khi đó, giá trị thực của biến sẽ là kết quả của biểu thức (sau khi đã được tính toán xong).
- **VD :**
    ```js
    var x = 5,
    y = 6,
    z = x + y + 5;
    ```
### **3.5) Giá trị của biến là `undefined`**
- Khi một biến được khai báo mà chưa được gán giá trị thì biến đó sẽ nhận giá trị là `undefined` (không xác định) .
- **VD :**
    ```js
    var a;
    ```


