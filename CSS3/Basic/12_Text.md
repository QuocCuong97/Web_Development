# CSS Text
## **1) CSS text `color`**
- Thuộc tính `color` được sử dụng để đặt màu sắc cho text trong phần tử .
- Các màu có thể được gọi theo :
    - Tên màu - **VD :** `red`
    - Mã HEX - **VD :** `#ff0000`
    - Mã RGB - **VD :** `rgb(255,0,0)`
- Màu text mặc định của một trang sẽ được định nghĩa ở phần tử `body` :
    ```css
    body {
      color: blue;
    }

    h1 {
      color: green;
    }
    ```
## **2) CSS `text-align`**
- Thuộc tính `text-align` được sử dụng để cân chỉnh theo chiều ngang cho text .
- 1 đoạn text có thể được căn chỉnh theo lề trái (`left`), theo lề phải (`right`) , căn chỉnh giữa (`center`) hoặc căn chỉnh dàn chữ 2 bên (`justify`) ,
- **VD1 :**
    ```css
    h1 {
      text-align: center;
    }

    h2 {
      text-align: left;
    }

    h3 {
      text-align: right;
    }
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/Gw9rcoT.png>

- **VD2 :** Khi thuộc tính `text-align` được set giá trị "`justify`", mỗi dòng trong đoạn text sẽ được dãn ra sao có các dòng đều có cùng chiều rộng, lề trái và lề phải đều thẳng hàng ( giống các bài báo và các bài tạp chí )
    ```css
    div {
      text-align: justify;
    }
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/WqEAYFN.png>

## **3) CSS `text-decoration`**
- Thuộc tính `text-decoration` được sử dụng để trang trí hoặc gỡ bỏ phần trang trí cho text .
- Giá trị "`text-decoration: none;`" trong thực tế thường dùng để xóa dấu gạch chân ở dưới link :
    ```css
    a.und {
      text-decoration: none;
    }
    ```
    - Hiển thị trên trình duyệt :
        
        <img src=https://i.imgur.com/3oI4AAu.png>
- Các giá trị khác để trang trí text :
    - `overline`
    - `line-through`
    - `underline`
- **VD :**
    ```css
    h1 {
      text-decoration: overline;
    }
    h2 {
      text-decoration: line-through;
    }
    h3 {
      text-decoration: underline;
    }
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/H7knRXI.png>

## **4) CSS `text-transform`**
- Thuộc tính `text-transform` được sử dụng đề chuyển hóa đoạn text thành dạng chữ hoa hoặc chữ thường .
- Có 3 dạng chữ chuyển hóa :
    - `uppercase` : VIẾT HOA
    - `lowercase` : viết thường
    - `capitalize` : Viết Hoa Chữ Cái Đầu Của Mỗi Từ
- **VD :**
    ```html
    <style>
    p.uppercase {
      text-transform: uppercase;
    }

    p.lowercase {
      text-transform: lowercase;
    }

    p.capitalize {
      text-transform: capitalize;
    }
    </style>
    <p class="uppercase">This is some text.</p>
    <p class="lowercase">This is some text.</p>
    <p class="capitalize">This is some text.</p>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/PBtVgkX.png>

## **5) CSS `text-indent`**
- Thuộc tính `text-indent` được sử dụng để khai báo phần thụt đầu dòng của dòng đầu tiên trong đoạn text .
- **VD :**
    ```html
    <style>
    p {
      text-indent: 50px;
    }
    </style>
    <p>In my younger and more vulnerable years my father gave me some advice that I've been turning over in my mind ever since. 'Whenever you feel like criticizing anyone,' he told me, 'just remember that all the people in this world haven't had the advantages that you've had.'</p>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/NaWTZRH.png>

## **6) CSS `letter-spacing`**
- Thuộc tính `letter-spacing` được sử dụng để khai báo khoảng cách giữa các ký tự trong 1 đoạn text .
- **VD :**
    ```html
    <style>
    h1 {
      letter-spacing: 3px;
    }
    h2 {
      letter-spacing: -3px;
    }
    </style>
    <h1>This is heading 1</h1>
    <h2>This is heading 2</h2>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/IiySe9n.png>

## **7) CSS `line-height`**
- Thuộc tính `line-height` được sử dụng để khai báo khoảng cách giữa các dòng trong đoạn text .
- Khoảng cách giữa các dòng bằng :
    `khoảng_cách_tiêu_chuẩn * line-height`
- **VD :**
    ```html
    <style>
    p.small {
      line-height: 0.7;
    }
    p.big {
      line-height: 1.8;
    }
    </style>
    <p class="small">
    This is a paragraph with a smaller line-height.<br>
    This is a paragraph with a smaller line-height.<br>
    </p>
    <p class="big">
    This is a paragraph with a bigger line-height.<br>
    This is a paragraph with a bigger line-height.<br>
    </p>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/LHYuQf9.png>

## **8) CSS text `direction`**
- Thuộc tính `direction` sử dụng để thay đổi hướng hiển thị của đoạn text trong phần tử .
- **VD :**
    ```css
    p {
      direction: rtl;
    }
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/lsSRffx.png>
## **9) CSS `word-spacing`**
- Thuộc tính `word-spacing` được sử dụng để khai báo khoảng cách giữa các từ trong đoạn text .
- **VD :**
    ```css
    h1 {
      word-spacing: 10px;
    }
    h2 {
      word-spacing: -5px;
    }
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/ZCfKWuF.png>

## **10) CSS `text-shadow`**
- Thuộc tính `text-shadow` sẽ thêm phần bóng (shadow) vào text .
- Cú pháp :
    ```css
    text-shadow: horizontal-shadow vertical-shadow shadow-color
    ```
- **VD :**
    ```css
    h1 {
      text-shadow: 3px 2px red;
    }
    ```
    - Hiển thị trên trình duyệt :
        
        <img src=https://i.imgur.com/to7H4el.png>

