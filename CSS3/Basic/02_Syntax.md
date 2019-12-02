# Cú pháp CSS
## **1) Cú pháp**
- Một bộ quy tắc **CSS** bao gồm thẻ được chọn ( **selector** ) và phần khai báo thuộc tính ( **declaration block** )

    <img src=https://i.imgur.com/128ZOHt.gif>

- Phần **selector** là tên phần tử **HTML** muốn áp dụng style .
- **Declaration block** chứa một hoặc nhiều phần khai báo được khai báo cách nhau bởi dấu "`;`" .
- Mỗi phần khai báo bao gồm tên 1 thuộc tính **CSS** và giá trị của nó, ngăn cách nhau bởi dấu "`:`**
- **Declaration block** luôn kết thúc bằng dấu "`;`" , và được nằm trong cặp dấu ngoặc nhọn "`{}`" .
- **VD :**
    ```css
    p {
      color: red;
      text-align: center;
    }
    ```
## **2) CSS comment**
- Comment được sử dụng để giải thích code , giúp hiểu đoạn code sau một thời gian không dùng tới .
- Comment không ảnh hưởng đến code , sẽ được bỏ qua bởi trình duyệt
- **VD :**
    ```css
    p {
      color: red;
      /* This is a single-line comment */
      text-align: center;
    }

    /* This is
    a multi-line
    comment */
    ```
    