# CSS Border
## **1) CSS `border-style`**
- Thuộc tính `border-style` định nghĩa dạng border sẽ được hiển thị .
- Các kiểu `border-style` :
    
    <img src=https://i.imgur.com/h5X7mDf.png>

- **VD :**  
    ```html
    <style>
      p.dotted {border-style: dotted;}
    </style>
    <body>
     <p class="dotted">A dotted border.</p>
    </body>
    ```
    - Hiển thị trên trình duyệt :
        
        <img src=https://i.imgur.com/G5ytuJI.png>

## **2) CSS `border-width`**
- Thuộc tính `border-width` biểu thị chiều rộng của border .
- Chiều rộng này có thể được đặt theo các đơn vị (`px`, `pt`, `cm`, `em`...) hoặc theo 3 kích cỡ được định nghĩa trước : `thin`, `medium` và `thick` .
- Thuộc tính `border-width` có thể có từ `1` đến `4` giá trị ( cho `top-border`, `right-border`, `bottom-border`, `left-border` )
    ```css
    p.seven {
      border-style: solid;
      border-width: 2px 10px 4px 20px;
    }
    ```
    - Nếu không được khai báo đầy đủ các thông số trên, mặc định **CSS** sẽ hiểu :
        - `top-border` = `bottom-border`
        - `right-border` = `left-border`
- **VD :**
    ```html
    <style>
    p.seven {
      border-style: solid;
      border-width: 2px 10px 4px 20px;
    }
    </style>
    <p class="seven">Some text.</p>
    ```
    - Hiển thị trên trình duyệt :
        
        <img src=https://i.imgur.com/USOF1bA.png>

## **3) CSS `border-color`**
- Thuộc tính `border-color` dùng để đặt màu cho các border .
- Các màu có thể được gọi theo :
    - Tên màu - **VD :** `red`
    - Mã HEX - **VD :** `#ff0000`
    - Mã RGB - **VD :** `rgb(255,0,0)`
    - `transparent`
- Thuộc tính `border-color` cũng có thể có 4 giá trị ( cho `top-border`, `right-border`, `bottom-border`, `left-border` )
- Nếu thuộc tính `border-color` không được khai báo, nó sẽ tự kế thừa color của phần tử .
- **VD :**
    ```html
    <style>
    p.one {
      border-style: solid;
      border-color: red;
    }
    </style>
    <p class="one">A solid red border</p>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/wXZPPla.png>

## **4) CSS `border-style`**
- Có 2 cách sử dụng các thuộc tính style riêng biệt cho từng border trong 4 border .
- **Cách 1** :
    - `border-top-style` : border trên
    - `border-right-style` : border bên phải
    - `border-bottom-style` : border dưới
    - `border-right-style` :
    - **VD :**
        ```css
        p {
          border-top-style: dotted;
          border-right-style: solid;
          border-bottom-style: dotted;
          border-left-style: solid;
        }
        ```
        - Hiển thị trên trình duyệt :

            <img src=https://i.imgur.com/EhOFklM.png>

- **Cách 2** : Sử dụng thuộc tính `border-style` . Tương tự như cách dùng `border-width` , thuộc tính `border-style` có thể có từ `1` đến `4` giá trị ( cho `top-border`, `right-border`, `bottom-border`, `left-border` ) . Nếu không được khai báo đầy đủ các thông số trên, mặc định **CSS** sẽ hiểu :
    - `top-border` = `bottom-border`
    - `right-border` = `left-border`
    - **VD :**
        ```css
        p {
          border-style: dotted solid;
        }
        ```
## **5) CSS `border` - Rút ngắn code**
- Để rút ngắn code, có thể khai báo tất cả thông tin cho từng border (trong 4 border) trên dòng riêng biệt của chúng .
- Thuộc tính `border` có thể thêm thông tin các thuộc tính sau (cách này khai báo chung cho 4 đường border)
    - `border-width`
    - `border-style` ( bắt buộc )
    - `border-color`
    ```css
    p {
      border: 5px solid red;
    }
    ```
- Hoặc cũng có thể khai báo riêng cho từng border :
    ```css
    p {
      border-left: 6px solid red;
      background-color: lightgrey;
    }
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/E2q1IQX.png>

## **6) CSS `border-radius`**
- Thuộc tính `border-radius` được sử dụng để thêm các góc cong cho border .
- **VD :**
    ```html
    <style>
    p.round2 {
      border: 2px solid red;
      border-radius: 8px;
    }
    </style>
    <p class="round2">Rounder border</p>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/q1mox2p.png>

- Thuộc tính `border-radius` có thể có 4 giá trị ( cho `top-left corner`, `top-right corner`, `bottom-right corner`, `bottom-left corner` )

    <img src=https://i.imgur.com/5ufPbNZ.png>

- Nếu được khai báo 4 giá trị :
    ```css
    p {
      border-radius: 15px 50px 30px 5px;
    }
    ```
    <img src=https://i.imgur.com/SjEgrsO.png>

- Nếu được khai báo 3 giá trị :
    ```css
    p {
      border-radius: 15px 50px 30px;
    }
    ```
    <img src=https://i.imgur.com/yhIgFWN.png>

- Nếu được khai báo 2 giá trị :
    ```css
    p {
      border-radius: 15px 50px;
    }
    ```
    <img src=https://i.imgur.com/j1imGaU.png>

- Nếu được khai báo chỉ 1 giá trị :
    ```css
    p {
      border-radius: 15px;
    }
    ```
    <img src=https://i.imgur.com/O6SnylC.png>

