# Navigation
## **1) Basic Navigation**
### **1.1) Nav Menu**
- Để tạo một menu ngang đơn giản , thêm class "`.nav`" vào phần tử `<ul>` , theo sau là các class "`.nav-item`" cho mỗi phần tử `<li>` bên trong và class "`.nav-link`" cho link của chúng .
    ```html
    <ul class="nav">
      <li class="nav-item">
        <a class="nav-link" href="#">Link</a>
      </li>
      <li class="nav-item">
        <a class="nav-link" href="#">Link</a>
      </li>
      <li class="nav-item">
        <a class="nav-link" href="#">Link</a>
      </li>
      <li class="nav-item">
        <a class="nav-link disabled" href="#">Disabled</a>
      </li>
    </ul>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/QUwUf2J.png>

### **1.2) Aligned Nav**
- Có thể sử dụng các tiện ích căn chỉnh của **Bootstrap4** để căn chỉnh cho **nav** :
    - Mặc định : căn chỉnh trái
    - Class "`.justify-content-center`" : căn chỉnh giữa
    - Class " `.justify-content-end`" : căn chỉnh phải
- **VD :**
    ```html
    <!-- Centered nav -->
    <ul class="nav justify-content-center">

    <!-- Right-aligned nav -->
    <ul class="nav justify-content-end">
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/mCxxmyJ.png>
### **1.3) Vertical Nav**
- Sử dụng thêm class "`.flex-column`" để tạo một **nav** theo hướng dọc :
    ```html
    <ul class="nav flex-column">
      <li class="nav-item">
        <a class="nav-link" href="#">Link</a>
      </li>
      <li class="nav-item">
        <a class="nav-link" href="#">Link</a>
      </li>
      <li class="nav-item">
        <a class="nav-link" href="#">Link</a>
      </li>
      <li class="nav-item">
        <a class="nav-link disabled" href="#">Disabled</a>
      </li>
    </ul>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/hkK8v6M.png>