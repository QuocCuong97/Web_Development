# CSS Opacity - Transparency
- Thuộc tính `opacity` khai báo độ mờ/độ trong suốt của phần tử .
## **1) Transparent Image**
- Thuộc tính `opacity` có thể nhận giá trị từ `0.0` - `1.0` . Giá trị càng nhỏ, phần tử càng trong suốt .

    <img src=https://i.imgur.com/HHKwYDa.png>

- **VD :**
    ```html
    <style>
    img {
      opacity: 0.5;
    }
    </style>
    <img src="img_forest.jpg" alt="Forest" width="170" height="100">
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/WzgyhgN.png>

## **2) Transparent Hover Effect**
- Thuộc tính `opacity` thường được sử dụng với selector `:hover` để thay đổi độ mờ khi di chuột qua phần tử .
- **VD :** 
    ```css
    img {
      opacity: 0.5;
      filter: alpha(opacity=50); /* For IE8 and earlier */
    }

    img:hover {
      opacity: 1.0;
      filter: alpha(opacity=100); /* For IE8 and earlier */
    }
    ```
## **3) Text in Transparent Box**
- **VD :**
    ```html
    <style>
    div.background {
      background: url(klematis.jpg) repeat;
      border: 2px solid black;
    }

    div.transbox {
      margin: 30px;
      background-color: #ffffff;
      border: 1px solid black;
      opacity: 0.6;
      filter: alpha(opacity=60); /* For IE8 and earlier */
    }

    div.transbox p {
      margin: 5%;
      font-weight: bold;
      color: #000000;
    }
    </style>
    <div class="background">
    <div class="transbox">
      <p>This is some text that is placed in the transparent box.</p>
    </div>
    </div>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/0mLbBXk.png>
