# Class
## **1) Sử dụng thuộc tính `class` trong các phần tử block**
- Thuộc tính `class` được sử dụng để xác định `style` có các phần tử có cùng `class` . Vì vậy, các phần tử có cùng thuộc tính `class` sẽ có cùng `style` .
- **VD :**
    ```html
    <!DOCTYPE html>
    <html>
    <head>
    <style>
    .cities {
      background-color: black;
      color: white;
      margin: 20px;
      padding: 20px;
    }
    </style>
    </head>
    <body>

    <div class="cities">
      <h2>London</h2>
      <p>London is the capital of England.</p>
    </div>

    <div class="cities">
      <h2>Paris</h2>
      <p>Paris is the capital of France.</p>
    </div>

    <div class="cities">
      <h2>Tokyo</h2>
      <p>Tokyo is the capital of Japan.</p>
    </div>

    </body>
    </html>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/P6MzYto.png>

## **2) Sử dụng thuộc tính `class` trong phần tử Inline**
- Thuộc tính `class` cũng có thể được sử dụng trong các phần tử **inline** :
    ```html
    <!DOCTYPE html>
    <html>
    <head>
    <style>
    span.note {
      font-size: 120%;
      color: red;
    }
    </style>
    </head>
    <body>

    <h1>My <span class="note">Important</span> Heading</h1>
    <p>This is some <span class="note">important</span> text.</p>

    </body>
    </html>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/Mzhpihm.png>

## **3) Sử dụng nhiều `class` cho một phần tử**
- Phần tử trong HTML có thể sử dụng nhiều hơn 1 class, mỗi class được gọi tên cách nhau một dấu `space` .
- **VD :**
    ```html
    <!DOCTYPE html>
    <html>
    <style>
    .city {
      background-color: tomato;
      color: white;
      padding: 10px;
    } 

    .main {
      text-align: center;
    }
    </style>
    <body>

    <h2>Multiple Classes</h2>
    <p>All three headers have the class name "city". In addition, London also have the class name "main", which center-aligns the text.</p>

    <h2 class="city main">London</h2>
    <h2 class="city">Paris</h2>
    <h2 class="city">Tokyo</h2>

    </body>
    </html>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/46Zfxx8.png>

## **4) Sử dụng cùng `class` cho các tag khác nhau**
- **VD :**
    ```html
    <h2 class="city">Paris</h2>
    <p class="city">Paris is the capital of France.</p>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/566juYI.png>

## **5) Sử dụng thuộc tính `class` trong JavaScript**