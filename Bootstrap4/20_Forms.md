# Form
- Tất cả các phần tử liên quan đến text như `<input>` , `<textarea>`, và `<select>` với class "`.form-control`" có chiều rộng mặc định là `100%` trong **Bootstrap4** .
## **1) Form Layout**
- **Bootstrap4** cung cấp 2 loại layout :
    - **Stacked Form** ( full-width )
    - **Inline Form**
### **1.1) Stacked Form**
- **Stacked Form** có chiều dài các trường text input là `100%` .
- Tất cả các phần tử bên trong nó được gói trong class "`.form-group`"
- **VD :**
    ```html
    <form action="/action_page.php">
      <div class="form-group">
        <label for="email">Email address:</label>
        <input type="email" class="form-control" placeholder="Enter email" id="email">
      </div>
      <div class="form-group">
        <label for="pwd">Password:</label>
        <input type="password" class="form-control" placeholder="Enter password" id="pwd">
      </div>
      <div class="form-group form-check">
        <label class="form-check-label">
          <input class="form-check-input" type="checkbox"> Remember me
        </label>
      </div>
      <button type="submit" class="btn btn-primary">Submit</button>
    </form>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/jSD59bc.png>

### **1.2) Inline Form**
- Trong **Inline form**, tất cả các phần tử đứng trên cùng 1 dòng và được cân chỉnh sang trái .
    > Với màn hình nhỏ hơn `576px` , **inline form** sẽ lại được xếp xuống theo chiều dọc .
- Sử dụng class "`.form-inline`" để tạo **inline form** .
- **VD :**
    ```html
    <form class="form-inline" action="/action_page.php">
      <label for="email">Email address:</label>
      <input type="email" class="form-control" placeholder="Enter email" id="email">
      <label for="pwd">Password:</label>
      <input type="password" class="form-control" placeholder="Enter password" id="pwd">
      <div class="form-check">
        <label class="form-check-label">
          <input class="form-check-input" type="checkbox"> Remember me
        </label>
      </div>
      <button type="submit" class="btn btn-primary">Submit</button>
    </form>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/A7XEe6Y.png>

- Có thể sử dụng các tiện ích của **Bootstrap4** để giúp **inline form** dễ nhìn hơn :
    ```html
    <form class="form-inline" action="/action_page.php">
      <label for="email" class="mr-sm-2">Email address:</label>
      <input type="email" class="form-control mb-2 mr-sm-2" placeholder="Enter email" id="email">
      <label for="pwd" class="mr-sm-2">Password:</label>
      <input type="password" class="form-control mb-2 mr-sm-2" placeholder="Enter password" id="pwd">
      <div class="form-check mb-2 mr-sm-2">
        <label class="form-check-label">
        <input class="form-check-input" type="checkbox"> Remember me
        </label>
      </div>
      <button type="submit" class="btn btn-primary mb-2">Submit</button>
    </form>
    ```
    - Hiển thị trên trình duyệt :
        
        <img src=https://i.imgur.com/dtRNrcD.png>

## **2) Form Row/Grid**
- Có thể sử dụng class "`.col`" để kiểm soát chiều rộng và căn chỉnh cho form mà không cần dùng tiện ích `space` . Vẫn phải nhớ đặt chúng trong class "`.row`"
    ```html
    <form>
      <div class="row">
        <div class="col">
          <input type="text" class="form-control" id="email" placeholder="Enter email" name="email">
        </div>
        <div class="col">
          <input type="password" class="form-control" placeholder="Enter password" name="pswd">
        </div>
      </div>
    </form>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/CZBqb1R.png>

    - Nếu muốn khoảng cách giữa 2 trường input nhỏ lại, sử dụng class "`.form-row`" thay cho "`.row`" :

        <img src=https://i.imgur.com/sQvYDvI.png>

## **3) Form Validation**
- Có thể sử dụng các class check validation khác nhau để cung cấp các feedback cho user .
- Sử dụng class "`.was-validated`" hoặc "`.needs-validation`" cho phần tử `<form>` , tùy vào việc muốn feedback hiện ra trước hay sau khi user submit form .
- Trường input sẽ được hiển thị viền màu xanh (valid) hoặc viền màu đỏ (invalid) để chỉ ra những gì form còn thiếu .
- Có thể thêm class "`.valid-feedback`" hoặc "`.invalid-feedback`" để thêm thông báo cho user về những gì bị thiết , cần được thêm trước khi submit form .
- **VD1 :** Sử dụng class "`.was-validated`" :
    ```html
    <form action="/action_page.php" class="was-validated">
      <div class="form-group">
        <label for="uname">Username:</label>
        <input type="text" class="form-control" id="uname" placeholder="Enter username" name="uname" required>
        <div class="valid-feedback">Valid.</div>
        <div class="invalid-feedback">Please fill out this field.</div>
      </div>
      <div class="form-group">
        <label for="pwd">Password:</label>
        <input type="password" class="form-control" id="pwd" placeholder="Enter password" name="pswd" required>
        <div class="valid-feedback">Valid.</div>
        <div class="invalid-feedback">Please fill out this field.</div>
      </div>
      <div class="form-group form-check">
        <label class="form-check-label">
        <input class="form-check-input" type="checkbox" name="remember" required> I agree on blabla.
        <div class="valid-feedback">Valid.</div>
        <div class="invalid-feedback">Check this checkbox to continue.</div>
        </label>
      </div>
      <button type="submit" class="btn btn-primary">Submit</button>
    </form>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/5WFmSSP.png>

- **VD2 :** Sử dụng class "`.need-validation`" :
    [Tham khảo](https://www.w3schools.com/bootstrap4/tryit.asp?filename=trybs_form_validation_needs&stacked=h)



