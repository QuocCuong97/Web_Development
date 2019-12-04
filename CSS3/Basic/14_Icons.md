# CSS Icons
<img src=https://i.imgur.com/buFh7WU.png>


## **1) Bộ thư viện "Font Awesome Icons"**
### **1.1) Cách lấy `kit code`**
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
### **1.2) Cách insert icons**
- Thêm các **icon class** muốn chọn vào các thẻ **inline** ( như `<i>` hoặc `<span>` )
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

## **2) Bộ thư viện "Bootstrap Icons"**
- Để sử dụng bộ thư viện **Bootstrap Icons**, khai báo thêm dòng sau vào phần tử `<head>` :
    ```html
    <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css">
    ```
- **VD1 :**
    ```html
    <!DOCTYPE html>
    <html>
    <head>
    <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css">
    </head>
    <body>

    <i class="glyphicon glyphicon-cloud"></i>
    <i class="glyphicon glyphicon-remove"></i>
    <i class="glyphicon glyphicon-user"></i>
    <i class="glyphicon glyphicon-envelope"></i>
    <i class="glyphicon glyphicon-thumbs-up"></i>

    </body>
    </html>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/cVk4fWL.png>

- **VD2 :** Tùy chỉnh màu sắc, kích cỡ của icon :
    ```html
    <i class="glyphicon glyphicon-cloud" style="font-size:24px;"></i>
    <i class="glyphicon glyphicon-cloud" style="font-size:36px;"></i>
    <i class="glyphicon glyphicon-cloud" style="font-size:48px;color:red;"></i>
    <i class="glyphicon glyphicon-cloud" style="font-size:60px;color:lightblue;"></i>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/185Oq0V.png>

## **3) Bộ thư viện "Google Icons"**
- Để sử dụng bộ thư viện **Google Icons** , khai báo thêm dòng sau vào phần tử `<head>` :
    ```html
    <link rel="stylesheet" href="https://fonts.googleapis.com/icon?family=Material+Icons">
    ```
- **VD1 :**
    ```html
    <!DOCTYPE html>
    <html>
    <head>
    <link rel="stylesheet" href="https://fonts.googleapis.com/icon?family=Material+Icons">
    </head>
    <body>

    <i class="material-icons">cloud</i>
    <i class="material-icons">favorite</i>
    <i class="material-icons">attachment</i>
    <i class="material-icons">computer</i>
    <i class="material-icons">traffic</i>

    </body>
    </html>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/PgR1Ska.png>

- **VD2 :** Tùy chỉnh màu sắc, kích cỡ của icon :
    ```html
    <i class="material-icons" style="font-size:24px;">cloud</i>
    <i class="material-icons" style="font-size:36px;">cloud</i>
    <i class="material-icons" style="font-size:48px;color:red;">cloud</i>
    <i class="material-icons" style="font-size:60px;color:lightblue;">cloud</i>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/KTns16S.png>

[Tham khảo thêm](https://www.w3schools.com/icons/default.asp)