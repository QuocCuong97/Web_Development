# Tổng quan về Object
- Trong **JavaScript**, hầu hết mọi thứ đều là **object** ,
    - **Booleans** có thể là **object** ( nếu được định nghĩa bằng từ khóa `new` )
    - **Number** có thể là **object** ( nếu được định nghĩa bằng từ khóa `new` )
    - **String** có thể là **object** ( nếu được định nghĩa bằng từ khóa `new` )
    - **Date** luôn là **object** .
    - **Math** luôn là **object** .
    - **Regular Expression** luôn là **object** .
    - **Array** luôn là **object** .
    - **Function** luôn là **object** .
    - **Object** luôn là **object** 
- Trong tất cả các giá trị **JavaScript**, ngoại trừ các giá trị nguyên thủy, tất cả đều là **object**
## **1) Cách khởi tạo một Object**
### **1.1) Sử dụng định nghĩa của object**
- Đây là cách dễ nhất để tạo một **JavaScript Object** .
- Một cấu trúc định nghĩa **object** là một list các cặp `tên: giá trị` được đặt trong cùng một dấu "`{}`"
    ```js
    var person = {firstName:"John", lastName:"Doe", age:50, eyeColor:"blue"};
    ```
- Có thể ngắt thành nhiều dòng giúp cấu trúc **object** dễ nhìn hơn :
    ```js
    var person = {
      firstName: "John",
      lastName: "Doe",
      age: 50,
      eyeColor: "blue"
    };
    ```
### **1.2) Sử dụng từ khóa `new`**
- **VD :**
    ```js
    var person = new Object();
    person.firstName = "John";
    person.lastName = "Doe";
    person.age = 50;
    person.eyeColor = "blue";
    ```
## **2) Thuộc tính của object**
- Các thuộc tính là các giá trị song hành cùng **object** .
- Một **object** là tập hợp của nhiều thuộc tính được sắp xếp không theo thứ tự .
### **2.1) Truy cập vào từng thuộc tính**
- Có 3 cú pháp để truy cập các thuộc tính của 1 **object** là :
    ```js
    objectName.property         // person.age
    ```
    hoặc
    ```js
    objectName["property"]      // person["age"]
    ```
    hoặc
    ```js
    objectName[expression]      // x = "age"; person[x]
    ```
### **2.2) Vòng lặp `for...in`**
- Mệnh đề vòng lặp `for...in` sẽ lặp đi lặp lại thông qua các thuộc tính của **object** .
- Cú pháp :
    ```js
    for (variable in object) {
      // code to be executed
    }
    ```
- **VD :**
    ```js
    var person = {fname:"John", lname:"Doe", age:25};

    for (x in person) {
      txt += person[x];
    }
    ```
    => Kết quả : `txt = John Doe 25`
### **2.3) Thêm thuộc tính mới vào object**
- Có thể thêm thuộc tính mới vào **object** đã có sẵn bằng cách chỉ cần gắn cho nó một giá trị .
- **VD :**
    ```js
    var person = {
      firstname:"John",
      lastname:"Doe",
      age:50,
      eyecolor:"blue"
    };
    person.nationality = "English";
    ```
### **2.4) Xóa thuộc tính của object**
- Sử dụng từ khóa `delete` để xóa thuộc tính của 1 **object** .
- **VD :**
    ```js
    var person = {firstName:"John", lastName:"Doe", age:50, eyeColor:"blue"};
    delete person.age;   // or delete person["age"];
    ```
- Từ khóa `delete` sẽ xóa cả thuộc tính và giá trị của nó ra khỏi **object** .
## **3) Các phương thức Object**
### **3.1) Từ khóa `this`**
- Tương tự như từ khóa `self` trong **Python**, `this` ở đây đại diện cho chính chủ thể **object**
- **VD :**
    ```js
    var person = {
      firstName: "John",
      lastName : "Doe",
      id       : 5566,
      fullName : function() {
        return this.firstName + " " + this.lastName;
      }
    };
    ```
### **3.2) Sử dụng các phương thức có sẵn**
- **VD :**
    ```js
    var message = "Hello world!";
    var x = message.toUpperCase();
    ```
### **3.3) Thêm phương thức vào object**
- **VD :**
    ```js
    person.name = function () {
      return this.firstName + " " + this.lastName;
    };
    ```