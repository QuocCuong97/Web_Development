# CSS Lists
- Áp dụng **CSS** cho phép :
    - Sử dụng các kiểu đánh dấu list khác nhau .
    - Sử dụng hình ảnh để đánh dấu list .
    - Thêm màu nền cho list và các mục trong list .
## **1) CSS `list-style-type`**
- Thuộc tính `list-style-type` khai báo kiểu đánh dấu list .
- **VD :**
    ```html
    <style>
    ul.a {
      list-style-type: circle;
    }

    ul.b {
      list-style-type: square;
    }

    ol.c {
      list-style-type: upper-roman;
    }

    ol.d {
      list-style-type: lower-alpha;
    }
    </style>
    <p>Example of unordered lists:</p>
    <ul class="a">
      <li>Coffee</li>
      <li>Tea</li>
      <li>Coca Cola</li>
    </ul>

    <ul class="b">
      <li>Coffee</li>
      <li>Tea</li>
      <li>Coca Cola</li>
    </ul>

    <p>Example of ordered lists:</p>
    <ol class="c">
      <li>Coffee</li>
      <li>Tea</li>
      <li>Coca Cola</li>
    </ol>

    <ol class="d">
      <li>Coffee</li>
      <li>Tea</li>
      <li>Coca Cola</li>
    </ol>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/rkMcg7O.png>

## **2) CSS `list-style-image`**
- Thuộc tính `list-style-image` khai báo hình ảnh sử dụng để dùng để đánh dấu list .
- **VD :**
    ```css
    ul {
      list-style-image: url('sqpurple.gif');
    }
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/EB4dTVc.png>

## **3) CSS `list-style-position`**
- Thuộc tính `list-style-position` khai báo vị trí của phần đánh dấu list .
- Thuộc tính `list-style-position` có 2 giá trị :
    - `outside` : có nghĩa dấu tròn sẽ ở bên ngoài dòng chữ, chữ đầu dòng không bị thụt vào
    - `inside` : có nghĩa dấu tròn sẽ ở trên dòng chữ , chữ đầu tiên phải thụt vào để dư chỗ cho dấu tròn .
- **VD :**
    ```html
    <style>
    ul.a {
      list-style-position: outside;
    }

    ul.b {
      list-style-position: inside;
    }
    </style>