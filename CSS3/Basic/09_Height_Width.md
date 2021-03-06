# CSS Height/Width
## **1) CSS `height` - `width`**
- Thuộc tính `height` và `width` được sử dụng để set chiều cao và chiều rộng của phần tử .
- Thuộc tính `height` và `width` không bao gồm `padding` , `border` và `margin` . Nó chỉ set chiều cao cho phần nội dung phía trong padding, border và margin của một phần tử .
- Thuộc tính `height` và `width` có thể chứa các giá trị sau :
    - `auto` - mặc định . browser tự tính toán height và width
    - `length` - chỉ định height và width theo đơn vị `px`, `pt`, `cm`, ...
    - `%` - chỉ định height và width theo `%` chiều rộng của phần tử chứa nó 
    - `initial` - 
    - `inherit` - chỉ định height/width sẽ kế thừa thông số height/width của phần tử cha ( phần tử mà nó bị lồng ở trong )
    ???????
    ??????????
### **Cách sử dụng `width`, `max-width` và `margin: auto`**
- Set thuộc tính `width` của các phần tử block sẽ ngăn chúng không bị giãn về mép của phần tử cha . Sau đó , có thể set `margin` là `auto` để cân đối phần tử bên trong phần tử cha . Phần tử sẽ chiếm phần `width` được khai báo trước đó, và phần không gian còn lại sẽ được chia đôi cho 2 bên margin :
- **VD :**
    ```html
    <style>
    div.ex1 {
      width: 500px;
      margin: auto;
      border: 3px solid #73AD21;
    }
    </style>
    <div class="ex1">This div element has width: 500px;</div>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/NPIjOg7.png>

- Thay vào đó nếu sử dụng thuộc tính `max-width`, trong trường hợp này , sẽ cải thiện cách xử lý của trình duyệt đối với những tab nhỏ . Việc ày rất quan trọng khi hiển thị trang web trên các thiết bị di động có màn hình nhỏ .
- **VD2 :**
    ```html
    <style>
    div.ex2 {
      max-width: 500px;
      margin: auto;
      border: 3px solid #73AD21;
    }
    <div class="ex2">This div element has max-width: 500px;</div>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/umbjd5T.png>

- Khác biệt khi hiển thị trên các thiết bị nhỏ hơn :

    <img src=https://i.imgur.com/JprN1gO.png>
