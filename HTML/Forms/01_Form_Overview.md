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
### **2.4) 