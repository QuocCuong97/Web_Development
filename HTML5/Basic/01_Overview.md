# Tổng quan về HTML
## **1) Giới thiệu** <img src=https://i.imgur.com/wAv1sLp.png align=right width=35%>
- **HTML** - **Hyper Text Markup Language** ( *ngôn ngữ đánh dấu siêu văn bản* ) là ngôn ngữ tiêu chuẩn để tạo nên một trang web .
- Lịch sử phát triển :
    - **HTML** - `1991`
    - **HTML 2.0** - `1995`
    - **HTML 3.2** - `1997`
    - **HTML 4.01** - `1999`
    - **XHTML** - `2000`
    - **HTML5** - `2014`
- Một trang **HTML** tương ứng sẽ tạo ra nội dung của một trang web.
- Cấu trúc một trang **HTML** :

    <img src=https://i.imgur.com/70HJNj8.png>
- Trang**HTML** được lưu dưới dạng 1 file text với đuôi `.html` hoặc `.htm`
- **VD :** 1 file `.html`
    ```html
    <!DOCTYPE html>
    <html>
    <head>
    <title>Page Title</title>
    </head>
    <body>

    <h1>My First Heading</h1>
    <p>My first paragraph.</p>

    </body>
    </html>
    ```
- Hiển thị trang **HTML** (render HTML) là việc sử dụng một phần mềm như trình duyệt web để chuyển đọc và phần tích ý nghĩa các thẻ sau đó hiển thị ra nội dung trang tương ứng. 
- Ví dụ với đoạn mã HTML như trên sẽ được hiển thị như sau trên trình duyệt.

    <img src=https://i.imgur.com/CcO3tQm.png>

## **2) Thẻ HTML**
- **HTML** mô tả cấu trúc của một trang web sử dụng các thẻ đánh dấu ( ***markup tag*** ) hay còn gọi là **thẻ HTML** .
- **Thẻ** là một phần quan trọng trong **HTML** . Mỗi **thẻ HTML** được dùng để đánh dấu những nội dung khác nhau ví dụ như **thẻ đề mục** để đánh dấu **đề mục** , **thẻ văn bản** để đánh dấu văn bản thông thường , **thẻ hình ảnh** để đánh dấu hình ảnh.... Trình duyệt sẽ không hiển thị mã HTML thô (các thẻ) mà thay vào đó sẽ dựa trên từng loại thẻ để chuyển đổi sang các nội dung tương ứng của trang web .
- Mỗi thẻ khác nhau sẽ đánh dấu nội dung với ý nghĩa khác nhau.
- Thẻ gồm tên thẻ và bao quanh bởi cặp dấu `<>` . Mỗi thẻ HTML thường đi theo cặp bao gồm thẻ mở (opening tag) `<tag_name>` và thẻ đóng (closing tag) `</tag_name>` :
    ```html
    <tag_name>Nội dung bên trong thẻ</tag_name>
    ```
- Thẻ tự đóng (self-closing tag) là thẻ HTML với chỉ thẻ mở và không có thẻ đóng đi kèm . **VD :** thẻ `<br>` - thẻ xuống dòng
## **3) Khai báo `<!DOCTYPE>`**
- Khai báo `<!DOCTYPE>` đại diện cho định dạng văn bản , giúp trình duyệt hiển thị trang web chuẩn hơn .
- `<!DOCTYPE>` chỉ xuất hiện 1 lần ở đầu file .
    ```html
    <!DOCTYPE html>
    ....
    </html>
    ```