# Functions
## **1) Các cách khai báo hàm**
### **1.1) Khai báo theo cách truyền thống**
- Cú pháp :
    ```js
    function functionName(parameters) {
        //code
    }
    ```
- Hàm được khai báo theo cách truyền thống sẽ không được thực hiện ngay lập tức. Chúng sẽ được lưu lại, đợi đến khi được gọi mới thực thi
- **VD :**
    ```js
    function myFunction(a, b) {
        return a * b;
    }
    ```
> Vì function khai báo không thực thi luôn nên không kết thúc bằng dấu "`;`" 
### **1.2) Khai báo theo dạng biểu thức**
- **VD :**
    ```js
    var x = function(a, b) { return a * b};
    ```
- Sau khi biểu thức function được lưu trữ dưới dạng biến, biến cũng có thể được sử dụng dưới dạng function :
    ```js
    var z = x(4, 3);
    ```
- Hàm khai báo kiểu này còn được gọi là **hàm nặc danh ( *anynomous function* )** vì chúng lưu trữ dưới dạng biến và không cần tên function .
> Function được viết dưới dạng biểu thức thực thi nên sẽ kết thúc bằng dấu "`;`"
### **1.3) Khai báo theo cấu trúc `Function()`**
- **VD :**
    ```js
    var myFunction = new Function("a", "b", "return a * b");
    var x = myFunction(4, 3);
    ```
### **1.4) Hàm tự gọi**
- Một function tự gọi (***self-invoking***) có thể tự khởi động mà không cần được gọi.
- Để là được điều này , chỉ cần thêm dấu `()` vào sau function .
- Hàm khai báo theo kiểu truyền thống không thể tự gọi .
- **VD :
    ```js
    (function () {
        var x= "Hello!!";
    }) ();
    ```
- Hàm khai báo kiểu này còn được gọi là **hàm nặc danh tự gọi ( *anynomous self-invoking function* )** .
### **1.5) Arrow Function**
- Đây là một công thức rút gọn để viết biểu thức function , không cần từ khóa `function`, không cần từ khóa `return`, không cần các dấu ngoặc nhọn .
- **VD :**
    ```js
    // ES5
    var x = function(x, y) {
        return x * y;
    }

    // ES6
    const x = (x, y) => x * y
    ```
## **2) Function là Object**
- Cấu trúc `typeof` trong JavaScript sẽ trả về "`function`" cho các function .
- Tuy nhiên , function JavaScript có thể là tốt nhất khi được thể hiện dưới dạng **object** .
- Một hàm **JavaScript** có cả thuộc tính và các phương thức :
- Thuộc tính `arguments.length` trả về số lượng tham số truyền vào function khi function được thực thi .
    ```js
    function myFunction(a, b) {
        return arguments.length;
    }
    ```
    => Kết quả : `2`
- Phương thức `toString()` trả về function dưới dạng string :
    ```js
    function myFunction(a, b) {
        return a * b;
    }
    var txt = myFunction.toString();
    ```
    => Kết quả :
    ```
    function myFunction(a, b) { return a * b; }
    ```
## **3) Các tham số và đối số