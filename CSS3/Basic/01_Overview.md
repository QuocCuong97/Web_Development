# Tổng quan về CSS
- **CSS** - **Cascading Style Sheets** dùng để tạo kiểu ( trang trí ) cho trang web .
- **HTML** tạo ra cấu trúc , khung sườn cho trang web trong khi đó **CSS** dùng để quy định các phần tử của trang **HTML** sẽ được hiển thị như thế nào .
- **CSS** có thể được thêm vào trang theo 3 cách khác nhau :
    - **Inline** : sử dụng thuộc tính `style` trong thẻ mở để thêm mã **CSS** cho phần tử .
        - **VD :** 
            ```html
            <h1 style="color:blue;">This is a Blue Heading</h1>
            ```
            - Hiển thị trên trình duyệt :

                <img src=https://i.imgur.com/V3o6K4w.png>
    - **Internal** : Sử dụng thẻ `<style>` để thêm mã **CSS** cho trang **HTML** .
        - **VD :**
            ```html
            <!DOCTYPE html>
            <html>
            <head>
            <style>
            body {background-color: powderblue;}
            h1   {color: blue;}
            p    {color: red;}
            </style>
            </head>
            <body>

            <h1>This is a heading</h1>
            <p>This is a paragraph.</p>

            </body>
            </html>
            ```
            - Hiển thị trên trình duyệt :

                <img src=https://i.imgur.com/jV7MOHp.png>
    - **External** : Sử dụng thẻ `<link>` để tham chiếu tới một file **CSS** bên ngoài . Lúc này code **CSS** sẽ tách biệt với code **HTML** . Đây là cách thường được sử dụng nhất .
        - **VD :**
            ```html
            <!--File index.html-->
            <!DOCTYPE html>
            <html>
            <head>
              <link rel="stylesheet" href="styles.css">
            </head>
            <body>

            <h1>This is a heading</h1>
            <p>This is a paragraph.</p>

            </body>
            </html>
            ```
            ```css
            <!--File styles.css-->
            body {
              background-color: orange;
            }
            h1 {
              color: blue;
            }
            p {
              color: red;
            }
            ```
            - Hiển thị trên trình duyệt :
                
                <img src=https://i.imgur.com/2lmCdBh.png>
