# HTML Forms
## **1) Phần tử `<from>`**
- Phần tử `<form>` định nghĩa 1 form nhận input từ user .
- Cú pháp :
    ```html
    <form>
    .
    form elements
    .
    </form>
    ```
- Một form trong HTML chứa nhiều phần tử form .
- Phần tử form bao gồm nhiều loại phần tử input , như trường văn bản ( **text fields** ) , **checkbox** , **radio button** , **submit button** ,.....
## **2) Phần tử `<input>`**
- Phần tử `<input>` là phần tử form quan trọng nhất .
- Phần tử `<input>` có thể hiển thị theo nhiều cách , phụ thuộc vào các thuộc tính của nó .
### **2.1) Text input**
- Định nghĩa trường input 1 dòng để nhập text .
- Mặc định trường text input cho phép `20` ký tự .
- Cú pháp : 
    ```html
    <input type="text">
    ```
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

        <img src=https://i.imgur.com/LCEDWy3.png>

### **2.2) Radio Button input**
- Định nghĩa một radio button ( nút check hình tròn ) cho phép user chọn 1 trong các lựa chọn .
- Cú pháp :
    ```html
    <input type="radio">
    ```
- **VD :**
    ```html
    <form>
      <input type="radio" name="gender" value="male" checked> Male<br>
      <input type="radio" name="gender" value="female"> Female<br>
      <input type="radio" name="gender" value="other"> Other
    </form>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/2nn367V.png>

### **2.3) Submit Button input**
- Định nghĩa một nút để submit (duyệt) cho người dùng tự submit dữ liệu bằng tay .
- Cú pháp :
    ```html
    <input type="submit">
    ```
- Trình xử lý form sẽ là một trang với script xử lý dữ liệu đầu vào .
- Trình xử lý form được định nghĩa qua thuộc tính `action` :
    ```html
    <form action="/action_page.php">
      First name:<br>
      <input type="text" name="firstname" value="Mickey"><br>
      Last name:<br>
      <input type="text" name="lastname" value="Mouse"><br><br>
      <input type="submit" value="Submit">
    </form>
    ```
## **3) Thuộc tính `action`**
- Thuộc tính `action` định nghĩa sự việc sẽ xảy ra khi form được submit .
- Bình thường , dữ liệu form sẽ được gửi về trang web trên server khi user click vào nút `submit` .
- **VD :**
    ```html
    <form action="/action_page.php">
    ....
    </form>
    ```
## **4) Thuộc tính `target`**
- Thuộc tính `target` sẽ xác định kết quả sau khi submit sẽ được mở trong tab mới , mở trong một frame hay trong tab hiện tại .
- Giá trị mặc định của `target` là `_self` có nghĩa là kết quả submit sẽ ở tab hiện hành .
- Để đảm bảo form được mở ở tab mới , sử dụng giá trị `_blank` .
    ```html
    <form action="/action_page.php" target="_blank">
    ```
- Các giá trị khác là `_parent` và `_top` .
## **5) Thuộc tính `method`**
- Thuộc tính `method` chỉ ra phương thức HTTP ( `GET` hoặc `POST` ) sẽ được sử dụng khi dữ liệu được submit .
- **VD :**
    ```html
    <form action="/action_page.php" method="get">
    ```
    hoặc
    ```html
    <form action="/action_page.php" method="post">
    ```
### **5.1) `GET`**
- Phương thức mặc định được sử dụng khi submit là `GET` .
- Tuy nhiên , khi `GET` được sử dụng , dữ liệu form submit sẽ được nhìn thấy ở trên trang địa chỉ :
    ```
    /action_page.php?firstname=Mickey&lastname=Mouse
    ```
### **5.2) `POST`**
- Luôn sử dụng `POST` trong trường hợp form chứa dữ liệu nhạy cảm hoặc thông tin cá nhân ( như username, password, .....)
- Phương thức `POST` sẽ không hiển thị phần dữ liệu submit lên trang địa chỉ .
## **6) Thuộc tính `name`**
- Mỗi trường input bắt buộc phải có thuộc tính `name` khi submit .
- Nếu bỏ sót thuộc tính `name`, dữ liệu trong trường input sẽ không được gửi đi .
- **VD :**
    ```html
    <form action="/action_page.php">
      First name:<br>
      <input type="text" value="Mickey">
      <br>
      Last name:<br>
      <input type="text" name="lastname" value="Mouse">
      <br><br>
      <input type="submit" value="Submit">
    </form>
    ```
    => Trong trường hợp này , dữ liệu trong trường `First name` sẽ không được gửi đi .
## **7) Nhóm dữ liệu form trong `<fieldset>`**
- Phần tử `<fieldset>` được sử dụng để nhóm những dữ liệu liên quan đến nhau trong form .
- Phần tử `<legend>` định nghĩa caption cho phần tử `<fieldset>`
- **VD :**
    ```html
    <form action="/action_page.php">
      <fieldset>
        <legend>Personal information:</legend>
        First name:<br>
        <input type="text" name="firstname" value="Mickey">
        <br>
        Last name:<br>
        <input type="text" name="lastname" value="Mouse">
        <br><br>
        <input type="submit" value="Submit">
      </fieldset>
    </form>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/XiNbZ2D.png>




