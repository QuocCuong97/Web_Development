# Từ khóa `this`
- `this` trong Javascript nó cũng giống như các ngôn ngữ khác, đều là đại diện cho đối tượng hiện tại mà nó đang được sử dụng.
### **`this` trong Method**
- Trong một method, từ khóa `this` đại diện cho chủ thể object :
    ```js
    var person = {
      firstName: "John",
      lastName : "Doe",
      id     : 5566,
      fullName : function() {
      return this.firstName + " " + this.lastName;
      }
    };
    document.getElementById("demo").innerHTML = person.fullName();
    ```
    => Kết quả :
    ```
    John Doe
    ```
- Tuy nhiên nếu `this` đứng một mình trong trường hợp này thì kết quả sẽ khác :
    ```js
    var person = {
      firstName: "John",
      lastName : "Doe",
      id     : 5566,
      fullName : function() {
      return this;
      }
    };
    document.getElementById("demo").innerHTML = person.fullName();
    ```
    => Kết quả :
    ```
    [object Object]
    ```
### **`this` đứng một mình**
- Khi đứng một mình , `this` đại diện cho một global object 
- Ở trong cửa sổ trình duyệt, global object chính là `[object Window]`
    ```js
    var x = this;
    document.getElementById("demo").innerHTML = x;
    ```
    => Kết quả :
    ```
    [object Window]
    ```
- strictmode?????????
### **`this` trong function (mặc định)**
- Trong một function, `this` đại diện cho chủ thể sở hữu function
    ```js
    document.getElementById("demo").innerHTML = myFunction();
    function myFunction() {
      return this;
    }
    ```
    => Kết quả :
    ```
    [object Window]
    ```
### **`this` trong function (strict mode)**
- Trong **strict mode** , `this` không cho phép tham chiếu. Vì vậy, khi đặt trong function, nó sẽ trở thành `undefined`
    ```js
    "use strict";
    document.getElementById("demo").innerHTML = myFunction();
    function myFunction() {
      return this;
    }
    ```
    => Kết quả :
    ```
    undefined
    ```
### **`this` khi xử lý event HTML**
- Khi xử lý event HTML, `this` đại diện cho chính phần tử HTML nhận được event :
    ```html
    <button onclick="this.style.display='none'">
      Click to Remove Me!
    </button>
    ```
