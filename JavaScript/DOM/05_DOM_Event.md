# DOM Events
## **1) Tác động tới Event**
- Đoạn code **JavaScript** có thể được thực thi khi 1 event xảy ra, như khi user click vào phần tử HTML .
- Để thực hiện đoạn code khi user click vào phần tử, thêm code **JavaScript** vào thuộc tính HTML event :
    ```js
    onclick=JavaScript
    ```
- VD về các HTML Event :
    - Khi user click chuột 
    - Khi trang web được load
    - Khi một hình ảnh được load
    - Khi di chuột qua phần tử
    - Khi trường input thay đổi
    - Khi form được submit
- **VD :** Thay đổi phần tử `<h1>` bị thay đổi khi user click vào nó :
    ```html
    <h1 onclick="this.innerHTML = 'Ooops!'">Click on this text!</h1>
    ```
    hoặc 
    ```html
    <h1 onclick="changeText(this)">Click on this text!</h1>
    <script>
    function changeText(id) {
      id.innerHTML = "Ooops!";
    }
    </script>
    ```
## **2) Thuộc tính event** 
- Để gán event vào phần tử HTML có thể sử dụng thuộc tính event .
- **VD :**
    ```html
    <button onclick="displayDate()">The time is?</button>
    <script>
    function displayDate() {
      document.getElementById("demo").innerHTML = Date();
    }
    </script>
    ```
## **3) Gán event sử dụng HTML DOM**
- **HTML DOM** cho phép gán event vào phần tử HTML sử dụng **JavaScript** :
- **VD :**
    ```html
    <button id="myBtn">Try it</button>
    <p id="demo"></p>
    <script>
    document.getElementById("myBtn").onclick = displayDate;
    function displayDate() {
      document.getElementById("demo").innerHTML = Date();
    }
    </script>
    ```
## **4) Event `onload` và `onunload`**
- Event `onload` và `onunload` khi user vào hoặc rời khỏi trang web .
- Event `onload` có thể được sử dụng để check loại trình duyệt hoặc phiên bản trình duyệt của người vào trang web, sau đó load chính xác phiên bản của trang web dựa vào các thông tin trên .
- Event `onload` và `onunload` có thể được sử dụng với cookies .
- **VD :**
    ```html
    <body onload="checkCookies()">
    <p id="demo"></p>
    <script>
    function checkCookies() {
      var text = "";
      if (navigator.cookieEnabled == true) {
        text = "Cookies are enabled.";
      } else {
        text = "Cookies are not enabled.";
      }
      document.getElementById("demo").innerHTML = text;
    }
    </script>
    ```
    => Kết quả : `Cookies are enabled.`
## **5) Event `onchange`**
- Event `onchange` thường được sử dụng kết hợp với việc validate các trường input .
- **VD :** Gọi hàm `upperCase()` mỗi khi user thay đổi nội dung trong trường input :
    ```html
    <input type="text" id="fname" onchange="upperCase()">
    ```
## **6) Các event khác**
- Event `onmouseover` và `onmouseout` có thể được sử dụng để thực thi function khi user di chuột qua hoặc di chuột ra khỏi phần tử của HTML .
- Event `onmousedown`, `onmouseup` và `onclick` là 3 hành động quen thuộc của việc click chuột .
    - khi ấn lì chuột vào phần tử = `onmousedown`
    - khi nhả chuột ra = `onmouseup`
    - khi click = `onclick`
- Event `onfocus` thường dùng để thay đổi background của trường input khi nó được focus

