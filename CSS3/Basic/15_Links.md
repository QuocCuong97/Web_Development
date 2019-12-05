# CSS Link
- Với **CSS**, link có thể được tạo kiểu theo nhiều cách khác nhau .
## **1) Tạo kiểu cho `link`**
- Link có thể được tạo kiểu với các thuộc tính **CSS** ( như `color`, `font-family`, `background`, ....)
- **VD :**
    ```css
    a {
      color: hotpink;
    }
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/MyYWH4Q.png>

- Thêm vào đó, link có thể được tạo kiểu khác nhau dựa theo trạng thái của nó . Có 4 trạng thái của link :
    - `a:link` - trạng thái bình thường, ?????
    - `a:visited` - link đã được user click từ trước
    - `a:hover` - link khi được user di chuột qua'
    - `a:active` - link vào thời điểm user click chuột
- **VD :**
    ```css
    /* unvisited link */
    a:link {
      color: red;
    }

    /* visited link */
    a:visited {
      color: green;
    }

    /* mouse over link */
    a:hover {
      color: hotpink;
    }

    /* selected link */
    a:active {
      color: blue;
    }
    ```
## **2) CSS `text-decoration`**
- Thuộc tính `text-decoration` thường được sử dụng để bỏ dấu gạch dưới của link .
- **VD :**
    ```css
    a:link {
      text-decoration: none;
    }

    a:visited {
      text-decoration: none;
    }

    a:hover {
      text-decoration: underline;
    }

    a:active {
      text-decoration: underline;
    }
    ```
## **3) CSS `background-color`**
- Thuộc tính `background-color` được sử dụng để khai báo màu nền cho link .
- **VD :**
    ```css
    a:link {
      background-color: yellow;
    }

    a:visited {
      background-color: cyan;
    }

    a:hover {
      background-color: lightgreen;
    }

    a:active {
      background-color: hotpink;
    } 
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/yZFQI87.png>

## **4) Link Buttons**
- Có thể gộp một số thuộc tính **CSS** để hiển thị link dưới dạng 1 button :
    ```html
    <style>
    a:link, a:visited {
      background-color: #f44336;
      color: white;
      padding: 14px 25px;
      text-align: center;
      text-decoration: none;
      display: inline-block;
    }
    a:hover, a:active {
      background-color: red;
    }
    </style>
    <a href="default.asp" target="_blank">This is a link</a>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/n7uaITq.png>