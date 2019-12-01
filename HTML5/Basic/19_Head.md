# Head
## **1) Phần tử `<head>`**
- Phần tử `<head>` là một container chứa các metadata và được đặt ở giữa thẻ `<html>` và thẻ `<body>` .
- HTML metadata là phần data về file HTML . Phần metadata này sẽ không được hiển thị trên trình duyệt .
- Metadata thường định nghĩa tiêu đề, charset, styles, scripts, và các thông tin meta khác .
- Các thẻ mô tả metadata : `<title>`, `<style>`, `<meta>`, `<link>`, `<script>` và `<base>` .
## **2) Phần tử `<title>`**
- Phần tử `<title>` định nghĩa title cho một văn bản HTML, và nó được yêu cầu cho mọi văn bản HTML .
- Phần tử `<title>` :
    - Định nghĩa tiêu đề hiển thị trên tab của trình duyệt .
    - Cung cấp tiêu đề cho trang khi trang được thêm vào mục yêu thích trong trình duyệt ( favorites )
    - Hiển thị tiêu đề cho trang trong các kết quả của các nguồn tìm kiếm .
- Cấu trúc một văn bản HTML bình thường :
    ```html
    <!DOCTYPE html>
    <html>

    <head>
    <title>Page Title</title>
    </head>

    <body>
    The content of the document......
    </body>

    </html>
    ```
    - Hiển thị trên trình duyệt :
        
        <img src=https://i.imgur.com/ZThAKba.png>

## **3) Phần tử `<style>`**
- Phần tử `<style>` được sử dụng để định nghĩa style cho một trang HTML .
- **VD :**
    ```html
    <style>
      body {background-color: powderblue;}
      h1 {color: red;}
      p {color: blue;}
    </style>
    ```
## **4) Phần tử `<link>`**
- Phần tử `<link>` khi đặt trong `<head>` sẽ sử dụng để link đến 1 file `.css`
- **VD :**
    ```html
    <link rel="stylesheet" href="mystyle.css">
    ```
## **5) Phần tử `<meta>`**
- Phần tử `<meta>` được sử dụng để chỉ định bộ ký tự ( **charset** ) được sử dụng, mô tả, các keywords, tác giả và các metadata khác .
- Metadata được sử dụng bởi trình duyệt ( khi hiển thị nội dung ), bởi các công cụ tìm kiếm ( sử dụng các keywords ) và các dịch vụ web khác .
- Định nghĩa **charset** :
    ```html
    <meta charset="UTF-8">
    ```
- Định nghĩa mô tả của trang web :
    ```html
    <meta name="description" content="Học HTML">
    ```
- Định nghĩa các **keywords** dùng cho các công cụ tìm kiếm :
    ```html
    <meta name="keywords" content="HTML, CSS, XML, JavaScript">
    ```
- Định nghĩa tác giả của trang web :
    ```html
    <meta name="author" content="Quoc Cuong">
    ```
- Refresh trang web mỗi `30s` :
    ```html
    <meta http-equiv="refresh" content="30">
    ```
## **6) Viewport**
- **HTML5** giới thiệu một phương thức cho phép các web designer kiểm soát **viewport**, thông qua thẻ `<meta>` .
- **Viewport** là khu vực mà người dùng có thể nhìn thấy của trang web . Nó sẽ rất đa dạng trên các loại thiết bị , trên smartphone thì sẽ nhỏ hơn là trên máy tính .
- Nên bao gồm phần tử `<meta>` **viewport** trên tất cả các trang web :
    ```html
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    ```
- Phần tử `<meta>` **viewport** chỉ dẫn cho trình duyệt cách để kiểm soát kích thước và tỷ lệ của trang .
- Phần thông số `width=device-width` đặt độ rộng của trang phụ thuộc vào độ rộng màn hình của thiết bị .
- Phần thông số `initial-scale=1.0` đặt mức thu phóng ( **zoom** ) khi trang được load lần đầu bởi trình duyệt .
- **VD :** Trường hợp có và không có **viewport** :

    <img src=https://i.imgur.com/YmV6X3p.png>

## **7) Phần tử `<script>`**
- Phần tử `<script>` dùng để định nghĩa khối code **JavaScript** .
## **8) Phần tử `<base>`**
- Phần tử `<base>` chỉ định URL cơ sở và target cơ sở cho các đường dẫn tương đối bên trong page :
    ```html
    <base href="https://techrum.vn" target="_blank">

> ### **Có được bỏ sót các thẻ `<html>`, `<head>`, `<body>`**
- Theo tiêu chuẩn **HTML5**, các thẻ `<html>`, `<body>` và `<head>` có thể được bỏ qua nếu không muốn viết .
- **VD :**
    ```html
    <!DOCTYPE html>
    <title>Page Title</title>

    <h1>This is a heading</h1>
    <p>This is a paragraph.</p>
    ```