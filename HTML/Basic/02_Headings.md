# Headings
## **1) Giới thiệu**
- Trong HTML có tất cả sáu thẻ đề mục từ `<h1>` cho tới `<h6>`
- Thẻ `<h1>` đánh dấu các đề mục quan trọng nhất và các thẻ còn lại từ `<h2>` tới `<h6>` cho các đề mục ít quan trọng hơn .
- Trình duyệt sẽ tự động thiết lập kích thước phông chữ và khoảng cách cho từng loại đề mục .
- **VD :**
    ```html
    <h1>Heading 1</h1>
    <h2>Heading 2</h2>
    <h3>Heading 3</h3>
    <h4>Heading 4</h4>
    <h5>Heading 5</h5>
    <h6>Heading 6</h6>
    ```
    => Hiển thị trên trình duyệt :

    <img src=https://i.imgur.com/v9NkAVz.png>

- **Headings** không chỉ có ý nghĩa giúp người dùng hiểu được nội dung tóm tắt của phần nội dung theo sau mà còn được các công cụ tìm kiếm như **Google**, **Yahoo** hay **Bing**.... sử dụng để phân tích nội dung , cấu trúc website cũng như đánh giá và so sánh các trang web khác nhau có nội dung viết về cùng một chủ đề . Do đó việc sử dụng các **headings** đề mục hợp lý là rất quan trọng .
## **2) Kích thước font cho Headings**
- Trình duyệt sẽ tự động thiết lập kích thước font của **headings** . 
- Tuy nhiên để chắc chắn **heading** của trang hiển thị với cùng một kích thước trên các trình duyệt khác nhau thì có thể thiết lập kích font cho chúng .
- Để quy định kích thước cho đề mục chúng ta có thể sử dụng thuộc tính `style` như sau :
    ```html
    <h1 style="font-size:60px;">Heading 1</h1>
## **3) Horizontal Rules**
- Thẻ `<hr>` sẽ định nghĩa 1 đường ngắt dòng trong trang **HTML** .
- Thường được sử dụng để phân chia các khối nội dung trong trang **HTML** .
- **VD :**
    ```html
    <h1>This is heading 1</h1>
    <p>This is some text.</p>
    <hr>
    <h2>This is heading 2</h2>
    <p>This is some other text.</p>
    <hr>
    ```
    => Hiển thị trên trình duyệt :

    <img src=https://i.imgur.com/DStK7LN.png>

## **4) Phần tử `<head>`**
- Phần tử `<head>` là một container chứa dữ liệu dạng thô ( **metadata** ) . **Metadata** làm nên nội dung của trang **HTML** và chúng sẽ không được hiển thị .
- Phần tử `<head>` sẽ được đặt giữa thẻ `<html>` và thẻ `<body>`
- **VD :**
    ```html
    <!DOCTYPE html>
    <html>

    <head>
    <title>My First HTML</title>
    <meta charset="UTF-8">
    </head>

    <body>
    ```
    => Hiển thị trên trình duyệt :

    <img src=https://i.imgur.com/vBnKeva.png>

