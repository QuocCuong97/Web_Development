# Links
## **1) Giới thiệu**
- Link HTML (hay liên kết HTML) được tìm thấy trên gần như tất cả các trang web :
    - Link HTML dùng để tham chiếu tới các địa chỉ trang web khác nhau.
    - Link HTML có thể tham chiếu tới trang web trên cùng một website hoặc nằm ở một website khác.
- Link HTML là hyperlink, điều này có nghĩa rằng người dùng có thể click (hoặc tab nếu trên thiết bị điện thoại) lên liên kết để đi tới trang đích.
- Hyperlinks được định nghĩa qua thẻ `<a>` :
    ```html
    <a href="url" title="title">link_text</a>
    ```
    - Trong đó :
        - `url` là URL trang đích.
        - `title` là tiêu đề của liên kết, mô tả ngắn gọn về nội dung trang đích.
        - `link_text` là chữ hiển thị liên kết để người dùng có thể click vào.
- **VD :**
    ```html
    <a href="https://www.facebook.com/" title="Trang chủ Facebook">Facebook</a>
    ```
    => Hiển thị trên trình duyệt :

    <img src=https://i.imgur.com/rVjiGYi.png>

## **2) Local Links**
- Trường hợp đường dẫn của trang đích trong link HTML ở trên cùng một website với trang web hiện tại thì chúng ta có thể sử dụng địa chỉ tương đối .
- **VD :**
    ```html
    <a href="/images/HTML" title="HTML Images">Images</a>
    ```
## **3) Link Color**
- Mặc định , một đường link sẽ xuất hiện trong trình duyệt ở định dạng :
    - Một link chưa được truy cập sẽ được gạch chân và có màu xanh dương .
    - Một link đã được truy cập sẽ được gạch chân và có màu tím .
    - Một link active sẽ được gạch chân và có màu đỏ .
- Có thể thay đổi mặc định này bằng cách sử dụng **CSS** :
- **VD :**
    ```html
    <style>
    a:link {
    color: green;
    background-color: transparent;
    text-decoration: none;
    }
    a:visited {
    color: pink;
    background-color: transparent;
    text-decoration: none;
    }
    a:hover {
    color: red;
    background-color: transparent;
    text-decoration: underline;
    }
    a:active {
    color: yellow;
    background-color: transparent;
    text-decoration: underline;
    }
    </style>
    </head>
    <body>

    <h2>Link Colors</h2>

    <p>You can change the default colors of links</p>

    <a href="https://www.facebook.com/" title="Trang chủ Facebook">Facebook</a>
    ```
    => Hiển thị trên trình duyệt :

    <img src=https://i.imgur.com/apPX3Nr.png>

## **4) Thuộc tính `target`**
- Thuộc tính `target` được dùng để xác định địa chỉ trang đích của liên kết . Trình duyệt sẽ mở trang này khi người dùng click (hoặc tab) lên liên kết .
- Thuộc tính `target` có thể nhận một trong các giá trị sau:
    - `_blank` : Với giá trị này thì trình duyệt sẽ mở trang đích ở một cửa sổ hoặc tab mới.
    - `_self` : Với giá trị này thì trình duyệt sẽ mở trang đích ở cửa sổ hoặc tab hiện tại (đây là giá trị mặc định).
    - `_parent` : Với giá trị này thì trình duyệt sẽ mở trang đích thay thế frame cha (`*`)
    - `_top` : Với giá trị này thì trình duyệt sẽ mở trang đích trên toàn bộ màn hình
    - `framename` : Với giá trị này thì trình duyệt sẽ mở trang đích ở frame với tên cho trước.(`*`)
## **5) Chèn link vào hình ảnh**
- Để tạo một link hình ảnh chúng ta sẽ thay thế `link_text` bằng một phần tử `img` :
    ```html
    <a href="https://www.facebook.com/" title="Trang chủ Facebook">
        <img src="https://i.imgur.com/0JkPv6st.png">
    </a>
    ```
    => Hiển thị trên trình duyệt :

    <img src=https://i.imgur.com/HoTYV1W.png>

## **6) Bookmark**
- Để link tới một phần tử trên trang với giá trị cho trước của thuộc tính `id` , chúng ta sử dụng link bookmark . Lúc này đích đến chính là phần tử với thuộc tính `id` cho trước nằm trên cùng một trang với trang hiện tại .
- **VD :**
    - Tạo 1 bookmark :
        ```html
        <h2 id="C4">Chapter 4</h2>
        ```
    - Gọi liên kết tới bookmark ( trong cùng trang web ) :
        ```html
        <a href="#C4">Jump to Chapter 4</a>
        ```
    - Thêm bookmark vào trang web khác ( cùng folder ):
        ```html
        <a href="html_demo.html#C4">Jump to Chapter 4</a>
        ```
        