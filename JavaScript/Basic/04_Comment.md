# Comment trong JavaScript
- **Comment** trong **JavaScript** có thể được sử dụng để giải thích code , làm cho chúng dễ đọc hơn .
- **Comment** cũng có thể sử dụng để test code , không cho 1 câu lệnh nào đó được thực thi .
### **1) Single-line Comment**
- **Single-line comment** bắt đầu bằng dấu "`//`" .
- Bất cứ đoạn text nào nằm trên dòng và sau dấu `//` đều bị **JavaScript** bỏ qua ( không thực hiện )
- **VD :**
    ```js
    var x = 5;      // Declare x, give it the value of 5
    var y = x + 2;  // Declare y, give it the value of x + 2

    // Change heading:
    document.getElementById("myH").innerHTML = "My First Page";

    // Change paragraph:
    document.getElementById("myP").innerHTML = "My first paragraph.";
    ```
### **2) Multi-line Comment**
- **Multi-line comment** bắt đầu bằng dấu `/*` và kết thúc bằng dấu `*/` .
- Bất cứ đoạn text nào nằm giữa cặp dấu `/*` và `*/` đều bị **JavaScript** bỏ qua .
- **VD :**
    ```js
    /*
    The code below will change
    the heading with id = "myH"
    and the paragraph with id = "myP"
    in my web page:
    */
    document.getElementById("myH").innerHTML = "My First Page";
    document.getElementById("myP").innerHTML = "My first paragraph.";
    ```