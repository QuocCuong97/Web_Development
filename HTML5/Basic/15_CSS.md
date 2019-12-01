# HTML CSS
## **1) CSS**
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

## **2) CSS Font**
- Thuộc tính `color` định nghĩa màu chữ được sử dụng .
- Thuộc tính `font-family` định nghĩa loại font được sử dụng .
- Thuộc tính `font-size` định nghĩa cỡ chữ được sử dụng .
- **VD :**
    ```html
    <!DOCTYPE html>
    <html>
    <head>
    <style>
    h1 {
      color: blue;
      font-family: verdana;
      font-size: 300%;
    }
    p  {
      color: red;
      font-family: courier;
      font-size: 160%;
    }
    </style>
    </head>
    <body>

    <h1>This is a heading</h1>
    <p>This is a paragraph.</p>

    </body>
    </html>
    ```
    - Hiển thị trên trình duyệt :
                
        <img src=https://i.imgur.com/vca7FwE.png>

## **3) CSS Border**
- Thuộc tính `border` định nghĩa đường viền bao quanh 1 phần tử html .
- **VD :** Chỉnh sửa đoạn code trên :
    ```html
    p  {
      color: red;
      font-family: courier;
      font-size: 160%;
      border: 1px solid black;
    }
    ```
    - Hiển thị trên trình duyệt :
                
        <img src=https://i.imgur.com/zYV44z5.png>
## **4) CSS Padding**
- Thuộc tính `padding` định nghĩa phần khoảng cách ( *padding* ) giữa chữ và đường viền ( *border* )
- **VD :** Chỉnh sửa đoạn code trên :
    ```html
    p  {
      color: red;
      font-family: courier;
      font-size: 160%;
      border: 1px solid black;
      padding: 30px;
    }
    ```
    - Hiển thị trên trình duyệt :
                
        <img src=https://i.imgur.com/FI8tnr1.png>

## **5) CSS Margin**
- Thuộc tính `margin` định nghĩa khoảng cách lề ( *margin* )
bên ngoài đường viền ( *border* )
- **VD :** Chỉnh sửa đoạn code trên :
    ```html
    p  {
      color: red;
      font-family: courier;
      font-size: 160%;
      border: 1px solid black;
      padding: 30px;
      margin: 50px;
    }
    ```
    - Hiển thị trên trình duyệt :
                
        <img src=https://i.imgur.com/yZu4vyr.png>

## **6) Thuộc tính `id`**
- Để định nghĩa một style đặc biệt cho một phần tử đặc biệt, thêm thuộc tính `id` vào phần **CSS** của phần tử đó .
- **VD :**
    ```html
    <!DOCTYPE html>
    <html>
    <head>
    <style>
    #p01 {
      color: blue;
    }
    </style>
    </head>
    <body>

    <p>This is a paragraph.</p>
    <p>This is a paragraph.</p>
    <p id="p01">I am different.</p>

    </body>
    </html>
    ```
    - Hiển thị trên trình duyệt :
                
        <img src=https://i.imgur.com/Uv6l3K2.png>

## **7) Thuộc tính `class`**
- Thuộc tính `class` cũng sử dụng gần giống với `id` , nhưng thường được dùng để phân loại các element có ý nghĩa khác nhau trong code .
- **VD :**
    ```html
    <!DOCTYPE html>
    <html>
    <head>
    <style>
    p.error {
      color: red;
    }
    </style>
    </head>
    <body>

    <p>This is a paragraph.</p>
    <p>This is a paragraph.</p>
    <p class="error">I am different.</p>
    <p>This is a paragraph.</p>
    <p class="error">I am different too.</p>

    </body>
    </html>
    ```
    - Hiển thị trên trình duyệt :
                
        <img src=https://i.imgur.com/HwCQ1cJ.png>

## **8) Cách gọi file `.css`**
- Gọi file `styles.css` từ một đường dẫn tuyệt đối ( có thể ở server local hoặc remote ) :
    ```html
    <link rel="stylesheet" href="https://www.w3schools.com/html/styles.css">
    ```
- Gọi file `styles.css` từ một đường dẫn tương đối ( nằm trong server local ) :
    ```html
    <link rel="stylesheet" href="/html/styles.css">
    ```
- Gọi file `styles.css` từ trong chính folder đang đứng ( chứa file `index.html` ) :
    ```html
    <link rel="stylesheet" href="styles.css">
    ```
    


    
