# Location
- **Object** `window.location` được sử dụng để trả về địa chỉ **URL** của trang hiện tại và để điều hướng trình duyệt tới trang mới .
- **Object** `window.location` có thể được gọi mà không cần tiền tố `window` .
## **1) Thuộc tính `href`**
- Thuộc tính `window.location.href` trả về địa chỉ **URL** của trang hiện tại .
- **VD :**
    ```js
    document.getElementById("demo").innerHTML = "Page location is " + window.location.href;
    ```
    => Kết quả : `Page location is https://www.w3schools.com/js/js_window_location.asp`
## **2) Thuộc tính `hostname`**
- Thuộc tính `window.location.hostname` trả về tên của host đang đứng trên Internet .
- **VD :**
    ```js
    document.getElementById("demo").innerHTML = "Page hostname is " + window.location.hostname;
    ```
    => Kết quả : `Page hostname is www.w3schools.com`
## **3) Thuộc tính `pathname`**
- Thuộc tính `window.location.pathname` trả về đường dẫn tương đối của trang web hiện tại đối với trang chủ >
- **VD :**
    ```js
    document.getElementById("demo").innerHTML = "Page path is " + window.location.pathname;
    ```
    => Kết quả : `Page path is /js/js_window_location.asp`
## **4) Thuộc tính `protocol`**
- Thuộc tính `window.location.protocol` trả về giao thức web của trang ( `http` hay `https` )
- **VD :**
    ```js
    document.getElementById("demo").innerHTML = "Page protocol is " + window.location.protocol;
    ```
    => Kết quả : `Page protocol is https:`
## **5) Thuộc tính `port`**
- Thuộc tính `window.location.port` trả về số port kết nối internet của host ( của trang hiện tại )
    > Nếu trang web sử dụng port mặc định là `80` hoặc `443` thì phần lớn các trình duyệt sẽ hiển thị là `0` hoặc không có gì .
- **VD :**
    ```js
    document.getElementById("demo").innerHTML = "Port number is " + window.location.port;
    ```
    => Kết quả : `Port number is`
## **6) Phương thức `assign()`**
- Phương thức `assign()` sẽ load 1 trang web mới .
- **VD :**
    ```js
    <html>
    <head>
    <script>
    function newDoc() {
      window.location.assign("https://www.w3schools.com")
    }
    </script>
    </head>
    <body>

    <input type="button" value="Load new document" onclick="newDoc()">

    </body>
    </html>
    ```