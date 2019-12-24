# Badges
## **1) Cơ bản về badges**
- **Badges** thường được sử dụng để thêm thông tin bổ sung cho content . Sử dụng class "`.badge`" với class biểu thị màu sắc ( như "`.badge-secondary`",....) trong phần tử `<span>` để tạo một **badge** hình chữ nhật .
    > **Badges** sẽ tự động căn chỉnh kích cỡ so với phần tử cha (nếu có)
- **VD :**
    ```html
    <h1>Example heading <span class="badge badge-secondary">New</span></h1>
    <h2>Example heading <span class="badge badge-secondary">New</span></h2>
    <h3>Example heading <span class="badge badge-secondary">New</span></h3>
    <h4>Example heading <span class="badge badge-secondary">New</span></h4>
    <h5>Example heading <span class="badge badge-secondary">New</span></h5>
    <h6>Example heading <span class="badge badge-secondary">New</span></h6>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/bfd4tG1.png>

## **2) Contextual Badges**
- Các class biểu thị màu sắc : sử dụng cấu trúc "`.badge-*`" để thay đổi màu cho **badge** :
    ```html
    <span class="badge badge-primary">Primary</span>
    <span class="badge badge-secondary">Secondary</span>
    <span class="badge badge-success">Success</span>
    <span class="badge badge-danger">Danger</span>
    <span class="badge badge-warning">Warning</span>
    <span class="badge badge-info">Info</span>
    <span class="badge badge-light">Light</span>
    <span class="badge badge-dark">Dark</span>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/Pt2Av9b.png>

## **3) Pill Badges**
- Sử dụng class "`.badge-pill`" để cho góc borber của **badge** tròn hơn :
    ```html
    <span class="badge badge-pill badge-primary">Primary</span>
    <span class="badge badge-pill badge-secondary">Secondary</span>
    <span class="badge badge-pill badge-success">Success</span>
    <span class="badge badge-pill badge-danger">Danger</span>
    <span class="badge badge-pill badge-warning">Warning</span>
    <span class="badge badge-pill badge-info">Info</span>
    <span class="badge badge-pill badge-light">Light</span>
    <span class="badge badge-pill badge-dark">Dark</span>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/aixxBmH.png>

## **4) Sử dụng badge trong một phần tử khác**
- **VD :**
    ```html
    <button type="button" class="btn btn-primary">
      Messages <span class="badge badge-light">4</span>
    </button>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/aI2JWbn.png>