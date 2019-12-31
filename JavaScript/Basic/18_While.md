# While
## **1) Cấu trúc `while`**
- Mệnh đề `While` dùng để lặp đi lặp lại 1 khối code trong khi condition vẫn `true` .
- Cú pháp :
    ```js
    while (condition) {
      // code block to be executed
    }
    ```
- **VD :**
    ```js
    while (i < 10) {
      text += "The number is " + i;
      i++;
    }
    ```
    => Kết quả :
    ```
    The number is 0
    The number is 1
    The number is 2
    The number is 3
    The number is 4
    The number is 5
    The number is 6
    The number is 7
    The number is 8
    The number is 9
    ```
## **2) Cấu trúc `do/while`**
- Vòng lặp `do/while` là một biến thể của vòng lặp `while` .
- Dạng vòng lặp này sẽ thực hiện khối code block 1 lần , trước khi kiểm tra điều kiện có `true` không , rồi mới tiếp tục chạy lặp lại khối code .
- Cú pháp :
    ```js
    do {
      // code block to be executed
    }
    while (condition);
    ```
- **VD :**  
    ```js
    do {
      text += "The number is " + i;
      i++;
    }
    while (i < 10);
    ```
    => Kết quả :
    ```
    The number is 0
    The number is 1
    The number is 2
    The number is 3
    The number is 4
    The number is 5
    The number is 6
    The number is 7
    The number is 8
    The number is 9
    ```
