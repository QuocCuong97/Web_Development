# If...else
## **1) `If`**
- Sử dụng mệnh đề `if` để khai báo 1 khối code **JavaScript** sẽ được thực hiện nếu điều kiện đưa ra là `true` .
- Cú pháp :
    ```js
    if (condition) {
      //  block of code to be executed if the condition is true
    }
    ```
- **VD :**
    ```js
    if (hour < 18) {
      greeting = "Good day";
    }
    ```
    => Kết quả : `greeting = Good day`
## **2) `If...else`**
- Sử dụng mệnh đề `else` để khai báo 1 khối code **JavaScript** sẽ được thực hiện nếu điều kiện đưa ra là `false` .
- Cú pháp :
    ```js
    if (condition) {
      //  block of code to be executed if the condition is true
    } else {
      //  block of code to be executed if the condition is false
    }
    ```
- **VD :**
    ```js
    if (hour < 18) {
      greeting = "Good day";
    } else {
      greeting = "Good evening";
    }
    ```
    => Kết quả : `greeting = Good day`
## **3) `If...else if...else`**
- Sử dụng mệnh đề `else if` để khai báo điều kiện mới nếu điều kiện trước đó là `false` .
- Cú pháp :
    ```js
    if (condition1) {
      //  block of code to be executed if condition1 is true
    } else if (condition2) {
      //  block of code to be executed if the condition1 is false and condition2 is true
    } else {
      //  block of code to be executed if the condition1 is false and condition2 is false
    }
    ```
- **VD :**
    ```js
    if (time < 10) {
      greeting = "Good morning";
    } else if (time < 20) {
      greeting = "Good day";
    } else {
      greeting = "Good evening";
    }
    ```
    => Kết quả : `greeting = Good day`