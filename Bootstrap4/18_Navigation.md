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

### **2.2) Vertical Navbar**
- Bỏ đi các class "`.navbar-expand-xl|lg|md|sm`" để tạo một **navigation bar** theo hướng dọc :
    ```html
    <!-- A vertical navbar -->
    <nav class="navbar bg-light">

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

        <img src=https://i.imgur.com/sttEusg.png>
### **2.3) Căn chỉnh giữa cho Navbar**
- Thêm class "`.justify-content-center`" để căn chỉnh giữa cho **navigation bar** .
- **VD :**
    ```html
    <nav class="navbar navbar-expand-sm bg-light justify-content-center">
      ...
    </nav>
    ```
    - Hiển thị trên trình duyệt :
        
        <img src=https://i.imgur.com/l4zIEDD.png>
### **2.4) Colored Navbar**
- Sử dụng bất kì class "`.bg-color`" nào để thay đổi màu background của **navbar** ( "`.bg-primary`", "`.bg-success`", "`.bg-info`", "`.bg-warning`", "`.bg-danger`", "`.bg-dark`", "`.bg-light`" )
> Nên sử dụng chữ màu trắng cho class "`navbar-dark`" hoặc chữ màu đen cho class "`navbar-light`"
- **VD :**
    ```html
    <!-- Grey with black text -->
    <nav class="navbar navbar-expand-sm bg-light navbar-light">
      <ul class="navbar-nav">
        <li class="nav-item active">
          <a class="nav-link" href="#">Active</a>
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
    </nav>

    <!-- Black with white text -->
    <nav class="navbar navbar-expand-sm bg-dark navbar-dark">...</nav>

    <!-- Blue with white text -->
    <nav class="navbar navbar-expand-sm bg-primary navbar-dark">...</nav>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/WJEwhdW.png>

### **2.5) Brand / Logo**
- Class "`.navbar-brand`" được sử dụng để highlight logo - thương hiệu của trang web .
- **VD :**
    ```html
    <nav class="navbar navbar-expand-sm bg-dark navbar-dark">
      <a class="navbar-brand" href="#">
        <img src="https://nhanhoa.com/templates/images/logo.png" alt="Logo" style="width:200px;">
      </a>
      ...
    </nav>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/guOQ41V.png>

### **2.6) Thu gọn Navigation Bar**
- Tình huống đặt ra, đặc biệt đối với những màn hình nhỏ , người dùng muốn ẩn đi các link điều hướng và thay thế chúng bằng 1 button mà họ có thể click vào để hiện ra khi cần thiết .
- Để tạo một **navigation bar** có thể thu gọn , sử dụng một button với class "`.navbar-toggler`" , thuộc tính `.data-toggle="collapse"` và `data-target="#target"` . Sau đó gói gọn nội dung **navbar** ( links ,... ) trong phần tử `<div>` với class "`.collapse navbar-collapse`" , theo sau là id được match với giá trị `data-target` của button .
- **VD :**
    ```html
    <nav class="navbar navbar-expand-md bg-dark navbar-dark">
      <!-- Brand -->
      <a class="navbar-brand" href="#">Navbar</a>

      <!-- Toggler/collapsibe Button -->
      <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#collapsibleNavbar">
        <span class="navbar-toggler-icon"></span>
      </button>

      <!-- Navbar links -->
      <div class="collapse navbar-collapse" id="collapsibleNavbar">
        <ul class="navbar-nav">
          <li class="nav-item">
            <a class="nav-link" href="#">Link</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">Link</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">Link</a>
          </li>
        </ul>
      </div>
    </nav>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/xnW8SlS.png>

### **2.7) Navbar với Dropdown**
- **VD :**
    ```html
    <nav class="navbar navbar-expand-sm bg-dark navbar-dark">
      <!-- Brand -->
      <a class="navbar-brand" href="#">Logo</a>

      <!-- Links -->
      <ul class="navbar-nav">
        <li class="nav-item">
          <a class="nav-link" href="#">Link 1</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">Link 2</a>
        </li>

        <!-- Dropdown -->
        <li class="nav-item dropdown">
          <a class="nav-link dropdown-toggle" href="#" id="navbardrop" data-toggle="dropdown">
            Dropdown link
          </a>
          <div class="dropdown-menu">
            <a class="dropdown-item" href="#">Link 1</a>
            <a class="dropdown-item" href="#">Link 2</a>
            <a class="dropdown-item" href="#">Link 3</a>
          </div>
        </li>
      </ul>
    </nav>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/w1xpCMm.png>

### **2.8) Navbar Forms và Buttons**
- Thêm phần tử `<form>` với class "`.form-inline`" để nhóm phần input và button cạnh nhau .
    ```html
    <nav class="navbar navbar-expand-sm bg-dark navbar-dark">
      <form class="form-inline" action="/action_page.php">
        <input class="form-control mr-sm-2" type="text" placeholder="Search">
        <button class="btn btn-success" type="submit">Search</button>
      </form>
    </nav>
    ```
    - Hiển thị trên trình duyệt :
        
        <img src=https://i.imgur.com/trs3Gmn.png>
- Có thể sử dụng các class input khác , như "`.input-group-prepend`" hoặc "`.input-group-append`" để đính kèm 1 icon hoặc 1 đoạn text gợi ý cạnh trường input .
    ```html
    <nav class="navbar navbar-expand-sm bg-dark navbar-dark">
      <form class="form-inline" action="/action_page.php">
        <div class="input-group">
          <div class="input-group-prepend">
            <span class="input-group-text">@</span>
          </div>
          <input type="text" class="form-control" placeholder="Username">
        </div>
      </form>
    </nav>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/1YEd4Rk.png>

### **2.9) Navbar Text**
- Sử dụng class "`.navbar-text`" để căn chỉnh theo chiều dọc bất cứ phần tử nào bên trong **navbar** mà không phải link .
- **VD :**
    ```html
    <nav class="navbar navbar-expand-sm bg-dark navbar-dark">

    <!-- Links -->
      <ul class="navbar-nav">
        <li class="nav-item">
          <a class="nav-link" href="#">Link 1</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">Link 2</a>
        </li>
      </ul>

      <!-- Navbar text-->
      <span class="navbar-text">
        Navbar text
      </span>

    </nav>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/9180ZeO.png>
### **2.10) Fixed Navigation Bar**
- **Navigation bar** có thể được fix cứng ở trên đầu hoặc phía dưới cùng của trang web mà không phụ thuộc vào việc trang web bị cuộn lên/xuống .
- Class "`.fixed-top`" cho phép **navigation bar** được fix cứng ở đầu trang :
    ```html
    <nav class="navbar navbar-expand-sm bg-dark navbar-dark fixed-top">
      ...
    </nav>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/kyU5f6s.png>
- Class "`.fixed-bottom`" cho phép **navigation bar** được fix cứng ở cuối trang :
    ```html
    <nav class="navbar navbar-expand-sm bg-dark navbar-dark fixed-bottom">
      ...
    </nav>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/1NS82wA.png>
- Sử dụng class "`.sticky-top` để cho phép **navbar** được giữ chân lại ở đầu trang khi cuộn qua nó :
    ```html
    <nav class="navbar navbar-expand-sm bg-dark navbar-dark sticky-top">
      ...
    </nav>
    ```