# Let
- **ES2015** giới thiệu 2 từ khóa quan trọng của **JavaScript** : `let` và `const` .
- Đây là 2 từ khóa cung cấp biến **Block Scope** ( và hằng số ) trong **JavaScript** .
- Trước **ES2015**, **JavaScript** chỉ có 2 loại scope : **Global Scope** và **Function Scope** .
    - **Global Scope** : biến được khai báo bên ngoài hàm . Biến Global có thể được truy cập từ bất cứ nơi nào trong chương trình :
        ```js
        var carName = "Volvo";
        // code here can use carName

        function myFunction() {
        // code here can also use carName
        }
        ```
    - **Function Scope** : biến được khai báo local trong function , chỉ sử dụng được trong function .
        ```js
        // code here can NOT use carName

        function myFunction() {
        var carName = "Volvo";
        // code here CAN use carName
        }

        // code here can NOT use carName
        ```
        