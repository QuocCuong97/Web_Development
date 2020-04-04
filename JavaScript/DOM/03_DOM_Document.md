# DOM Document
- **HTML DOM Document object** đại diện cho trang web, là chủ sở hữu của các đối tượng khác trong trang web .
- Trước khi muốn truy cập các phần tử của trang HTML, phải truy cập vào **document object** .
## **1) Tìm phần tử HTML**

| Phương thức | Mô tả |
|-------------|-------|
| `document.getElementById(`*`id`*`)` | Tìm phần tử bằng `id` của phần tử |
| `document.getElementsByTagName(`*`name`*`)` | Tìm phần tử bằng tên `tag` |
| `document.getElementsByClassName(`*`name`*`)` | Tìm phần tử bằng tên `class` |

- **VD1 :** Tìm phần tử có `id="intro"` :
    ```html
    <p id="intro">Hello World!</p>
    <p id="demo"></p>
    <script>
    var myElement = document.getElementById("intro");
    document.getElementById("demo").innerHTML = 
    "The text from the intro paragraph is " + myElement.innerHTML;
    </script>
    ```
    => Kết quả : `The text from the intro paragraph is Hello World!`
- **VD2 :** Tìm tất cả các phần tử `<p>` :
    ```html
    <p>Hello World!</p>
    <p id="demo"></p>
    <script>
    var x = document.getElementsByTagName("p");
    document.getElementById("demo").innerHTML = 
    'The text in first paragraph (index 0) is: ' + x[0].innerHTML;
    </script>
    ```
    => Kết quả : `The text in first paragraph (index 0) is: Hello World!`
- **VD3 :** Tìm phần tử có `id="main"`, sau đó tìm tất cả các phần tử `<p>` trong `"main"` :
    ```html
    <div id="main">
      <p>The DOM is very useful.</p>
    </div>
    <p id="demo"></p>
    <script>
    var x = document.getElementById("main");
    var y = x.getElementsByTagName("p");
    document.getElementById("demo").innerHTML = 
    'The first paragraph (index 0) inside "main" is: ' + y[0].innerHTML;
    </script>
    ```
    => Kết quả : `The first paragraph (index 0) inside "main" is: The DOM is very useful.`
- **VD4 :** Tìm tất cả các phần tử có `class="intro"` :
    ```html
    <p class="intro">The DOM is very useful.</p>
    <p class="intro">This example demonstrates the <b>getElementsByClassName</b> method.</p>
    <p id="demo"></p>
    <script>
    var x = document.getElementsByClassName("intro");
    document.getElementById("demo").innerHTML = 
    'The first paragraph (index 0) with class="intro": ' + x[0].innerHTML;
    </script>
    ```
    => Kết quả : `The first paragraph (index 0) with class="intro": The DOM is very useful.`
- **VD5 :** Tìm kiếm các thẻ `<p>` có `class="intro"` :
    ```js
    var x = document.querySelectorAll("p.intro");
    ```
- **VD6 :** Tìm kiếm tất cả các phần tử trong form, liệt kê giá trị của các trường :
    ```html
    <form id="frm1" action="/action_page.php">
      First name: <input type="text" name="fname"><br>
      Last name: <input type="text" name="lname"><br><br>
      <input type="submit">
    </form> 
    <p>Click "Try it" to display the value of each element in the form.</p>
    <button onclick="myFunction()">Try it</button>
    <p id="demo"></p>
    <script>
    function myFunction() {
      var x = document.forms["frm1"];
      var text = "";
      var i;
      for (i = 0; i < x.length ;i++) {
        text += x.elements[i].value + "<br>";
      }
      document.getElementById("demo").innerHTML = text;
    }
    </script>
    ```
    <img src=https://i.imgur.com/HVe7yYG.png>

## **2) Thay đổi phần tử HTML**

| Thuộc tính | Mô tả |
|------------|-------|
| *`element`*`.innerHTML` = *`new html content`* | Thay đổi phần nội dung HTML bên trong phần tử |
| *`element`*`.attribute` = *`new value`* | Thay đổi giá trị thuộc tính của phần tử HTML |
| *`element`*`.style.property` = *`new style`* | Thay đổi style CSS của phần tử HTML |

| Phương thức | Mô tả |
|-------------|-------|
| *`element`*`.setAttribute`*`(attribute, value)`* | Thay đổi giá trị thuộc tính của phần tử HTML | 
- **VD1 :** Thay đổi phần nội dung HTML bên trong phần tử :
    ```html
    <p id="p1">Hello World!</p>
    <script>
    document.getElementById("p1").innerHTML = "New text!";
    </script>
    ```
    => Kết quả : `New text!`
- **VD2 :** Thay đổi giá trị thuộc tính của phần tử HTML :
    ```html
    <img id="myImage" src="smiley.gif">
    <script>
    document.getElementById("myImage").src = "landscape.jpg";
    </script>
    ```
- **VD3 :** Thay đổi style CSS của phần tử HTML :
    ```html
    <h1 id="id1">My Heading 1</h1>
    <button type="button"
    onclick="document.getElementById('id1').style.color = 'red'">
    Click Me!</button>
    ```
## **3) Thêm và xóa phần tử**

| Phương thức | Mô tả |
|------------|-------|
| `document.createElement(`*`element`*`)` | Tạo một phần tử HTML |
| `document.removeChild(`*`element`*`)` | Xóa một phần tử HTML |
| `document.appendChild(`*`element`*`)` | Thêm một phần tử HTML |
| `document.replaceChild(`*`new, old`*`)` | Thay thế một phần tử HTML |
| `document.write(`*`text`*`)` | Thay đổi HTML Output Stream |
- **VD1 :** Thay đổi HTML Output Stream  :
    ```html
    <script>
    document.write(Date());
    </script>
    ```
    => Kết quả : `Sat Apr 04 2020 23:38:49 GMT+0700 (Indochina Time)`
## **4) Thêm trình điều khiển Event ( *event handlers* )**

| Phương thức | Mô tả |
|------------|-------|
| `document.getElementById(`*`id`*`).onclick = function(){code}` | Thêm trình xử lý event vào một event `onclick` |

## **5) Tìm các HTML object**
| Thuộc tính | Mô tả |
|------------|-------|
| `document.anchors` | Trả về tất cả các phần tử `<a>` có thuộc tính `name` |
| `document.applets` | Trả về các phần tử `<applet>` |
| `document.baseURI` | Trả về URI tuyệt đối của document |
| `document.body` | Trả về phần tử `<body>` |
| `document.cookie` | Trả về cookie của trang |
| `document.doctype` | Trả về doctype của trang |
| `document.documentElement` | Trả về phần tử `<html>` |
| `document.documentMode` | Trả về mode được sử dụng bởi trình duyệt |
| `document.documentURI` | Trả về URI của document|
| `document.domain` | Trả về domain name của server |
| `document.embeds` | Trả về tất cả các phần tử `<embed>` |
| `document.forms` | Trả về tất cả các phần tử `<form>` |
| `document.head` | Trả về phần tử `<head>` |
| `document.images` | Trả về tất cả các phần tử `<img>` |
| `document.inputEncoding` | |
| `document.lastModified` | |
| `document.links` | Trả về tất cả các phần tử `<area>` và phần tử `<a>` có thuộc tính `href` |
| `document.readyState` | |
| `document.referrer` | |
| `document.strictErrorChecking` | |
| `document.scripts` | Trả về tất cả các phần tử `script` |
| `document.title` | Trả về phần tử `<title>` |
| `document.URL` | Trả về đường dẫn hoàn chỉnh của document |
