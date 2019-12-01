# Các thuộc tính Input
## **1) Thuộc tính `value`**
- Thuộc tính `value` xác định giá trị khởi tạo của trường input (có sẵn khi load trang web)
- **VD :**
    ```html
    <form action="">
      First name:<br>
      <input type="text" name="firstname" value="John">
    </form>
    ```
    - Hiển thị trên trình duyệt :
        
        <img src=https://i.imgur.com/IrwjOKn.png>

## **2) Thuộc tính `readonly`**
- Thuộc tính `readonly` chỉ định trường input chỉ có thể đọc (không thể bị sửa đổi)
- **VD :**
    ```html
    <form action="">
      First name:<br>
      <input type="text" name="firstname" value="John" readonly>
    </form>
    ```
    - Hiển thị trên trình duyệt :
        
        <img src=https://i.imgur.com/zX0Snal.png>

## **3) Thuộc tính `disabled`**
- Thuộc tính disabled xác định trường input bị disable .
- Một trường input bị disable sẽ không thể sử dụng, không thể click, và giá trị của nó cũng không được gửi đi khi submit form .
- **VD :**
    ```html
    <form action="">
      First name:<br>
      <input type="text" name="firstname" value="John" disabled>
    </form>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/3VsmK8E.png>

## **4) Thuộc tính `size`**
- Thuộc tính `size` chỉ định số ký tự text có thể nhìn thấy trong trường input (có thể nói là chiều dài của ô input).
- **VD :**
    ```html
    <form action="">
      First name:<br>
      <input type="text" name="firstname" value="John" size="40">
    </form>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/Sr0KmXY.png>

## **5) Thuộc tính `maxlength`**
- Thuộc tính `maxlength` chỉ ra số ký tự tối đa được nhập trong trường input .
- Thuộc tính `maxlength` sẽ không đưa ra cảnh báo . Nếu muốn cảnh báo khi nhập quá số ký tự, phải viết cảnh báo bằng **JavaScript** .
- **VD :**
    ```html
    <form action="">
      First name:<br>
      <input type="text" name="firstname" maxlength="10">
    </form>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/dUvgg87.png>

## **6) Thuộc tính `autocomplete` (HTML5)**
- Thuộc tính `autocomplete` xác định form có được phép tự động điền bởi trình duyệt hay không .
- Khi bật `autocomplete`, trình duyệt sẽ tự động điền thông tin vào trường input ( VD : username, password,... ) dựa vào thông tin đã được nhập trước đo .
- Thuộc tính `autocomplete` hoạt động với form có các trường input sau : **text**, **search**, **url**, **tel**, **email**, **password**, **datepickers**, **range** , **color**,....
- Ở một số trình duyệt, cần kích hoạt chế độ tự động điền để sử dụng chức năng này .
- **VD :**
    ```html
    <form action="/action_page.php" autocomplete="on">
      First name:<input type="text" name="fname"><br>
      Last name: <input type="text" name="lname"><br>
      E-mail: <input type="email" name="email" autocomplete="off"><br>
      <input type="submit">
    </form>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/sBiTy4d.png>

## **7) Thuộc tính `novalidate` (HTML5)**
- Thuộc tính `novalidate` là một dạng thuộc tính `<form>` .
- Khi được gọi, `novalidate` sẽ xác định dữ liệu form sẽ không được validate (kiểm duyệt) khi submit .
- **VD :**
    ```html
    <form action="/action_page.php" novalidate>
      E-mail: <input type="email" name="user_email">
      <input type="submit">
    </form>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/2YVNLQz.png>

## **8) Thuộc tính `autofocus` (HTML5)**
- Thuộc tính `autofocus` chỉ ra rằng trường input sẽ được focus sau khi trang được load ( con trỏ chuột sẽ nháy ở trường input )
- **VD :**
    ```html
    First name:<input type="text" name="fname" autofocus>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/r7X0tmi.png>

## **9) Thuộc tính `form` (HTML5)**
- Thuộc tính `form` chỉ xác định cho phần tử `<input>` có thể thuộc 1 hoặc nhiều form khác nhau .
- **VD :**
    ```html
    <form action="/action_page.php" id="form1">
      First name: <input type="text" name="fname"><br>
      <input type="submit" value="Submit">
    </form>

    Last name: <input type="text" name="lname" form="form1">
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/OXPSuvU.png>

## **10) Thuộc tính `formaction` (HTML5)**
- Thuộc tính `formaction` chỉ ra đường dẫn URL của file sẽ xử lý luồng input sau khi form được submit .
- Thuộc tính `formaction` sẽ ghi đè lên thuộc tính `action` nếu có khai báo trên phần tử `<form>` .
- Thuộc tính `formaction` được sử dụng với `type="submit"` và `type="image"` .
- **VD :**
    ```html
    <form action="/action_page.php">
      First name: <input type="text" name="fname"><br>
      Last name: <input type="text" name="lname"><br>
      <input type="submit" value="Submit"><br>
      <input type="submit" formaction="/action_page2.php"
      value="Submit as admin">
    </form>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/oBle6hs.png>

## **11) Thuộc tính `formenctype` (HTML5)**
- Thuộc tính `formenctype` chỉ ra cách mà dữ liệu form được mã hóa sau khi submit (chỉ sử dụng cho form có `method="post"`) .
- Thuộc tính `formenctype` sẽ ghi đè thuộc tính `enctype` nếu có khai báo trên phần tử `<form>` .
- Thuộc tính `formenctype` được sử dụng với `type="submit"` và `type="image"` .
- **VD :**
    ```html
    <form action="/action_page_binary.asp" method="post">
      First name: <input type="text" name="fname"><br>
      <input type="submit" value="Submit">
      <input type="submit" formenctype="multipart/form-data"
      value="Submit as Multipart/form-data">
    </form>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/cvD2GLO.png>

## **12) Thuộc tính `formmethod` (HTML5)**
- Thuộc tính `formmethod` định nghĩa phương thức HTTP được sử dụng để gửi data đến trình xử lý form (`action`)
- Thuộc tính `formmethod` sẽ ghi đề lên thuộc tính `method` của phần tử `<form>` nếu được khai báo .
- Thuộc tính `formmethod` được sử dụng với `type="submit"` và `type="image"` .
- **VD :**
    ```html
    <form action="/action_page.php" method="get">
      First name: <input type="text" name="fname"><br>
      Last name: <input type="text" name="lname"><br>
      <input type="submit" value="Submit">
      <input type="submit" formmethod="post" value="Submit using POST">
    </form>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/LSpDF7a.png>

## **13) Thuộc tính `formnovalidate` (HTML5)**
- Thuộc tính `formnovalidate` sẽ ghi đè lên thuộc tính `novalidate` của phần tử `<form>` nếu được khai báo .
- Thuộc tính `formnovalidate` đuuợc sử dụng với `type="submit"` .
- **VD :**
    ```html
    <form action="/action_page.php">
      E-mail: <input type="email" name="userid"><br>
      <input type="submit" value="Submit"><br>
      <input type="submit" formnovalidate value="Submit without validation">
    </form>
    ```
    - Hiển thị trên trình duyệt :
        
        <img src=https://i.imgur.com/CUyyzPk.png>

## **14) Thuộc tính `formtarget` (HTML5)**
- Thuộc tính `formtarget` chỉ ra tên hoặc keyword về nơi mà kết quả trả về sau khi submit được hiển thị (mở trong tab mới, mở trong tab hiện tại,...)
- Thuộc tính `formtarget` sẽ ghi đè lên thuộc tính `target` nếu được khai báo ở phần tử `<form>`
- Thuộc tính `formtarget` được sử dụng với `type="submit"` và `type="image"` .
- **VD :**
    ```html
    <form action="/action_page.php">
      First name: <input type="text" name="fname"><br>
      Last name: <input type="text" name="lname"><br>
      <input type="submit" value="Submit as normal">
      <input type="submit" formtarget="_blank"
      value="Submit to a new window">
    </form>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/65PBCuT.png>

## **15) Thuộc tính `height` và `width` (HTML5)**
- Thuộc tính `height` và `width` chỉ ra chiều cao và chiều rộng của phần tử `<input type="image">` .
- Luôn luôn chỉ định kích thước của hình ảnh trong thuộc tính `type`
- **VD :**
    ```html
    <input type="image" src="img_submit.gif" alt="Submit" width="48" height="48">
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/LNnedYT.png>

## **16) Thuộc tính `list` (HTML5)**
- Thuộc tính `list` liên quan tới phần tử `<datalist>` chứa các option đã được định nghĩa trước cho phần tử `<input>`
- **VD :**
    ```html
    <input list="browsers">

    <datalist id="browsers">
      <option value="Internet Explorer">
      <option value="Firefox">
      <option value="Chrome">
      <option value="Opera">
      <option value="Safari">
    </datalist>
    ```
    - Hiển thị trong trình duyệt :

        <img src=https://i.imgur.com/f1gdR9z.png>

## **17) Thuộc tính `min` và `max` (HTML5)**
- Thuộc tính `min` và `max` giới hạn giá trị nhỏ nhất và lớn nhất có thể nhập vào trường input .
- Thuộc tính `min` và `max` hoạt động với các kiểu input sau : **number**, **range**, **date**, **datetime-local**, **month**, **time** và **week** .
- **VD :**
    ```html
    Enter a date before 1980-01-01:
    <input type="date" name="bday" max="1979-12-31">

    Enter a date after 2000-01-01:
    <input type="date" name="bday" min="2000-01-02">

    Quantity (between 1 and 5):
    <input type="number" name="quantity" min="1" max="5">
    ```
    - Hiển thị trên trình duyệt:

        <img src=https://i.imgur.com/0namprq.png>

## **18) Thuộc tính `multiple` (HTML5)**
- Thuộc tính `multiple` xác định user được cho phép nhập nhiều hơn 1 giá trị vào trường input .
- Thuộc tính `multiple` là việc với các kiểu input sau : **email**, **file** .
- **VD :**
    ```html
    Select images: <input type="file" name="img" multiple>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/wn3yIMS.png>
## **19) Thuộc tính `pattern` (HTML5)**
- Thuộc tính `pattern` sẽ chỉ ra cấu trúc định dạng (format) của input và sẽ check lại sau khi người dùng nhập input . Nếu sai format , sẽ xuất hiện cảnh báo vào người dùng phải nhập lại .
- Thuộc tính `pattern` làm việc với các kiểu input sau : **text**, **search**, **url**, **tel**, **email**, **password** .
- **VD :**
    ```html
    Country code: <input type="text" name="country_code" pattern="[A-Za-z]{3}" title="Three letter country code">
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/n2scYBe.png>

## **20) Thuộc tính `placeholder` (HTML5)**
- Thuộc tính `placeholder` đưa ra gợi ý mô tả về input mong muốn trong trường input (cũng có thể là 1 gợi ý về format) .
- Gợi ý sẽ được hiển thị trên trường input trước khi user bắt đầu nhập dữ liệu .
- Thuộc tính `placeholder` làm việc với các kiểu input sau : **text**, **search**, **url**, **tel**, **email**, **password** .
- **VD :**
    ```html
    <form action="/action_page.php">
      <input type="text" name="fname" placeholder="First name"><br>
      <input type="text" name="lname" placeholder="Last name"><br>
      <input type="submit" value="Submit">
    </form>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/OgDSj3d.png>

## **21) Thuộc tính `required` (HTML5)**
- Thuộc tính `required` yêu cầu trường input phải được điền dữ liệu (không được để trống trước khi submit) . Nếu để trống trường input khi submit sẽ xuất hiện cảnh báo .
- Thuộc tính `required` làm việc trên các kiểu input sau : **text**, **search**, **url**, **tel**, **email**, **password**, **date picker**, **number**, **checkbox**, **radio** và **file** .
- **VD :**
    ```html
    Username: <input type="text" name="usrname" required>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/hvPwSla.png>

## **22) Thuộc tính `step` (HTML5)**
- Thuộc tính `step` chỉ ra các khoảng số nhập vào cho phần tử `<input>` . VD : nếu `step = 3` , các con số là `-3`, `0`, `3`, `6`, ...
- Thuộc tính `step` làm việc với các kiểu input sau : **number** , **range** , **date**, **datetime-local**, **month**, **time** và **week** .
- **VD :**
    ```html
    <input type="number" name="points" step="3">
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/bLKeOVB.png>
