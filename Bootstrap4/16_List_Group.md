# List Groups
## **1) Cơ bản về List Group**
- **List Group** cơ bản nhất là **unordered list** .
- Để tạo một **list group** cơ bản, sử dụng phần tử `<ul>` với class "`.list-group`" , và phần tử `<li>` bên trong với class "`.list-group-item`" .
- **VD :**
    ```html
    <ul class="list-group">
      <li class="list-group-item">First item</li>
      <li class="list-group-item">Second item</li>
      <li class="list-group-item">Third item</li>
    </ul>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/GhC2Cbl.png>

## **2) Trạng thái Active**
- Sử dụng class "`.active`" để highlight item đã chọn .
- **VD :**
    ```html
    <ul class="list-group">
      <li class="list-group-item active">Active item</li>
      <li class="list-group-item">Second item</li>
      <li class="list-group-item">Third item</li>
    </ul>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/WZtbPxx.png>

## **3) List Group với item được gán link**
- Để tjao một **list group** với item được gán link , sử dụng phần tử `<div>` thay vì dùng phần tử `<ul>` và phần tử `<a>` thay cho `<li>` .
- Có thể sử dụng class "`.list-group-item-action`" nếu muốn item có nền xám khi user di chuột qua .
- **VD :**
    ```html
    <div class="list-group">
      <a href="#" class="list-group-item list-group-item-action">First item</a>
      <a href="#" class="list-group-item list-group-item-action">Second item</a>
      <a href="#" class="list-group-item list-group-item-action">Third item</a>
    </div>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/GikTqul.png>

## **4) Trạng thái Disabled**
- Class "`.disabled`" được sẽ đổi màu chữ của item bị disable thành màu sáng trắng . Và item bị disable sẽ bỏ qua hiệu ứng khi di chuột qua .
- Sử dụng cho **list group** với item được gán link .
- **VD :**
    ```html
    <div class="list-group">
      <a href="#" class="list-group-item disabled">Disabled item</a>
      <a href="#" class="list-group-item disabled">Disabled item</a>
      <a href="#" class="list-group-item">Third item</a>
    </div>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/Bi61jH2.png>
## **5) Xóa border**
- Sử dụng class "`.list-group-flush`" để xóa các border và các góc bao quanh item .
- **VD :**
    ```html
    <ul class="list-group list-group-flush">
      <li class="list-group-item">First item</li>
      <li class="list-group-item">Second item</li>
      <li class="list-group-item">Third item</li>
      <li class="list-group-item">Fourth item</li>
    </ul>
    ```
    - Hiển thị trên trình duyệt :
        
        <img src=https://i.imgur.com/hxqhMxY.png>

## **6) Horizontal List Groups**
- Nếu muốn list các item được hiển thị theo chiều ngang thay vì theo chiều dọc , thêm class "`.list-group-horizontal`" vào phần tử chứa class "`.list-group`" .
- **VD :**
    ```html
    <ul class="list-group list-group-horizontal">
      <li class="list-group-item">First item</li>
      <li class="list-group-item">Second item</li>
      <li class="list-group-item">Third item</li>
      <li class="list-group-item">Fourth item</li>
    </ul>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/Oqqg40H.png>

## **7) Sử dụng các class biểu thị màu sắc**
- Các class để hiển thị màu nền cho list-item là : 
    - `.list-group-item-success`
    - `.list-group-item-secondary`
    - `.list-group-item-info`
    - `.list-group-item-warning`
    - `.list-group-item-danger`
    - `.list-group-item-primary`
    - `.list-group-item-dark`
    - `.list-group-item-light`
- **VD1 :**
    ```html
    <ul class="list-group">
      <li class="list-group-item list-group-item-success">Success item</li>
      <li class="list-group-item list-group-item-secondary">Secondary item</li>
      <li class="list-group-item list-group-item-info">Info item</li>
      <li class="list-group-item list-group-item-warning">Warning item</li>
      <li class="list-group-item list-group-item-danger">Danger item</li>
      <li class="list-group-item list-group-item-primary">Primary item</li>
      <li class="list-group-item list-group-item-dark">Dark item</li>
      <li class="list-group-item list-group-item-light">Light item</li>
    </ul>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/kbq49x7.png>

## **8) Thêm Badges vào List Group**
- Gộp class "`.badge`" với các class hỗ trợ khác để thêm **badge** vào trong **list group** .
- **VD :**
    ```html
    <ul class="list-group">
      <li class="list-group-item d-flex justify-content-between align-items-center">
        Inbox
        <span class="badge badge-primary badge-pill">12</span>
      </li>
      <li class="list-group-item d-flex justify-content-between align-items-center">
        Ads
        <span class="badge badge-primary badge-pill">50</span>
      </li>
      <li class="list-group-item d-flex justify-content-between align-items-center">
        Junk
        <span class="badge badge-primary badge-pill">99</span>
      </li>
    </ul>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/Mc9gmrY.png>

