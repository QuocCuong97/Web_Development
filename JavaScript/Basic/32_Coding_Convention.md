# Coding Convention
## **1) Các quy tắc đặt tên**
- Tên biến và tên hàm sử dụng kiểu chữ **camelCase** .
    ```js
    var firstName;
    ```
- Biến **global** sử dụng kiểu chữ **UPPERCASE** .
- Hằng số sử dụng kiểu chữ **UPPERCASE** .
- Tất cả tên biến phải bắt đầu bằng 1 ký tự .
- Đặt tên file :
    - Các dịch vụ **Unix** như **Apache** phân biệt chữ hoa - chữ thường khi đặt tên file ( `london.jpg` >< `London.jpg` )
    - Các dịch vụ **Microsoft** như **IIS** không phân biệt chữ hoa - chữ thường khi đặt tên file ( `london.jpg` <=> `London.jpg` )
    - Nếu muốn sử dụng cả chữ hoa và chữ thường khi đặt tên file, phải cực kỳ nhất quán .
    - Để tránh các lỗi, nên sử dụng đồng bộ tên file là chữ thường ( nếu có thể ) .
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
## **6) Quy tắc viết lệnh**
- Luôn kết thúc 1 câu lệnh đơn bằng dấu "`;`"
- Đối với những khối lệnh phức tạp :
    - Đặt dấu "`{`" ở cuối dòng đầu tiên 
    - Dùng 1 dấu `space` phía trước dấu "`{`"
    - Đặt dấu "`}`" ở dòng cuối mà không cần dấu cách phía trước 
    - Sau dấu "`}`" không có dấu "`;`"
    ```js
    for (i = 0; i < 5; i++) {
      x += i;
    }
    ```
    ```js
    if (time < 20) {
      greeting = "Good day";
    } else {
      greeting = "Good evening";
    }
    ```
## **7) Quy tắc khai báo Object**
- Đặt dấu "`{`" cùng dòng khai báo tên object
- Sử dụng dấu "`:`" + "`space`" giữa mỗi thuộc tính và giá trị của nó .
- Sử dụng dấu `""` hoặc `''` quanh giá trị chuỗi, còn giá trị số thì không cần .
- Không thêm dấu "`,`" sau cặp thuộc tính-giá trị cuối cùng .
- Đặt dấu "`}`" ở dòng cuối mà không cần dấu cách phía trước .
- Luôn kết thúc việc khai báo **object** bằng một dấu "`;`"
    ```js
    var person = {
      firstName: "John",
      lastName: "Doe",
      age: 50,
      eyeColor: "blue"
    };
    ```
    ```js
    var person = {firstName:"John", lastName:"Doe", age:50, eyeColor:"blue"};
    ```