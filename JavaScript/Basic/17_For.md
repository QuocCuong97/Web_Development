# For
## **1) Cấu trúc `For`**
- Cú pháp :
    ```js
    for (statement 1; statement 2; statement 3) {
      // code block to be executed
    }
    ```
    - Trong đó :
        - ***statement 1*** được thực thi 1 lần trước khi thực thi khối code
        - ***statement 2*** khai báo điều kiện để thực thi khối code . Nếu ***statement 2*** là `true` , khối code sẽ được thực hiện lặp đi lặp lại cho đến khi ***statement 2*** `false`
        - ***statement 3*** được thực thi sau mỗi lần khối code được thực thi 
- **VD1 :**
    ```js
    for (i = 0; i < 5; i++) {
      text += "The number is " + i + "<br>";
    }
    ```
    => Kết quả :
    ```
    The number is 0
    The number is 1
    The number is 2
    The number is 3
    The number is 4
    ```
- ***Statement 1*** có thể được bỏ qua nếu đã khai báo giá trị khởi tạo từ trước đó :
    ```js
    var i = 2;
    var len = cars.length;
    var text = "";
    for (; i < len; i++) {
      text += cars[i] + "<br>";
    }
    ```
## **2) Cấu trúc `For/In`**
- Cấu trúc **`for/in`** sẽ thực hiện vòng lặp thông qua các giá trị thuộc tính của một **object** .
- **VD :**
    ```js
    var person = {fname:"John", lname:"Doe", age:25};

    var text = "";
    var x;
    for (x in person) {
      text += person[x];
    }
    ```
    => Kết quả : `John Doe 25`
## **3) Cấu trúc `For/Of`**
- Cấu trúc **`for/of`** sẽ thực hiện vòng lặp thông qua các giá trị của một **iterable object** ( **Array**, **String**, **Map**, **Nodelist**, ....)
- Cú pháp :
    ```js
    for (variable of iterable) {
      // code block to be executed
    }
    ```
- **VD1 :** Loop qua **array** :
    ```js
    var cars = ['BMW', 'Volvo', 'Mini'];
    var x;

    for (x of cars) {
      document.write(x + "<br >");
    }
    ```
    => Kết quả :
    ```
    BMW
    Volvo
    Mini
    ```
- **VD2 :** Loop qua **string** :
    ```js
    var txt = 'JavaScript';
    var x;

    for (x of txt) {
      document.write(x + "<br >");
    }
    ```
