# CSS Fonts
## **1) Các kiểu font trong CSS**
- Các thuộc tính về font trong **CSS** khai báo về họ font, độ đậm, cỡ chữ, kiểu chữ .
- Trong **CSS** , có 2 dạng **font-family** ( họ font ) :
    - **generic family** - là một nhóm các **font-family** có kiểu nét nhìn giống nhau .
        <img src=https://i.imgur.com/F9GcYip.png>
    - **font-family** - là một **font-family** riêng (bộ font riêng)
- Bảng phân loại font :

    | Generic-Family | Font-Family | Mô tả |
    |----------------|-------------|-------|
    | **Serif** | <code style="font-family:'Times New Roman', Times, serif;">Times New Roman</code><br><code style="font-family:'Georgia', Times, serif;">Georgia</code> | Font **serif** có nét nhỏ và chân ngang ở cuối các ký tự |
    | **Sans-serif** | <code style="font-family:'Arial', Helvetica, sans-serif;">Arial</code><br><code style="font-family:Verdana, Geneva, sans-serif;">Verdana</code> | Font **sans** có nghĩa là font không có chân ngang ở cuối ký tự |
    | **Monospace** | <code style="font-family:'Courier New', Courier, monospace;">Courier New</code><br><code style="font-family:'Lucida Console', Monaco, monospace;">Lucida Console</code> | Tất cả các ký tự trong các font **monospace** đều có độ rộng giống nhau |

## **2) CSS `font-family`**
- **Font-family** của một đoạn text được set bằng thuộc tính `font-family` .
- Thuộc tính `font-family` phải giữ một vài font chữ như một hệ thống dự phòng . Nếu trình duyệt không hỗ trợ font thứ nhất, nó sẽ tự chuyển sang font tiếp theo . 
- Gọi **font-family** bắt đầu bằng font muốn gọi , kết thúc bằng **generic-family** để trình duyệt sẽ chọn các font tương tự trong **generic family** font đang gọi không được hỗ trợ .
    >Nếu tên của **font-family** muốn gọi nhiều hơn 1 từ, cần phải đặt trong dấu ngoặc ( **VD :** '`Times New Roman`' )
- **Web Safe Font Combinations** :
    - **Serif** :

      <table style="width:100%">
      <tr>
        <th>font-family</th>
        <th>Ví dụ</th>
      </tr>
      <tr>
        <td>Georgia, serif</td>
        <td><h2 style="font-family:Georgia, Times, serif;">This is a heading</h2></td>
      </tr>
      <tr>
        <td>'Palatino Linotype', 'Book Antiqua', Palatino, serif</td>
        <td><h2 style="font-family:'Palatino Linotype', 'Book Antiqua', Palatino, serif;">This is a heading</h2></td>
      </tr>
      <tr>
        <td>'Times New Roman', Times, serif</td>
        <td><h2 style="font-family:'Times New Roman', Times, serif;">This is a heading</h2></td>
    </table>




        <!-- | font-family | Ví dụ |
        |-------------|-------|
        | `Georgia, serif` | <h2 style="font-family:Georgia, Times, serif;">This is a heading</h2> |
        | `'Palatino Linotype', 'Book Antiqua', Palatino, serif` | <h2 style="font-family:'Palatino Linotype', 'Book Antiqua', Palatino, serif;">This is a heading</h2> |
        | `'Times New Roman', Times, serif` | <h2 style="font-family:'Times New Roman', Times, serif;">This is a heading</h2> | -->

    - **Sans-serif** :
        
        | font-family | Ví dụ |
        |-------------|-------|
        | `Arial, Helvetica, sans-serif` | <h2 style="font-family:Arial, Helvetica, sans-serif;">This is a heading</h2> |
        | `'Arial Black', Gadget, sans-serif` | <h2 style="font-family:'Arial Black', Gadget, sans-serif;">This is a heading</h2> |
        | `'Comic Sans MS', cursive, sans-serif` | <h2 style="font-family:'Comic Sans MS', cursive, sans-serif;">This is a heading</h2> |
        | `Impact, Charcoal, sans-serif` | <h2 style="font-family:Impact, Charcoal, sans-serif;">This is a heading</h2> |
        | `'Lucida Sans Unicode', 'Lucida Grande', sans-serif` | <h2 style="font-family:'Lucida Sans Unicode', 'Lucida Grande', sans-serif;">This is a heading</h2> |
        | `Tahoma, Geneva, sans-serif` | <h2 style="font-family:Tahoma, Geneva, sans-serif;">This is a heading</h2> |
        | `'Trebuchet MS', Helvetica, sans-serif` | <h2 style="font-family:'Trebuchet MS', Helvetica, sans-serif;">This is a heading</h2> |
        | `Verdana, Geneva, sans-serif` | <h2 style="font-family:Verdana, Geneva, sans-serif;">This is a heading</h2> |

    - **Monospace** :

        | font-family | Ví dụ |
        |-------------|-------|
        | `'Courier New', Courier, monospace` | <h2 style="font-family:'Courier New', Courier, monospace;">This is a heading</h2> |
        | `'Lucida Console', Monaco, monospace` | <h2 style="font-family:'Lucida Console', Monaco, monospace;">This is a heading</h2> |

- **Google Fonts** :
    - [Tìm hiểu thêm](https://www.w3schools.com/howto/howto_google_fonts.asp)
- **VD :**
    ```html
    <style>
    p.serif {
      font-family: "Times New Roman", Times, serif;
    }
    p.sansserif {
      font-family: Arial, Helvetica, sans-serif;
    }
    </style>
    <p class="serif">This is a paragraph, shown in the Times New Roman font.</p>
    <p class="sansserif">This is a paragraph, shown in the Arial font.</p>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/04TXFOn.png>

## **3) CSS `font-size`**
- Thuộc tính `font-size` set kích cỡ cho text .
- Cách kiểm soát kích thước font rất quan trọng trong thiết kế web . Tuy nhiên, không nên cân chỉnh một đoạn paragraph để nó trông to như headings, cũng không nên cân chỉnh một headings để nhìn như một đoạn paragraph .
- Luôn sử dụng chính xác tag **HTML** cho văn bản , như `<h1>` - `<h6>` cho headings và `<p>` cho paragraph .
- Giá trị `font-size` có thể là kích cỡ tuyệt đối hoặc tương đối .
- Kích cỡ tuyệt đối :
    - Set kích cỡ text theo kích cỡ định sẵn
    - Không cho phép user thay đổi kích cỡ tron gtaast cả các trình duyệt 
    - Kích cỡ tuyệt đối rất hữu ích khi kích cỡ của phần output được biết trước .
- Kích cỡ tương đối :
    - Set kích cỡ text phụ thuộc vào các phần tử xung quanh .
    - Cho phép user thay đổi kích cỡ chữ trong trình duyệt .
- Nếu thuộc tính `font-size` không được khai báo, kích cỡ mặc định của 1 đoạn text bình thường trong paragraph là `16px` (=`1em`)
### **3.1) Đặt `font-size` với đơn vị `px`**
- Đặt kích cỡ font bằng `pixels` cho phép người lập trình kiểm soát hoàn toàn kích cỡ chữ .
- Nếu sử dụng `pixels` , vẫn có thể sử dụng công cụ zoom trên trình duyệt để phóng to/thu nhỏ toàn bộ trang web .
- **VD :**
    ```css
    h1 {
    font-size: 40px;
    }
    h2 {
    font-size: 30px;
    }
    p {
    font-size: 14px;
    }
    ```
### **3.2) Đặt `font-size` với đơn vị `em`**
- Để cho phép user có thể thay đổi kích cỡ chữ ( trong menu của trình duyệt ), nhiều lập trình viên sử dụng đơn vị `em` thay cho `pixel` .
- Đơn vị `em` được **W3C** khuyến nghị .
- Kích cỡ mặc định của chữ trong trình duyệt là `16px = 1em` .
- Kích cỡ font có thể được tính toán từ `pixel` sang `em` bằng công thức :
    ```
    em = pixels/16
    ```
- **VD :**
    ```css
    h1 {
      font-size: 2.5em; /* 40px/16=2.5em */
    }
    h2 {
      font-size: 1.875em; /* 30px/16=1.875em */
    }
    p {
      font-size: 0.875em; /* 14px/16=0.875em */
    }
    ```
### **3.3) Sử dụng kết hợp giữa `%` và `em`**
- Giải pháp hữu dụng trên tất cả các trình duyệt là set `font-size` mặc định theo `%` trên phần tử `<body>` :
    ```css
    body {
    font-size: 100%;
    }
    h1 {
    font-size: 2.5em;
    }
    h2 {
    font-size: 1.875em;
    }
    p {
    font-size: 0.875em;
    }
    ```
### **3.4) Reponsive `font-size`**
- Kích cỡ font có thể được đặt với đơn vị `vw` - **viewport width** .
- Cách này sẽ giúp font chữ tự động phù hợp với kích cỡ của trình duyệt :
- **VD :**
    ```html
    <h1 style="font-size:10vw">Hello World</h1>
    ```
## **4) CSS `font-style`**
- Thuộc tính `font-style` phần lớn được sử dụng để khai báo chữ ngiêng ( ***italic*** )
- Thuộc tính này có 3 giá trị :
    - `normal` - Text được hiển thị bình thường
    - `italic` - Text được hiển thị chữ nghiêng
    - `oblique` - Dạng hiển thị tương tự chữ nghiêng, nhưng ít được hỗ trợ
- **VD :**
    ```html
    <style>
    p.normal {
      font-style: normal;
    }
    p.italic {
      font-style: italic;
    }
    p.oblique {
      font-style: oblique;
    }
    </style>
    <p class="normal">This is a paragraph in normal style.</p>
    <p class="italic">This is a paragraph in italic style.</p>
    <p class="oblique">This is a paragraph in oblique style.</p>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/6sNEE1Y.png>

## **5) CSS `font-weight`**
- Thuộc tính `font-weight` khai báo độ đậm của chữ :
- Thuộc tính này có 2 giá trị :
    - `normal` : chữ thường
    - `light` : chữ thường
    - `bold` : chữ đậm
    - `number` : tùy chỉnh độ đậm theo số
- **VD :**
    ```html
    <style>
    p.normal {
      font-weight: normal;
    }
    p.light {
      font-weight: lighter;
    }
    p.thick {
      font-weight: bold;
    }
    p.thicker {
      font-weight: 900;
    }
    </style>
    <p class="normal">This is a paragraph.</p>
    <p class="light">This is a paragraph.</p>
    <p class="thick">This is a paragraph.</p>
    <p class="thicker">This is a paragraph.</p>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/G2498vC.png>



    




        