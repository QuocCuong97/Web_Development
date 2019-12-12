# Các kiểu dữ liệu
- Trong **JavaScript**, mỗi giá trị dữ liệu sẽ thuộc một nhóm kiểu dữ liệu nhất định .
- Trong **JavaScript**, các kiểu dữ liệu được chia thành những loại cơ bản như sau :
    - **string**
    - **number**
    - **boolean**
    - **object**
    - **undefined**
    - **array** - trường hợp đặc biệt của kiểu dữ liệu **object**
### **1) Kiểu dữ liệu `string`**
- Là một chuỗi các ký tự, được đặt trong dấu nháy đơn ( `''` ) hoặc dấu ngoặc kép ( `""` ) .
- **VD :**
    ```js
    var answer1 = "It's alright";             // Single quote inside double quotes
    var answer2 = "He is called 'Johnny'";    // Single quotes inside double quotes
    var answer3 = 'He is called "Johnny"';    // Double quotes inside single quotes
    ```
### **2) Kiểu dữ liệu `number`**
- Là một tập hợp của các con số ( `0 - 9` ) không chứa dấu khoảng trắng và có thể chứa dấu trừ ( `-` ) nằm ở đầu để đại diện cho số âm .
- **VD :**
    ```js
    var x1 = 34.00;
    var x2 = 34; 
    var y = 123e5;
    var z = 123e-5;
    ```
### **3) Kiểu dữ liệu `boolean`**
- Trong **JavaScript**, dữ liệu thuộc kiểu **boolean** chỉ có thể nhận một trong hai giá trị, đó là :
    - `true` - đúng
    - `false` - sai
- Có 2 cách để nhận giá trị kiểu **boolean** :
    - Gán giá trị trực tiếp
    - Nhận được từ một điều kiện
- **VD :**
    ```js
    var a = true;
    var b = false;
    var c = 6 > 2;
    var d = 6 > 10;
    ```
### **4) Kiểu dữ liệu `object`**
- Trong **JavaScript**, dữ liệu thuộc kiểu **object** (hay còn được gọi là "đối tượng") là một tập hợp gồm các thuộc tính và mỗi thuộc tính sẽ chứa đựng một giá trị dữ liệu.
- **VD :**
    ```js
    var person = {
      firstName : "John",
      lastName  : "Doe",
      age     : 50,
      eyeColor  : "blue"
    };
    ```
    hoặc
    ```js
    var person = {firstName:"John", lastName:"Doe", age:50, eyeColor:"blue"};
    ```
### **5) Kiểu dữ liệu `undefined`**
- Trong **JavaScript**, khi một biến được khai báo mà không gán giá trị thì biến đó sẽ có giá trị là `undefined` và kiểu dữ liệu cũng là **undefined** . 
- **VD :**
    ```js
    var myName;
    ```
- Hoặc cũng có thể gán kiểu dữ liệu **undefined** ngay từ đầu :
    ```js
    var myName = undefined;
    ```
### **6) Kiểu dữ liệu `array`**
- Trong **JavaScript**, **array** còn được gọi là "mảng", là một trường hợp đặc biệt của đối tượng.
- **Mảng** thực ra có kiểu dữ liệu là **object** .
- **Mảng** là một loại biến đặc biệt có thể lưu trữ nhiều giá trị đồng thời, mỗi giá trị được gọi là một phần tử mảng .
- **VD :**
    ```js
    var mobile = ["HTC","Nokia","SamSung"];
    ```
## **Cách xác định kiểu dữ liệu**
- Để xác định kiểu của một dữ liệu , sử dụng toán tử `typeof` :
    ```js
    var a = typeof ""; //string
    var b = typeof "Lập Trình Web"; //string
    var c = typeof 1993; //number
    var d = typeof true; //boolean
    var e = typeof false; //boolean
    var f = typeof {name:"Nhân", gender:"Nam", year:1993}; //object
    var g = typeof undefined; //undefined
    var h = typeof ["HTC","Nokia","SamSung"]; //object
    ```
