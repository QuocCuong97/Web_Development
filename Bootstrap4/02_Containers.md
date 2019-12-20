# Containers
- **Container** được sử dụng để chứa content bên trong nó .
- Có 2 kiểu class container :
    - Class "`.container`" cung cấp một **reponsive container** với chiều rộng được fix theo trình duyệt .
    - Class "`.container-fluid`" cung cấp một **container** với full chiều rộng trải dài hết chiều rộng của viewport .

        <img src=https://i.imgur.com/nPVKfUQ.png>

## **1) Fixed Container**
- Sử dụng class "`.container`" để tạo 1 **reponsive** container, với chiều rộng được fix theo trình duyệt .
- Thuộc tính `max-width` của container sẽ thay đổi tùy theo các kích cỡ màn hình khác nhau :

    | | Siêu nhỏ<br>`<576px` | Nhỏ<br><code>&ge;576px</code> | Trung bình<br><code>&ge;768px</code> | Lớn<br><code>&ge;992px</code> | Siêu Lớn<br><code>&ge;1200px</code> |
    |-|----------------------|-------------------------------|--------------------------------------|----------------|-------------------------------|
    | `max-width` | `100%` | `540px` | `720px` | `960px` | `1140px` |
- **VD :**
    ```html
    <div class="container">
      <h1>My First Bootstrap Page</h1>
      <p>This is some text.</p>
    </div>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/b36Ic1M.png>

## **2) Fluid Container**
- Sử dụng class "`.container-fluid`" để tạo một container full chiều rộng , trải dài toàn bộ chiều rộng của màn hình ( `width = 100%` )
- **VD :**
    ```html
    <div class="container-fluid">
      <h1>My First Bootstrap Page</h1>
      <p>This is some text.</p>
    </div>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/8lqVoTh.png>

<!-- ## **3) Container Padding**
- Mặc định, container có `padding-left` và `padding-right` là `15px` .
- Do đó, sử dụng thêm những tiện ích ( **spacing ultilities** ) như thêm padding hay margin sẽ giúp trang web hiển thị tốt hơn .
- **VD :** Thêm class "`.pt-3`" có nghĩa là thêm `padding-top` là `16px` :
    ```html
    <div class="container pt-3">
      <h1>My First Bootstrap Page</h1>
      <p>This container has a top padding of 16 pixels (.pt-3).</p>
    </div>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/gIrsY0h.png> -->
## **3) Responsive Containers**
- Có thể sử dụng các class "`.container-sm|md|lg|xl`" để tạo các responsive container .
- Chiều rộng (thuộc tính `max-width`) của container sẽ thay đổi tùy theo các kích cỡ màn hình khác nhau :

    | Class | ExtraSmall<br>`<576px` | Small<br><code>&ge;576px</code> | Medium<br><code>&ge;768px</code> | Large<br><code>&ge;992px</code> | ExtraLarge<br><code>&ge;1200px</code> |
    |-------|------------------------|------------------------------------|-------------------------------|--------------------------------|---------------------------------------|
    | `.container-sm` | `100%` | `540px` | `720px` | `960px` | `1140px` |
    | `.container-md` | `100%` | `100%` | `720px` | `960px` | `1140px` |
    | `.container-lg` | `100%` | `100%` | `100%` | `960px` | `1140px` |
    | `.container-xl` | `100%` | `100%` | `100%` | `100%` | `1140px` |
- **VD :**
    ```html
    <div class="container-sm">.container-sm</div>
    <div class="container-md">.container-md</div>
    <div class="container-lg">.container-lg</div>
    <div class="container-xl">.container-xl</div>
    ```