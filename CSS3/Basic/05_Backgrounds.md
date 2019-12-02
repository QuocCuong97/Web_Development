# CSS Background
## **1) CSS `background-color`**
- Thuộc tính `background-color` khai báo màu nền của phần tử .
- Với **CSS** , màu sắc có thể được khai báo bằng :
    - Tên màu - **VD :** `red`
    - Mã HEX - **VD :** `#ff0000`
    - Mã RGB - **VD :** `rgb(255,0,0)`
- **VD :**
    ```html
    <style>
    body {
      background-color: lightblue;
    }
    </style>
    <body>
      <p>Hello World!</p>
      <p>This page has a light blue background color!</p>
    </body>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/OEeRXqO.png>

## **2) CSS `background-image`**
- Thuộc tính `background-image` khai báo hình ảnh được sử dụng để làm hình nền cho phần tử .
- Mặc định , hình ảnh sẽ được lặp lại để có thể lấp kín phần tử .
- **VD :**
    ```html
    <style>
      body {
      background-image: url("paper.gif");
    }
    </style>
    <body>
    <h1>Hello World!</h1>
      <p>This page has an image as the background!</p>
    </body>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/gBEpcCX.png>

## **3) CSS `background-repeat`**
- Mặc định , thuộc tính `background-image` lặp lại hình ảnh cả về chiều ngang và chiều dọc .
- Một số hình ảnh nên chỉ được lặp lại theo chiều dọc hoặc chiều ngang , nếu không sẽ nhìn rất kỳ lạ :

    <img src=https://i.imgur.com/zpP8azY.png>

- Giá trị của thuộc tính `background-repeat` :
    - `repeat-x` : lặp ảnh theo chiều ngang
    - `repeat-y` : lặp lại theo chiều dọc
    - `no-repeat` : ảnh chỉ hiển thị theo đúng kích cỡ và không lặp lại
- **VD :** Sửa lại trường hợp trên :
    ```html
    <style>
    body {
      background-image: url("gradient_bg.png");
      background-repeat: repeat-x;
    }
    </style>
    <body>
      <h1>Hello World!</h1>
      <p>Here, a background image is repeated only horizontally!</p>
    </body>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/E5kQFCV.png>

## **4) CSS `background-position`**
- Thuộc tính `background-position` được sử dụng để chỉ ra vị trí của ảnh nền trong phần tử .
- **VD :**
    ```html
    <style>
    body {
      background-image: url("img_tree.png");
      background-repeat: no-repeat;
      background-position: right top;
      margin-right: 200px;
    }
    </style>
    <body>
      <h1>Hello World!</h1>
      <p>Now the background image is only shown once, and positioned away from the text.</p>
    </body>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/Xep2Ste.png>

## **5) CSS `background-attachment`**
- Thuộc tính `background-attachment` chỉ định hình nền sẽ ở chế độ ghim hoặc sẽ bị cuộn xuống theo trang web .
- Giá trị của thuộc tính `background-attachment` :
    - `fixed` : ảnh sẽ được ghim và không bị cuộn theo trang web .
    - `scroll` : ảnh sẽ bị cuộn theo trang web
- **VD :**
    ```html
    <style>
    body {
      background-image: url("img_tree.png");
      background-repeat: no-repeat;
      background-position: right top;
      margin-right: 200px;
      background-attachment: fixed;
    }
    </style>
## **6) CSS `background` - Rút ngắn code**
- Để làm ngắn code , có thể khai báo thuộc tính `background` trong đúng 1 dòng .
- **VD :**
    ```css
    body {
      background: #ffffff url("img_tree.png") no-repeat right top;
    }
    ```