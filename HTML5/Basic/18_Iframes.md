# Iframes
## **1) Công thức Iframe**
- Một **iframe** được sử dụng để hiển thị 1 trang web trong một trang web .
- Một **iframe** được định nghĩa bằng thẻ `<iframe>` theo công thức :
    ```html
    <iframe src="URL"></iframe>
    ```
    - Thuộc tính `src` biểu thị trang web sẽ được hiển thị trong **iframe** .
## **2) Đặt chiều cao và chiều rộng cho iframe**
- Sử dụng thuộc tính `height` và `width` để chỉ định kích cỡ của **iframe** .
- Đơn vị của `height` và `width` mặc định là `pixel` .
- **VD :**
    ```html
    <iframe src="demo_iframe.html" height="200" width="300"></iframe>
    ```
- Cũng có thể sử dụng **CSS** để chỉ định chiều rộng và chiều cao cho **iframe** :
    ```html
    <iframe src="demo_iframe.html" style="height:200px;width:300px;"></iframe>
    ```
## **3) Xóa viền của iframe**
- Mặc định, **iframe** sẽ có một đường border quanh nó .
- Để loại bỏ đường border này, thêm thuộc tính `style` và sử dụng thuộc tính `border` trong **CSS** :
    ```html
    <iframe src="demo_iframe.html" style="border:none;"></iframe>
    ```
- Hoặc với **CSS** , cũng có thê thay đổi style, kích cỡ, màu sắc của đường border :
    ```html
    <iframe src="demo_iframe.htm" style="border:2px solid red;"></iframe>
    ```
## **4) Sử dụng iframe để hứng 1 link**
- Một **iframe** có thể được sử dụng để là **target** cho một link .
- Thuộc tính `target` của link phải trùng với thuộc tính `name` của **iframe** .
- **VD :**
    ```html
    <!DOCTYPE html>
    <html>
    <body>

    <iframe height="300px" width="100%" src="demo_iframe.htm" name="iframe_a"></iframe>

    <p><a href="https://tinhte.vn" target="iframe_a">Tinhte.vn</a></p>

    <p>When the target of a link matches the name of an iframe, the link will open in the iframe.</p>

    </body>
    </html>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/KY76GQn.png>


    

