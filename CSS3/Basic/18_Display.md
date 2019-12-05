# CSS Layout - Thuộc tính `display`
## **1) Thuộc tính `display`**
- Thuộc tính `display` là một thuộc tính quan trọng trong **CSS** để kiểm soát layout của trang .
- Thuộc tính `display` khai báo cách mà phần tử được hiển thị .
- Tất cả các phần tử **HTML** đều có giá trị hiển thị mặc định tùy theo nó là phàn tử gì . Các giá trị mặc định đó là `block` và `inline` .
- Một số phần tử `block` :

    <img src=https://i.imgur.com/VZE4fiz.png>

    - `<div>`
    - `<h1>` - `<h6>`
    - `<p>`
    - `<form>`
    - `<header>`
    - `<footer>`
    - `<section>`

- Một số phần tử `inline` :

    <img src=https://i.imgur.com/td8nV8y.png>

    - `<span>`
    - `<a>`
    - `<img>`
## **2) Ghi đè giá trị hiển thị của phần tử**
- Giá trị hiển thị của phần tử có thể bị ghi đè , biến một phần tử `inline` thành một phần tử `block` hoặc ngược lại . Điều này có thể hữu ích để nhìn trang web một cách sống động hơn mà vẫn không phá chuẩn của web .
- **VD :** Chuyển `<li>` từ một phần tử `block` thành một phần tử `inline` :
    ```html
    <style>
    li {
      display: inline;
    }
    </style>
    <ul>
      <li><a href="/html/default.asp" target="_blank">HTML</a></li>
      <li><a href="/css/default.asp" target="_blank">CSS</a></li>
      <li><a href="/js/default.asp" target="_blank">JavaScript</a></li>
    </ul>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/4aN239N.png>

## **3) Ẩn phần tử trong CSS**
- Giá trị "`display: none;`" thường được sử dụng với JavaScript để ẩn/hiện các phần tử mà không cần xóa và tạo lại chúng .
- Mặc định phần tử `<script>` sử dụng giá trị "`display: none;`"
- Phần tử sau khi bị ẩn sẽ bị coi như không có trong trang, không chiếm không gian của trang .
- **VD1 :**
    ```html
    <style>
    h1.hidden {
      display: none;
    }
    </style>
    <h1>This is a visible heading</h1>
    <h1 class="hidden">This is a hidden heading</h1>
    <p>Notice that the h1 element with display: none; does not take up any space.</p>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/kuEx8Yo.png>

- Thuộc tính "`visibility:hidden`" cũng là một cách để ẩn phần tử .
- Tuy nhiên, phần tử bị ẩn nhưng vẫn chiếm lấy khoảng không gian mà nó cần chiếm .
- **VD2 :**
    ```html
    <style>
    h1.hidden {
      visibility: hidden;
    }
    </style>
    <h1>This is a visible heading</h1>
    <h1 class="hidden">This is a hidden heading</h1>
    <p>Notice that the hidden heading still takes up space.</p>
    ```
    - Hiển thị trên trình duyệt :   

        <img src=https://i.imgur.com/hhlQ8W3.png>