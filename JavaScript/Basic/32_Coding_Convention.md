# Coding Convention
## **1) Tên biến**
- Nên sử dụng kiểu chữ **camelCase** ( cho tên biến và tên hàm )
    ```js
    var firstName;
    ```
- Tất cả tên biến phải bắt đầu bằng 1 ký tự .
## **2) Khoảng cách xung quanh các toán tử**
- Luôn đặt khoảng cách (`space`) quanh các toán tử ( `= + - * /` ) và đằng sau dấu "`,`" .
    ```js
    var x = y + z;
    var values = ["Volvo", "Saab", "Fiat"];
    ```
## **3) Thụt đầu dòng**
- Thụt đầu dòng `2-space` để nhận biết các đoạn code :
    ```js
    function toCelsius(fahrenheit) {
      return (5 / 9) * (fahrenheit - 32);
    }
    ```
## **4) Chiều dài tối đa của dòng code**
- Để dễ đọc, tránh 1 dòng code dài hơn `80` ký tự .
- Nếu một mệnh đề **JavaScript** quá dài, cách tốt nhất là ngắt nó ra , sau một toán tử hoặc một dấu "`,`"
    ```js
    document.getElementById("demo").innerHTML =
    "Hello Dolly.";
    ```
## **5) Định dạng file**
- File **JavaScript** phải có định dạng file là `.js`
