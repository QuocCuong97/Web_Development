# Try...Catch
- **JavaScript** cung cấp bốn loại lệnh dùng để kiểm soát và xử lý lỗi: `try`, `catch`, `throw`, `finally`
## **1) `try` và `catch`**
- Khi thực thi một đoạn code **JavaScript**, nếu một câu lệnh nào đó bị lỗi thì việc thực thi sẽ kết thúc ( tất cả những câu lệnh nằm phía sau câu lệnh bị lỗi sẽ không được thực thi ) . Lệnh `try` giúp tránh tình trạng này .
- Lệnh `try` cho phép định nghĩa 1 khối code sẽ được test xem có lỗi hay không trước khi được thực thi .
- Lệnh `catch` cho phép định nghĩa 1 khối code sẽ được thực thi nếu có lỗi xảy ra trong khối code `try` .
- Lệnh `try` và `catch` thường được sử dụng thành 1 cặp :
    ```js
    try {
      Block of code to try
    }
    catch(err) {
      Block of code to handle errors
    }
    ```
## **2) `throw`**
- Khi có lỗi xảy ra, **JavaScript** sẽ dừng lại và đưa ra 1 thông báo lỗi .
- Lệnh `throw` được sử dụng để tự tạo ra 1 câu lệnh lỗi . 
    >  Sau khi lệnh `throw` được thực thi thì một lỗi sẽ được tạo ra, điều đó cũng đồng nghĩa với việc câu lệnh bị lỗi . Do đó , những câu lệnh còn lại nằm phía sau lệnh `throw` sẽ không được thực thi.
- Lỗi được tạo ra có thể là một **JavaScript** ***string***, ***number*** , ***boolean*** hoặc 1 ***object*** .
    ```js
    throw "Too big";    // throw a text
    throw 500;          // throw a number
    ```
- Sử dụng `throw` kết hợp với `try` và `catch` có thể giúp kiểm soát luồng chương trình và đưa ra những lỗi được lập trình trước .
- **VD1 :** Có thể áp dụng `throw` vào thuật toán validate input cho form . Nếu giá trị nhập vào sai, sẽ có lỗi hiện ra :
    ```html
    <!DOCTYPE html>
    <html>
    <body>

    <p>Please input a number between 5 and 10:</p>

    <input id="demo" type="text">
      <button type="button" onclick="myFunction()">Test Input</button>
    <p id="p01"></p>

    <script>
    function myFunction() {
      var message, x;
       message = document.getElementById("p01");
      message.innerHTML = "";
      x = document.getElementById("demo").value;
      try {
        if(x == "") throw "empty";
        if(isNaN(x)) throw "not a number";
        x = Number(x);
        if(x < 5) throw "too low";
        if(x > 10) throw "too high";
      }
      catch(err) {
        message.innerHTML = "Input is " + err;
      }
    }
    </script>

    </body>
    </html>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/WLwow9Q.png>
## **3) `finally`**
- Lệnh `finally` cho phép thực thi 1 khối code, sau khối `try` và `catch`, cho dù kết quả có thế nào .
    ```js
    try {
      //Block of code to try
    }
    catch(err) {
      //Block of code to handle errors
    }
    finally {
      //Block of code to be executed regardless of the try / catch result
    }
    ```
- **VD :**
    ```js
    function myFunction() {
      var message, x;
      message = document.getElementById("p01");
      message.innerHTML = "";
      x = document.getElementById("demo").value;
      try {
        if(x == "") throw "is empty";
        if(isNaN(x)) throw "is not a number";
        x = Number(x);
        if(x > 10) throw "is too high";
        if(x < 5) throw "is too low";
      }
      catch(err) {
        message.innerHTML = "Error: " + err + ".";
      }
      finally {
        document.getElementById("demo").value = "";
      }
    }
    ```
## **4) Error Object**
- **JavaScript** có sử dụng 1 loại **error object** để cung cấp thông tin về lỗi nếu có lỗi xảy ra .
- **Error object** cung cấp 2 thuộc tính hữu ích :
    - ***name*** : trả về tên lỗi
    - ***message*** : trả về nội dung lỗi ( dạng chuỗi )
- Các giá trị của ***name*** :
    - `RangeError` sẽ được đưa ra nếu user sử dụng số nằm ngoài vùng giá trị cho phép .
        ```js
        var num = 1;
        try {
          num.toPrecision(500);   // A number cannot have 500 significant digits
        }
        catch(err) {
          document.getElementById("demo").innerHTML = err.name;
        }
        ```
        => Kết quả : `RangeError`
    - `ReferenceError` sẽ được đưa ra nếu sử dụng 1 biến không được khai báo trước :
        ```js
        var x;
        try {
          x = y + 1;   // y cannot be referenced (used)
        }
        catch(err) {
          document.getElementById("demo").innerHTML = err.name;
        }
        ```
        => Kết quả : `ReferenceError`
    - `SyntaxError` sẽ được đưa ra nếu câu lệnh bị sai cú pháp :
        ```js
        try {
          eval("alert('Hello)");   // Missing ' will produce an error
        }
        catch(err) {
          document.getElementById("demo").innerHTML = err.name;
        }
        ```
        => Kết quả : `SyntaxError`
    - `TypeError` sẽ được đưa ra nếu giá trị đưa vào sai với loại giá trị mong muốn :
        ```js
        var num = 1;
        try {
          num.toUpperCase();   // You cannot convert a number to upper case
        }
        catch(err) {
          document.getElementById("demo").innerHTML = err.name;
        }
        ```
        => Kết quả : `TypeError`
    - `URIError` ( *Uniform Resource Identifier* ) sẽ được đưa ra nếu sử dụng các ký tự không hợp lệ trong hàm xử lý URI :
        ```js
        try {
          decodeURI("%%%");   // You cannot URI decode percent signs
        }
        catch(err) {
          document.getElementById("demo").innerHTML = err.name;
        }
        ```
    