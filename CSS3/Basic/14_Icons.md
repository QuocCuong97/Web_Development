# CSS Icons
<img src=https://i.imgur.com/buFh7WU.png>

## **1) Cách thêm icon trong CSS**
- Cách đơn giản nhất để thêm **icon** vào trang **HTML** là sử dụng một **thư viện icon** , như **Font Awesome** .
- Thêm các **icon class** muốn chọn vào các thẻ **inline** ( như `<i>` hoặc `<span>` )
- Thêm thẻ `<script>` có chứa link thư viện icon để gọi bộ thư viện .
## **2) Bộ thư viện "Font Awesome Icons"**
### **2.1) Cách lấy `kit code`**
- **B1 :** Để sử dụng bộ thư viện **Font Awesome icons**, vào trang web `fontawesome.com`, đăng nhập, lấy code và thêm vào thẻ `<head>` .

    <img src=https://i.imgur.com/eWIzEES.png>

- **B2 :** Sau khi đã đăng nhập, lấy `kit code` . Do **font awesome** có tính thương mại, nên phải xác định `kit code` của user nào được phép sử dụng icon nào :

    <img src=https://i.imgur.com/DdeqKaZ.png>

- **B3 :** Lưu lại `kit code` :

    <img src=https://i.imgur.com/jzWqTGx.png>

- **B4 :** Thêm `kit code` vào phần tử `<head>` theo cấu trúc :
    ```html
    <head>
      <script src="https://kit.fontawesome.com/yourcode.js"></script>
    </head>
    ```
    - **VD :**
        ```html
        <script src="https://kit.fontawesome.com/a076d05399.js"></script>
        ```



To use the Font Awesome icons, go to fontawesome.com, sign in, and get a code to add in the <head> section of your HTML page:

<script src="https://kit.fontawesome.com/yourcode.js"></script>

Read more about how to get started with Font Awesome in our Font Awesome 5 tutorial.

Note: No downloading or installation is required!
- **VD :**
    - Gọi bộ thư viện **Font Awesome** :
        ```html
        <script src="https://kit.fontawesome.com/a076d05399.js"></script>
        ```



- **VD1 :**
    ```html
    <!DOCTYPE html>
    <html>
    <head>
    <script src="https://kit.fontawesome.com/a076d05399.js"></script>
    </head>
    <body>

    <i class="fas fa-cloud"></i>
    <i class="fas fa-heart"></i>
    <i class="fas fa-car"></i>
    <i class="fas fa-file"></i>
    <i class="fas fa-bars"></i>

    </body>
    </html>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/y9acPmu.png>

- **VD2 :** Tùy chỉnh màu sắc, kích cỡ của icon :
    ```html
    <i class="fas fa-cloud" style="font-size:24px;"></i>
    <i class="fas fa-cloud" style="font-size:36px;"></i>
    <i class="fas fa-cloud" style="font-size:48px;color:red;"></i>
    <i class="fas fa-cloud" style="font-size:60px;color:lightblue;"></i>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/9I3Vwey.png>

## **2) 