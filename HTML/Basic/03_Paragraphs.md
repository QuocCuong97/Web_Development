# Paragraphs
## **1) Giới thiệu**
- Để đánh dấu một đoạn văn bản thì chúng ta sử dụng thẻ `<p>` trong **HTML** .
- Cú pháp :
    ```html
    <p>Pargraphs</p>
## **2) Hiển thị HTML**
- **HTML** sẽ hiển thị theo đúng chuẩn của nó .
- Màn hình lớn hay màn hình nhỏ , cửa sổ lớn hay cửa sổ nhỏ sẽ hiển thị theo các cách khác nhau .
- Với **HTML** , không thể thay đổi nội dung hiển thị bằng cách add thêm `spaces` hoặc các dòng trống trong đoạn code . Trình duyệt sẽ tự động xóa những `space` và những dòng trống không cần thiết khi hiển thị trang :
- **VD :**
    ```html
    <p>
    This paragraph
    contains a lot of lines
    in the source code,
    but the browser
    ignores it.
    </p>

    <p>
    This paragraph
    contains         a lot of spaces
    in the source         code,
    but the        browser
    ignores it.
    </p>
    ```
    => Hiển thị trên trình duyệt :

    <img src=https://i.imgur.com/ZT9h9nQ.png>

## **3) Xuống dòng trong HTML**
- Sử dụng phần tử `<br>` để xuống dòng trong **HTML** .
- Thẻ `<br>` là thẻ tự đóng .
- **VD :**
    ```html
    <p>This is<br>a paragraph<br>with line breaks.</p>
    ```
    => Hiển thị trên trình duyệt :

    <img src=https://i.imgur.com/tXhzQhq.png>

## **4) Phần tử `<pre>`**
- Phần tử `<pre>` của **HTML** xác định văn bản được định dạng sẵn.
- `<pre>` cho phép hiển thị văn bản giống y với trong code
- **VD :**
    ```html
    <pre>
    My Bonnie lies over the ocean.

    My Bonnie lies over the sea.

    My Bonnie lies over the ocean.

    Oh, bring back my Bonnie to me.
    </pre>
    ```
    => Hiển thị trên trình duyệt :

    <img src=https://i.imgur.com/leEuORy.png>