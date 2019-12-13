# Arrays
## **1) Kiểu dữ liệu `array`**
- **Mảng** ( **array** ) là một loại biến đặc biệt, có thể lưu trữ nhiều giá trị đồng thời .
    ```js
    var mobile = ["HTC", "Nokia", "SamSung", "LG", "Apple"];
    ```
- Mỗi giá trị của **mảng** được gọi là một "**phần tử mảng**" và mỗi **phần tử mảng** thì được xác định bởi một chỉ số . Phần tử mảng đầu tiên sẽ có chỉ số là `0` , chỉ số của các phần tử mảng sẽ tăng dần theo thứ tự được khai báo .

    | HTC | Nokia | Samsung | LG | Apple |
    |-----|-------|---------|----|-------|
    | `0` | `1` | `2` | `3` | `4` |
- Cách tạo một mảng :
    ```js
    var array_name = [item1, item2, ...]; 
    ```
- **VD :**
    ```js
    var cars = ["Saab", "Volvo", "BMW"];
    ```
    hoặc
    ```js
    var cars = [
      "Saab",
      "Volvo",
      "BMW"
    ];
    ```
- Hoặc cách khác để tạo 1 mảng :
    ```js
    var array_name = new Array(item1, item2, ...);
    ```
## **2) Các thao tác với phần tử của mảng**
### **2.1) Truy cập phần tử mảng**
- Để truy cập phần tử mảng, ta sử dụng chỉ số của phần tử mảng ( **index number** ) theo cú pháp :
    ```js
    array_name[index]
    ```
- **VD :**
    ```js
    var cars = ["Saab", "Volvo", "BMW"];
    document.getElementById("demo").innerHTML = cars[0];
    document.getElementById("demo").innerHTML = cars[1];
    document.getElementById("demo").innerHTML = cars[2];
    ```
    => Kết quả :
    ```
    Saab
    Volvo
    BMW
    ```
### **2.2) Thay đổi phần tử mảng**
- Có thể thay đổi trực tiếp phần tử của mảng bằng **index number** .
- **VD :**
    ```js
    array_name[index] = new_value
    ```
- **VD :**
    ```js
    var cars = ["Saab", "Volvo", "BMW"];
    cars[0] = "VinFast"
    document.getElementById("demo").innerHTML = cars[0];
    ```
    => Kết quả :
    ```
    VinFast
    ```
### **2.3) Gọi tất cả các phần tử mảng cùng lúc**
- Riêng với JavaScript, có thể gọi tất cả các phần tử mảng cùng một lúc .
- **VD :**
    ```js
    var cars = ["Saab", "Volvo", "BMW"];
    document.getElementById("demo").innerHTML = cars;
    ```
    => Kết quả :
    ```
    Saab,Volvo,BMW
    ```
## **3) Mảng có thể trở thành object**
## **4) Các phương thức làm việc với mảng**
### **4.1) Thuộc tính `length`**
- Thuộc tính `length` trả về số phần tử của mảng .
- **VD1 :** Tính số phần tử của mảng :
    ```js
    var fruits = ["Banana", "Orange", "Apple", "Mango"];
    fruits.length;   // the length of fruits is 4
    ```
- **VD2 :** Gọi phần tử cuối cùng của mảng :
    ```js
    var fruits = ["Banana", "Orange", "Apple", "Mango"];
    var last = fruits[fruits.length - 1];
    ```
    => Kết quả : `last = Mango`
- **VD3 :** Loop với mảng (cách tốt nhất là sử dụng vòng lặp `for`):
    ```js
    var fruits, text, fLen, i;
    fruits = ["Banana", "Orange", "Apple", "Mango"];
    fLen = fruits.length;

    text = "<ul>";
    for (i = 0; i < fLen; i++) {
      text += "<li>" + fruits[i] + "</li>";
    }
    text += "</ul>"; 
    document.getElementById("demo").innerHTML = text;
    ```
    hoặc sử dụng hàm `forEach()` :
    ```js
    var fruits, text;
    fruits = ["Banana", "Orange", "Apple", "Mango"];

    text = "<ul>";
    fruits.forEach(myFunction);
    text += "</ul>";

    function myFunction(value) {
      text += "<li>" + value + "</li>";
    }
    document.getElementById("demo").innerHTML = text;
    ```
    => Hiển thị trên trình duyệt :

    <img src=https://i.imgur.com/uH1gsDE.png>
### **4.2) Phương thức `push()`**
- Phương thức `push()` sử dụng để thêm phần tử vào vị trí cuối của mảng .
- **VD1 :**
    ```js
    var fruits = ["Banana", "Orange", "Apple", "Mango"];
    fruits.push("Lemon");
    document.getElementById("demo").innerHTML = fruits;
    ```
    => Kết quả :
    ```
    Banana,Orange,Apple,Mango,Lemon
    ```
- **VD2 :** Sử dụng thuộc tính `length` để thêm phần tử vào mảng :
    ```js
    var fruits = ["Banana", "Orange", "Apple", "Mango"];
    fruits[fruits.length] = "Lemon";
    ```
### **4.3) Phương thức `toString()`**
- Phương thức `toString()` chuyển đổi một mảng thành một chuỗi chứa các giá trị của mảng, được ngăn cách bằng dấu "`,`"
- **VD :**
    ```js
    var fruits = ["Banana", "Orange", "Apple", "Mango"];
    document.getElementById("demo").innerHTML = fruits.toString();
    ```
    => Kết quả :
    ```
    Banana,Orange,Apple,Mango
    ```
### **4.4) Phương thức `join()`**
- Phương thức `join()` chuyển đổi một mảng thành một chuỗi chứa các giá trị của mảng, được ngăn cách một tham số tùy chọn (do người lập trình truyền vào) :
- **VD :**
    ```js
    var fruits = ["Banana", "Orange", "Apple", "Mango"];
    document.getElementById("demo").innerHTML = fruits.join(" * ");
    ```
    => Kết quả :
    ```
    Banana * Orange * Apple * Mango
    ```
### **4.5) Phương thức `pop()`**
- Phương thức `pop` sẽ xóa phần tử cuối cùng của mảng .
- **VD :**
    ```js
    var fruits = ["Banana", "Orange", "Apple", "Mango"];
    fruits.pop(); 
    document.getElementById("demo2").innerHTML = fruits;
    ```
    => Kết quả :
    ```
    Banana,Orange,Apple
    ```
### **4.6) Phương thức `shift()`**
- Phương thức `shift()` hoạt động tương tự với `pop()` , khác là nó sẽ xóa phần tử đầu tiên của mảng .
- **VD :**
    ```js
    var fruits = ["Banana", "Orange", "Apple", "Mango"];
    fruits.shift(); 
    document.getElementById("demo2").innerHTML = fruits;
    ```
    => Kết quả :
    ```
    Orange,Apple,Mango
    ```
### **4.7) Phương thức `unshift()`**
- Phương thức `unshift()` sẽ thêm tham số được truyền vào trở thành phần tử đầu tiên của mảng .
- **VD :**
    ```js
    var fruits = ["Banana", "Orange", "Apple", "Mango"];
    fruits.unshift("Lemon");
    document.getElementById("demo2").innerHTML = fruits;
    ```
    => Kết quả :
    ```
    Lemon,Banana,Orange,Apple,Mango
    ```
### **4.8) Phương thức 