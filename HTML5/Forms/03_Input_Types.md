# Các kiểu input trong HTML
## **1) Text Input**
- Cú pháp :
    ```html
    <input type="text">
    ```
- Công dụng : định nghĩa trường input 1 dòng
- **VD :**
    ```html
    <form>
      First name:<br>
      <input type="text" name="firstname"><br>
      Last name:<br>
      <input type="text" name="lastname">
    </form>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/SNhg7T8.png>

## **2) Password Input**
- Cú pháp :
    ```html
    <input type="password">
    ```
- Công dụng : định nghĩa trường nhập password
- Password sau khi nhập sẽ được che lại dưới dạng hình <code>&ast;</code> hoặc hình <code>&#9679;</code>
- **VD :**
    ```html
    <form>
      User name:<br>
      <input type="text" name="username"><br>
      User password:<br>
      <input type="password" name="psw">
    </form>
    ```
    - Hiển thị trên trình duyệt :
        
        <img src=https://i.imgur.com/hBECZ2F.png>

## **3) Submit Input**
- Cú pháp :
    ```html
    <input type="submit">
    ```
- Công dụng : định nghĩa 1 nút submit ( duyệt ) dữ liệu để đưa đến trình xử lý form .
- Trình xử lý là các đoạn code sẽ sử lý dữ liệu input sau khi submit .
- Trình xử lý form được chỉ ra ở thuộc tính `action` của thẻ form :
    ```html
    <form action="/action_page.php">
      First name:<br>
      <input type="text" name="firstname" value="Mickey"><br>
      Last name:<br>
      <input type="text" name="lastname" value="Mouse"><br><br>
      <input type="submit" value="Submit">
    </form>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/niJKwUz.png>

## **4) Reset Input**
- Cú pháp :
    ```html
    <input type="reset">
    ```
- Công dụng : định nghĩa 1 nút reset sẽ reset toàn bộ dữ liệu form thành giá trị mặc định .
- **VD :**
    ```html
    <form action="/action_page.php">
      First name:<br>
      <input type="text" name="firstname" value="Mickey"><br>
      Last name:<br>
      <input type="text" name="lastname" value="Mouse"><br><br>
      <input type="submit" value="Submit">
      <input type="reset">
    </form>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/BVuUFn4.png>

## **5) Radio Input**
- Cú pháp :
    ```html
    <input type="radio">
    ```
- Công dụng : định nghĩa một nút radio button <code>&#128280;</code>
- **VD :**
    ```html
    <form>
      <input type="radio" name="gender" value="male" checked> Male<br>
      <input type="radio" name="gender" value="female"> Female<br>
      <input type="radio" name="gender" value="other"> Other
    </form>
    ```
    - Hiển thị trên trình duyệt :
        
        <img src=https://i.imgur.com/gxMKfYu.png>

## **6) Checkbox Input**
- Cú pháp :
    ```html
    <input type="checkbox">
    ```
- Công dụng : định nghĩa 1 checkbox
- **VD :**
    ```html
    <form>
      <input type="checkbox" name="vehicle1" value="Bike"> I have a bike<br>
      <input type="checkbox" name="vehicle2" value="Car"> I have a car
    </form>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/kaPpoIt.png>

## **7) Button Input**
- Cú pháp :
    ```html
    <input type="button">
    ```
- Công dụng : định nghĩa 1 nút click
- **VD :**
    ```html
    <input type="button" onclick="alert('Hello World!')" value="Click Me!">
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/fzkjbu3.png>

## **8) Color Input (HTML5)**
- Cú pháp :
    ```html
    <input type="color">
    ```
- Công dụng : sử dụng cho trường input có thể chứa đựng màu sắc . 
- Tùy vào trình duyệt hỗ trợ, một bảng color picker sẽ hiện lên để chọn màu khi click vào button .
- **VD :**
    ```html
    <form>
      Select your favorite color:
      <input type="color" name="favcolor" value="#ff0000">
      <input type="submit">
    </form>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/r5AFUnK.png>

## **9) Date Input (HTML5)**
> Không được **Safari** hỗ trợ .
- Cú pháp :
    ```html
    <input type="date">
    ```
- Công dụng : sử dụng cho trường input có thể chứa đựng ngày tháng .
- Tùy vào trình duyệt hỗ trợ, một bảng date picker sẽ hiện lên để chọn ngày khi click vào button .
- **VD :**
    ```html
    <form>
      Birthday:
      <input type="date" name="bday">
      <input type="submit>
    </form>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/Y6Fole5.png>

- Có thể sử dụng thuộc tính `min` và `max` để giới hạn giá trị ngày tháng nhập vào :
    ```html
    <form>
      Enter a date before 1980-01-01:
      <input type="date" name="bday" max="1979-12-31"><br>
      Enter a date after 2000-01-01:
      <input type="date" name="bday" min="2000-01-02"><br>
    </form>
    ```
## **10) Datetime-Local Input (HTML5)**
> Không được **Mozilla Firefox** , **Safari** hỗ trợ .
- Cú pháp :
    ```html
    <input type="datetime-local">
    ```
- Công dụng : sử dụng để nhập ngày tháng năm và giờ phút vào trường input, không có time zone .
- Tùy vào trình duyệt hỗ trợ, một bảng date picker sẽ hiện lên để chọn ngày khi click vào button .
- **VD :**
    ```html
    <form action="/action_page.php">
      Birthday (date and time):
      <input type="datetime-local" name="bdaytime">
      <input type="submit" value="Send">
    </form>
    ```
    - Hiển thị trên trình duyệt :
        
        <img src=https://i.imgur.com/zQxw9mB.png>

## **11) Email Input (HTML5)**
- Cú pháp :
    ```html
    <input type="email">
    ```
- Công dụng : sử dụng cho trường input có thể chứa đựng địa chỉ email .
- Tùy vào trình duyệt hỗ trợ, địa chỉ email có thể được validate khi được submit .
- Một số trình duyệt điện thoại nhận dạng được email input, và thêm nút `.com` vào bàn phím cảm ứng để tiện cho việc nhập email .
- **VD :**
    ```html
    <form>
      E-mail:
      <input type="email" name="email">
    </form>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/htqrd0e.png>

## **12) File Input (HTML5)**
- Cú pháp :
    ```html
    <input type="file">
    ```
- Công dụng : định nghĩa một trường cho phép chọn file và một nút "Browse" để upload file .
- **VD :**
    ```html
    <form action="/action_page.php">
      Select a file: <input type="file" name="myFile"><br><br>
      <input type="submit">
    </form>
    ```
    - Hiển thị trên trình duyệt :
        
        <img src=https://i.imgur.com/jULCLvZ.png>

## **13) Month Input (HTML5)**
> Không được **Mozilla Firefox** , **Safari** hỗ trợ .
- Cú pháp :
    ```html
    <input type="month">
    ```
- Công dụng : cho phép user chọn tháng và năm .
- Tùy vào trình duyệt hỗ trợ, một bảng date picker sẽ hiện lên để chọn ngày khi click vào button .
- **VD :**
    ```html
    <form>
      Birthday (month and year):
      <input type="month" name="bdaymonth">
      <input type="submit">
    </form>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/7apLQC0.png>

## **14) Number Input (HTML5)**
- Cú pháp :
    ```html
    <input type="number">
    ```
- Công dụng : định nghĩa trường input chỉ cho phép nhập số .
- Có thể giới hạn số cho phép bằng thuộc tính `min` và `max` .
- **VD :**
    ```html
    <form>
      Quantity (between 1 and 5):
      <input type="number" name="quantity" min="1" max="5">
      <input type="submit>
    </form>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/0xk56EF.png>

## **15) Range Input (HTML5)**
- Cú pháp :
    ```html
    <input type="range">
    ```
- [Tham khảo thêm](https://www.w3schools.com/html/html_form_input_types.asp)
## **16) Search Input (HTML5)**
- Cú pháp :
    ```html
    <input type="search">
    ```
- Công dụng : sử dụng cho trường search ( tương tư như trường text )
- **VD :**
    ```html
    <form>
      Search Google:
      <input type="search" name="googlesearch">
      <input type="submit">
    </form>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/yY69bAS.png>

## **17) Tel Input (HTML5)**
- Cú pháp :
    ```html
    <input type="tel">
    ```
- Công dụng : sử dụng cho trường input dùng để nhập số điện thoại .
- **VD :**
    ```html
    <form>
      Telephone:
      <input type="tel" name="phone" pattern="[0-9]{3}-[0-9]{2}-[0-9]{3}" required>
      <input type="submit">
      <span>Format: 123-45-678</span>
    </form>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/5fKGK19.png>

## **18) Time Input (HTML5)**
> Không được **Safari** hỗ trợ .
- Cú pháp :
    ```html
    <input type="time">
    ```
- Công dụng : cho phép user chọn thời gian ( không có time zone )
- Tùy vào trình duyệt hỗ trợ, một bảng date picker sẽ hiện lên để chọn ngày khi click vào button .
- **VD :**
    ```html
    <form action="/action_page.php">
      Select a time:
      <input type="time" name="usr_time">
      <input type="submit">
    </form>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/kxq0r81.png>

## **19) URL Input (HTML5)**
- Cú pháp :
    ```html
    <input type="url">
    ```
- Công dụng : sử dụng cho trường input có thể chứa địa chỉ URL .
- Tùy vào trình duyệt hỗ trợ, trường URL có thể tự động được validated khi được submit .
- Một số trình duyệt điệnt thoại nhận dạng được URL input, và thêm nút `.com` vào bàn phím cảm ứng để tiện cho việc nhập URL .
- **VD :**
    ```html
    <form action="/action_page.php">
      Add your homepage:
      <input type="url" name="homepage">
      <input type="submit">
    </form>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/s2F7cSA.png>

## **20) Week Input (HTML5)**
> Không được **Mozilla Firefox** , **Safari** hỗ trợ .
- Cú pháp :
    ```html
    <input type="week">
    ```
- Công dụng : cho phép người dùng nhập tuần và năm .
- Tùy vào trình duyệt hỗ trợ, một bảng date picker sẽ hiện lên để chọn ngày khi click vào button .
- **VD :**
    ```html
    <form action="/action_page.php">
      Select a week:
      <input type="week" name="year_week">
      <input type="submit">
    </form>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/2nf1FCF.png>


