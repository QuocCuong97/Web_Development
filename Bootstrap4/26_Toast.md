# Toast
## **1) Cơ bản về Toast**
- **Toast** giống như một hộp thoại cảnh báo chỉ xuất hiện một vài giây khi có một điều gì đó xảy ra ( như khi user click vào một button, submit form,....)
- Để tạo ra một **toast**, sử dụng class "`.toast`" và thêm class "`.toast-header`" và "`.toast-body`" bên trong nó .
- **VD :**
    ```html
    <div class="toast">
      <div class="toast-header">Toast Header</div>
      <div class="toast-body">Some text inside the toast body</div>
    </div>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/Z3ya99H.png>

## **2) Ẩn và hiện Toast**
- Mặc định , **toast** sẽ bị ẩn đi .
- Sử dụng thuộc tính `data-autohide="false"` để hiển thị **toast** mặc định .
- Để đóng **toast**, sử dụng phần tử `<button>` và thêm thuộc tính `data-dismiss="toast"` :
    ```html
    <div class="toast" data-autohide="false">
      <div class="toast-header">
        <strong class="mr-auto text-primary">Toast Header</strong>
        <small class="text-muted">5 mins ago</small>
        <button type="button" class="ml-2 mb-1 close" data-dismiss="toast">&times;</button>
      </div>
      <div class="toast-body">
        Some text inside the toast body
      </div>
    </div>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/QzBYevv.png>