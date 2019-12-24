# Spinners
## **1) Cơ bản về spinner**
- Để tạo một icon spinner/loader , sử dụng class "`.spinner-border`" :
    ```html
    <div class="spinner-border"></div>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/PyHWBNV.png>
## **2) Colored Spinners**
- Có thể sử dụng các tiện ích để thêm màu cho spinner :
    ```html
    <div class="spinner-border text-muted"></div>
    <div class="spinner-border text-primary"></div>
    <div class="spinner-border text-success"></div>
    <div class="spinner-border text-info"></div>
    <div class="spinner-border text-warning"></div>
    <div class="spinner-border text-danger"></div>
    <div class="spinner-border text-secondary"></div>
    <div class="spinner-border text-dark"></div>
    <div class="spinner-border text-light"></div>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/9WxgnPU.png>
## **3) Growing Spinners**
- Sử dụng class "`.spinner-grow`" nếu muốn hiệu ứng spinner to dần /nhỏ dần thay vì quay tròn như mặc định :
    ```html
    <div class="spinner-grow text-muted"></div>
    <div class="spinner-grow text-primary"></div>
    <div class="spinner-grow text-success"></div>
    <div class="spinner-grow text-info"></div>
    <div class="spinner-grow text-warning"></div>
    <div class="spinner-grow text-danger"></div>
    <div class="spinner-grow text-secondary"></div>
    <div class="spinner-grow text-dark"></div>
    <div class="spinner-grow text-light"></div>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/3H9ZaJm.png>
## **4) Spinner Size**
- Sử dụng class "`.spinner-border-sm`" hoặc "`.spinner-grow-sm`" để tạo các spinner nhỏ hơn :
    ```html
    <div class="spinner-border spinner-border-sm"></div>
    <div class="spinner-grow spinner-grow-sm"></div>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/hfaKPOf.png>
## **5) Spinner Buttons**
- Có thể thêm spinner vào trong 1 button - có hoặc không có text :
    ```html
    <button class="btn btn-primary">
      <span class="spinner-border spinner-border-sm"></span>
    </button>

    <button class="btn btn-primary">
      <span class="spinner-border spinner-border-sm"></span>
    Loading..
    </button>

    <button class="btn btn-primary" disabled>
      <span class="spinner-border spinner-border-sm"></span>
    Loading..
    </button>

    <button class="btn btn-primary" disabled>
      <span class="spinner-grow spinner-grow-sm"></span>
    Loading..
    </button>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/tgP7SxE.png>
