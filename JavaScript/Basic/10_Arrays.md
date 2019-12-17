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
### **4.8) Phương thức `splice()`**
### **4.9) Phương thức `slice()`**
- Phương thức `slice()` dùng để cắt một phần của mảng ban đầu và tạo thành một mảng mới .
- Phương thức này tạo ra một mảng riêng biệt khác hẳn mảng ban đầu, không làm ảnh hưởng đến mảng ban đầu .
- Nếu chỉ truyền vào 1 tham số, phương thức `slice()` sẽ cắt từ điểm bắt đầu đến hết mảng :
    ```js
    var fruits = ["Banana", "Orange", "Lemon", "Apple", "Mango"];
    var citrus = fruits.slice(1);
    ```
    => Kết quả : `citrus = Orange,Lemon,Apple,Mango`
- Phương thức `slice()` có thể nhận vào 2 tham số là điểm start và điểm end (điểm end sẽ không được tính vào mảng mới) của phần mảng cần cắt :
    ```js
    var fruits = ["Banana", "Orange", "Lemon", "Apple", "Mango"];
    var citrus = fruits.slice(1, 3);
    ```
    => Kết quả : `citrus = Orange,Lemon`
## **5) Sắp xếp mảng trong JavaScript**
### **5.1) Hàm `sort()`**
- Hàm `sort()` sẽ sắp xếp mảng theo thứ tự bảng chữ cái .
- **VD :**
    ```js
    var fruits = ["Banana", "Orange", "Apple", "Mango"];
    fruits.sort();        // Sorts the elements of fruits
    ```
    => Kết quả : `fruits = Apple,Banana,Mango,Orange`
### **5.2) Hàm `reverse()`**
- Hàm `reverse()` sẽ đảo ngược thứ tự của mảng .
- **VD :**
    ```js
    var fruits = ["Banana", "Orange", "Apple", "Mango"];
    fruits.reverse();
    ```
    => Kết quả : `fruits = Mango,Apple,Orange,Banana`
### **5.3) Sắp xếp mảng chứa số**
- Mặc định , hàm `sort()` sắp xếp giá các giá trị của mảng là **string** .
- Tuy nhiên, khi so sánh 2 giá trị **number** mà dưới dạng **string**, số `25` sẽ lớn hơn số `100` ( vì `2 > 1` ) => Sắp xếp bị sai .
- Có thể fix điều này bằng cách sử dụng **hàm so sánh** ( **compare function** ) .
- **VD1 :** Sắp xếp theo chiều tăng dần :
    ```js
    var points = [40, 100, 1, 5, 25, 10];
    points.sort(function(a, b){return a - b});
    ```
    => Kết quả : `points = 1,5,10,25,40,100`
- **VD2 :** Sắp xếp theo chiều giảm dần :
    ```js
    var points = [40, 100, 1, 5, 25, 10];
    points.sort(function(a, b){return b - a});
    ```
    => Kết quả : `points = 100,40,25,10,5,1`
- **VD3 :** Sắp xếp theo thứ tự random :
    ```js
    var points = [40, 100, 1, 5, 25, 10];
    points.sort(function(a, b){return 0.5 - Math.random()});
    ```
    => Kết quả : `points = 40,1,10,100,5,25`
- Từ cách sắp xếp trên , có thể suy ra cách tìm giá trị nhỏ nhất và lớn nhất trong mảng . Sắp xếp theo thứ tự tăng dần
    ```js
    var points = [40, 100, 1, 5, 25, 10];
    points.sort(function(a, b){return a - b});
    ```
    - Giá trị nhỏ nhất là `points[0] = 1`
    - Giá trị lớn nhất là `points[points.length - 1] = 100`
#### **5.3.1) Sử dụng hàm `Math.max()` để tìm giá trị lớn nhất trong mảng**
- Có thể sử dụng công thức `Math.max.apply` để tìm ra phần tử có giá trị lớn nhất trong mảng .
- **VD :**
    ```js
    function myArrayMax(arr) {
      return Math.max.apply(null, arr);
    }
    var points = [40, 100, 1, 5, 25, 10];
    max = myArrayMax(points);
    ```
    => Kết quả : `max = 100`
#### **5.3.2) Sử dụng hàm `Math.min()` để tìm giá trị nhỏ nhất trong mảng**
- Có thể sử dụng công thức `Math.min.apply` để tìm ra phần tử có giá trị lớn nhất trong mảng .
- **VD :**
    ```js
    function myArrayMin(arr) {
      return Math.min.apply(null, arr);
    }
    var points = [40, 100, 1, 5, 25, 10];
    max = myArrayMin(points);
    ```
    => Kết quả : `min = 1`

