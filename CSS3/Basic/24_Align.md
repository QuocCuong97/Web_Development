# CSS Layout - Horizontal & Vertical Align
## **1) Center Align Elements**
- Để căn chỉnh theo chiều ngang cho 1 phần tử block ( như `<div>` ), sử dụng thuộc tính "`margin: auto;`" .
- Set chiều rộng cho phần tử ( thuộc tính `width` ) sẽ tránh cho phần tử không bị dãn ra dìa của phần tử chứa nó .
- Sau khi set thuộc tính `width`, phần tử sẽ chiếm đúng phần chiều rộng của nó, phần không gian còn lại sẽ được chia đều cho 2 bên margin .
- **VD :**
    ```css
    .center {
      margin: auto;
      width: 50%;
      border: 3px solid green;
      padding: 10px;
    }
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/QLiPIvv.png>

## **2) Center Align Text**
- Để căn chỉnh giữa cho 1 đoạn text trong 1 phần tử, sử dụng thuộc tính "`text-align: center;`"
- **VD :**
    ```css
    .center {
      text-align: center;
      border: 3px solid green;
    }
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/DbRu3jZ.png>

## **3) Center an Image**
- Để căn chỉnh giữa cho một hình ảnh, set "`margin-left: auto;`" và "`margin-right: auto;`" và đặt nó trong 1 phần tử block :
- **VD :**
    ```html
    <style>
    img {
      display: block;
      margin-left: auto;
      margin-right: auto;
      width: 40%;
    }
    </style>
    <body>
      <img src="paris.jpg" alt="Paris" style="width:40%">
    </body>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/0lgx4Wc.png>

## **4) Left and Right Align - sử dụng `position`**
- Sử dụng thuộc tính "`position: absolute;`"
- **VD :**
    ```html
    <style>
    .right {
      position: absolute;
      right: 10px;
      width: 300px;
      border: 3px solid #73AD21;
      padding: 10px;
    }
    </style>
    <div class="right">
      <p>In my younger and more vulnerable years my father gave me some advice that I've been turning over in my mind ever since.</p>
    </div>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/CFimgL4.png>

## **5) Left and Right Align - sử dụng `float`**
- Có thể sử dụng phương pháp khác để căn chỉnh cho phần tử bằng thuộc tính `float` .
- **VD :**
    ```html
    <style>
    .right {
      float: right;
      width: 300px;
      border: 3px solid #73AD21;
      padding: 10px;
    }
    </style>
    <div class="right">
      <p>In my younger and more vulnerable years my father gave me some advice that I've been turning over in my mind ever since.</p>
    </div>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/CFimgL4.png>

## **6) Căn chỉnh bằng `overflow` - clearfix**
- Có thể thêm thuộc tính "`overflow: auto;`" vào phần tử cha để fix :
- **VD :**
    - Không sử dụng clearfix :

        <img src=https://i.imgur.com/Iwp8rXO.png>

    - Sử dụng clearfix :
        ```html
        <style>
        .clearfix {
          overflow: auto;
        }
        .img2 {
          float: right;
        }
        </style>
        <div class="clearfix">
          <img class="img2" src="pineapple.jpg" alt="Pineapple" width="170" height="170">
        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus imperdiet, nulla et dictum interdum...
        </div>
        ```
        <img src=https://i.imgur.com/h6StaJp.png>

## **7) Căn chỉnh  - sử dụng `padding`**
- Một cách đơn giản nhất để căn chỉnh bên trong phần tử là sử dụng `padding` .
- **VD :**
    ```css
    .center {
      padding: 70px 0;
      border: 3px solid green;
    }
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/hY79aWO.png>

## **8) Căn chỉnh - sử dụng `line-height`**
- Một thủ thuật khác là sử dụng thuộc tính `line-height` với giá trị bằng với giá trị của thuộc tính `height` .
- **VD :**
    ```css
    .center {
      line-height: 200px;
      height: 200px;
      border: 3px solid green;
      text-align: center;
    }

    /* If the text has multiple lines, add the following: */
    .center p {
      line-height: 1.5;
      display: inline-block;
      vertical-align: middle;
    }
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/hY79aWO.png>

## **9) Căn chỉnh - sử dụng `position` và `transform`**
- **VD :**
    ```css
    .center {
      height: 200px;
      position: relative;
      border: 3px solid green;
    }
    .center p {
      margin: 0;
      position: absolute;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
    }
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/hY79aWO.png>