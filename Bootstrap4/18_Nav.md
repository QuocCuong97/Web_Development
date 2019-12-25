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
### **1.4) Tabs**
- Biến đổi **nav-menu** thành các tab điều hướng với class "`.nav-tabs`" .
- Thêm class "`.active` cho link hiện hành . 
- **VD :**  
    ```html
    <ul class="nav nav-tabs">
      <li class="nav-item">
        <a class="nav-link active" href="#">Active</a>
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

        <img src=https://i.imgur.com/JNi1MGN.png>

### **1.5) Pills**
- Biến đổi **nav-menu** thành các nút điều hướng với class "`.nav-pills`" .
- Thêm class "`.active` cho link hiện hành .
- **VD :**
    ```html
    <ul class="nav nav-pills">
      <li class="nav-item">
        <a class="nav-link active" href="#">Active</a>
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

        <img src=https://i.imgur.com/BHJNIhc.png>

### **1.6) Căn chỉnh giữa Tab/Pills**
- Căn chỉnh giữa cho các tab/pill bằng class "`.nav-justified`"
- **VD :**
    ```html
    <ul class="nav nav-pills nav-justified">..</ul>
    <ul class="nav nav-tabs nav-justified">..</ul>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/sVwofyM.png>
### **1.7) Pills kết hợp Dropdown**
- **VD :**
    ```html
    <ul class="nav nav-pills">
      <li class="nav-item">
        <a class="nav-link active" href="#">Active</a>
      </li>
      <li class="nav-item dropdown">
        <a class="nav-link dropdown-toggle" data-toggle="dropdown" href="#">Dropdown</a>
        <div class="dropdown-menu">
          <a class="dropdown-item" href="#">Link 1</a>
          <a class="dropdown-item" href="#">Link 2</a>
          <a class="dropdown-item" href="#">Link 3</a>
        </div>
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

        <img src=https://i.imgur.com/xG3NUoq.png>
### **1.8) Tabs kết hợp Dropdown**
- **VD :**
    ```html
    <ul class="nav nav-tabs">
      <li class="nav-item">
        <a class="nav-link active" href="#">Active</a>
      </li>
      <li class="nav-item dropdown">
        <a class="nav-link dropdown-toggle" data-toggle="dropdown" href="#">Dropdown</a>
        <div class="dropdown-menu">
          <a class="dropdown-item" href="#">Link 1</a>
          <a class="dropdown-item" href="#">Link 2</a>
          <a class="dropdown-item" href="#">Link 3</a>
        </div>
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

        <img src=https://i.imgur.com/2ZMhmda.png>
### **1.9) Dynamic Tabs**
- Để tạo các tab động, thêm thuộc tính `data-toggle="tab"` vào mỗi link . Sau đó thêm class "`.tab-pane`" gắn với ID duy nhất của mỗi tab và gói chúng trong phần tử `<div>` với class là "`.tab-content`" .
- Nếu muốn tab fade-in/out khi click vào chúng , thêm class "`.fade`" vào cạnh class "`.tab-pane`"
- **VD :**
    ```html
    <!-- Nav tabs -->
    <ul class="nav nav-tabs">
      <li class="nav-item">
        <a class="nav-link active" data-toggle="tab" href="#home">Home</a>
      </li>
      <li class="nav-item">
        <a class="nav-link" data-toggle="tab" href="#menu1">Menu 1</a>
      </li>
      <li class="nav-item">
        <a class="nav-link" data-toggle="tab" href="#menu2">Menu 2</a>
      </li>
    </ul>

    <!-- Tab panes -->
    <div class="tab-content">
      <div class="tab-pane container active" id="home">...</div>
      <div class="tab-pane container fade" id="menu1">...</div>
      <div class="tab-pane container fade" id="menu2">...</div>
    </div>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/oOo6Nr0.png>

### **1.10) Dynamic Pills**
- Áp dụng tương tự code với **pill** để tạo **pill** động , chr thay giá trị thuộc tính `data-toggle` thành `data-toggle="pill"` .
- **VD :**
    ```html
    <!-- Nav pills -->
    <ul class="nav nav-pills">
      <li class="nav-item">
        <a class="nav-link active" data-toggle="pill" href="#home">Home</a>
      </li>
      <li class="nav-item">
        <a class="nav-link" data-toggle="pill" href="#menu1">Menu 1</a>
      </li>
      <li class="nav-item">
        <a class="nav-link" data-toggle="pill" href="#menu2">Menu 2</a>
      </li>
    </ul>

    <!-- Tab panes -->
    <div class="tab-content">
      <div class="tab-pane container active" id="home">...</div>
      <div class="tab-pane container fade" id="menu1">...</div>
      <div class="tab-pane container fade" id="menu2">...</div>
    </div>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/pSEli4e.png>

## **2) Navigation Bar**
### **2.1) Cơ bản về Navigation Bar**
- **Navigation bar** - thanh điều hướng là một thanh header được đặt trên đầu trang web :

    <img src=https://i.imgur.com/Dq4OgJh.png>
- Với **Bootstrap**, **navigation bar** có thể tự mở rộng hoặc thu gọn lại tùy thuộc vào kích cỡ màn hình .
- Một **navigation bar** tiêu chuẩn được tạo ra bằng class "`.navbar`" , theo sau là các class thuộc kiểu responsive : "`.navbar-expand-xl|lg|md|sm`" ( chồng các navbar theo chiều dọc )
- Để thêm link vào trong **navbar** , sử dụng phần tử `<ul>` với `class="navbar-nav"` . Sau đó thêm vào các phần tử `<li>` class "`.nav-item`" theo sau bởi phần tử `<a>` với class "`.nav-link`"
- **VD :**
    ```html
    <!-- A grey horizontal navbar that becomes vertical on small screens -->
    <nav class="navbar navbar-expand-sm bg-light">

      <!-- Links -->
      <ul class="navbar-nav">
        <li class="nav-item">
          <a class="nav-link" href="#">Link 1</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">Link 2</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">Link 3</a>
        </li>
      </ul>

    </nav>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/8uqQLYB.png>

  