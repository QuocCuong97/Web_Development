# Text Typography
## **1) Font chữ mặc định của Bootstrap 4**
- **Bootstrap4** sử dụng `font-size` mặc định là `16px` , `line-height` là `1.5`
- Thuộc tính `font-family` mặc định là "`'Helvetica Neue', Helvetica, Arial, sans-serif`" .
- Các phần tử `<p>` có `margin-top = 0` và `margin-bottom = 1rem` ( `16px` ) .
## **2) Font chữ mặc định của một số phần tử HTML**
### **2.1) `<h1> - <h6>`**
- **Bootstrap4** định kiểu **HTML heading** ( `<h1> - <h6>` ) với font chữ đậm dần và cỡ chữ tăng dần .
- **VD :**
    ```html
    <div class="container">
      <h1>h1 Bootstrap heading (2.5rem = 40px)</h1>
      <h2>h2 Bootstrap heading (2rem = 32px)</h2>
      <h3>h3 Bootstrap heading (1.75rem = 28px)</h3>
      <h4>h4 Bootstrap heading (1.5rem = 24px)</h4>
      <h5>h5 Bootstrap heading (1.25rem = 20px)</h5>
      <h6>h6 Bootstrap heading (1rem = 16px)</h6>
    </div>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/4aVWckZ.png>
### **2.2) Display Headings**
- Các **display heading** được sử dụng để làm nổi bật hơn các **heading** thông thường ( cỡ chữ lớn hơn và chữ mảnh hơn ) .
- Có `4` class với cỡ chữ giảm dần : "`.display-1`", "`.display-2`", "`.display-3`", "`.display-4`"
- **VD :**
    ```html
    <div class="container">
      <h1>Display Headings</h1>
      <h1 class="display-1">Display 1</h1>
      <h1 class="display-2">Display 2</h1>
      <h1 class="display-3">Display 3</h1>
      <h1 class="display-4">Display 4</h1>
    </div>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/bMzEDsY.png>
### **2.3) Phần tử `<small>`**
- Trong **HTML**, phần tử `<small>` được dùng để tạo ra các đoạn text có chiều cao bằng với **heading** , nhưng nét chữ mảnh hơn .
- **VD :**  
    ```html
    <div class="container"> 
      <h1>h1 heading <small>secondary text</small></h1>
      <h2>h2 heading <small>secondary text</small></h2>
      <h3>h3 heading <small>secondary text</small></h3>
      <h4>h4 heading <small>secondary text</small></h4>
      <h5>h5 heading <small>secondary text</small></h5>
      <h6>h6 heading <small>secondary text</small></h6>
    </div>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/65tp57z.png>
### **2.4) Phần tử `<mark>`**
- **Bootstrap4** định kiểu phần tử `<mark>` của **HTML** với background màu vàng và một ít padding .
- **VD :**
    ```html
    <div class="container">   
      <p>Use the mark element to <mark>highlight</mark> text.</p>
    </div>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/PrxWfCW.png>

### **2.5) Phần tử `<abbr>`**
- **Bootstrap4** định kiểu phần tử `<abbr>` với một đường chấm gạch chân .
- **VD :**
    ```html
    <div class="container">
      <p>The <abbr title="World Health Organization">WHO</abbr> was founded in 1948.</p>
    </div>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/RqA22T3.png>
### **2.6) Phần tử `<blockquote>`**
- Thêm class "`.blockquote`" vào phần tử `<blockquote>` để chú thích cho phần nội dung đến từ nguồn khác .
- **VD :**
    ```html
    <div class="container">
      <blockquote class="blockquote">
        <p>For 50 years, WWF has been protecting the future of nature. The world's leading conservation organization, WWF works in 100 countries and is supported by 1.2 million members in the United States and close to 5 million globally.</p>
        <footer class="blockquote-footer">From WWF's website</footer>
      </blockquote>
    </div>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/IPdTFJE.png>
### **2.7) Phần tử `<dl>`**
- **Bootstrap4** định kiểu phần tử `<dl>` theo cách sau :
    ```html
    <div class="container">
    <h1>Description Lists</h1>    
      <p>The dl element indicates a description list:</p>
      <dl>
        <dt>Coffee</dt>
        <dd>- black hot drink</dd>
        <dt>Milk</dt>
        <dd>- white cold drink</dd>
      </dl>     
    </div>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/sodhMoU.png>

### **2.8) Phần tử `<code>`**
- **Bootstrap4** sẽ định kiểu cho phần tử `<code>` theo cách sau :
    ```html
    <div class="container">
      <p>The following HTML elements: <code>span</code>, <code>section</code>, and <code>div</code> defines a section in a document.</p>
    </div>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/87Ftosd.png>

### **2.9) Phần tử `<kbd>`**
- **Bootstrap4** sẽ định kiểu cho phần tử `<kbd>` theo cách sau :
    ```html
    <div class="container">
      <p>Use <kbd>ctrl + p</kbd> to open the Print dialog box.</p>
    </div>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/siR3DZA.png>
### **2.10) Phần tử `<pre>`**
- **Bootstrap4** sẽ định kiểu cho phần tử `<pre>` theo cách sau :
    ```html
    <div class="container">
    <p>For multiple lines of code, use the pre element:</p>
    <pre>
    Text in a pre element
    is displayed in a fixed-width
    font, and it preserves
    both      spaces and
    line breaks.
    </pre>
    </div>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/0ervgtx.png>
## **3) Các class khác**
- `.font-weight-bold` : chữ đậm
- `.font-weight-bolder` : chữ đậm hơn
- `.font-weight-normal` : chữ thường
- `.font-weight-light` : chữ mảnh
- `.font-weight-lighter` : chữ mảnh hơn
- `.font-italic` : chữ nghiêng 
    ```html
    <div class="container">
      <p class="font-weight-bold">Bold text.</p>
      <p class="font-weight-bolder">Bolder text.</p>
      <p class="font-weight-normal">Normal weight text.</p>
      <p class="font-weight-light">Light weight text.</p>
      <p class="font-weight-lighter">Lighter weight text.</p>
      <p class="font-italic">Italic text.</p>
    </div>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/Bg2K0Lm.png>

- `.lead` : làm cho chữ nổi bật hơn :
    ```html
    <div class="container">
      <p class="lead">This paragraph stands out.</p>
      <p>This is a regular paragraph.</p>
    </div>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/Z4Mq70l.png>
- `.small` : thu nhỏ cỡ chữ bình thường xuống `80%`
    ```html
    <div class="container">
      <p class="small">This paragraph is smaller.</p>
      <p>This is a regular paragraph.</p>
    </div>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/LFjVDcH.png>

- `.text-left` : căn chỉnh chữ vào bên trái container
- `.text-right` : căn chỉnh chữ vào bên phải container
- `.text-center`  : căn chỉnh chữ vào giữa container
- `.text-justify` : căn chỉnh chữ tự hiển thị cân bằng 2 bên
- `.text-nowrap` : căn chỉnh không wrap chữ 
    ```html
    <div class="container">
      <p class="text-left">Left-aligned text.</p>
      <p class="text-right">Right-aligned text.</p>      
      <p class="text-center">Center-aligned text.</p>
      <p class="text-justify">Justified text. Justified text. Justified text. Justified text. Justified text. Justified text.</p>      
      <p class="text-nowrap">No wrap text. No wrap text. No wrap text. No wrap text. No wrap text. No wrap text. No wrap text</p>   
    </div>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/7ah6hSY.png>

- `.text-*-left` : căn chỉnh chữ sang trái kết hợp chọn kiểu container ( `*` là một trong các giá trị `sm` , `md` , `lg` , `xl`)
- `.text-*-right` : căn chỉnh chữ sang phải kết hợp chọn kiểu container ( `*` là một trong các giá trị `sm` , `md` , `lg` , `xl`)
- `.text-*-center` : căn chỉnh chữ ở giữa kết hợp chọn kiểu container ( `*` là một trong các giá trị `sm` , `md` , `lg` , `xl`)
    ```html
    <div class="container">
      <p class="text-left">Left aligned text on all screen sizes.</p>
      <p class="text-sm-left">Left aligned text on small or wider screens.</p>
      <p class="text-md-left">Left aligned text on medium or wider screens.</p>
      <p class="text-lg-left">Left aligned text on large or wider screens.</p>
      <p class="text-xl-left">Left aligned text on xlarge or wider screens.</p>
    </div>
    ```
- `.text-break` : tự động xuống dòng khi dòng text quá dài . Nếu không sử dụng , text sẽ tự tràn giống như `.text-nowrap` :
    ```html
    <div class="container">
      <p>With .text-break:</p>
      <p class="text-break">AaBbCcDdEeFfGgHhIiJjKkLlMmNnOoPpQqRrSsTtUuVvWwXxYyZzAaBbCcDdEeFfGgHhIiJjKkLlMmNnOoPpQqRrSsTtUuVvWwXxYyZzAaBbCcDdEeFfGgHhIiJjKkLlMmNnOoPpQqRrSsTtUuVvWwXxYyZzAaBbCcDdEeFfGgHhIiJjKkLlMmNnOoPpQqRrSsTtUuVvWwXxYyZz</p>
      <p>Without .text-break:</p>
      <p>AaBbCcDdEeFfGgHhIiJjKkLlMmNnOoPpQqRrSsTtUuVvWwXxYyZzAaBbCcDdEeFfGgHhIiJjKkLlMmNnOoPpQqRrSsTtUuVvWwXxYyZzAaBbCcDdEeFfGgHhIiJjKkLlMmNnOoPpQqRrSsTtUuVvWwXxYyZzAaBbCcDdEeFfGgHhIiJjKkLlMmNnOoPpQqRrSsTtUuVvWwXxYyZz</p>
    </div>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/v4QrFhg.png>
- `.text-monospace` : convert chữ về font `monospace` 
    ```html
    <div class="container">
      <p class="text-monospace">Monospaced text.</p>
    </div>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/LBUFKlh.png>

- `.text-lowercase` : convert đoạn text thành chữ thường
- `.text-uppercase` : convert đoạn text thành chữ hoa
- `.text-capitalize` : convert đoạn text thành dạng viết hoa chữ cái đầu
    ```html
    <div class="container">
      <p class="text-lowercase">Lowercased text.</p>
      <p class="text-uppercase">Uppercased text.</p>      
      <p class="text-capitalize">Capitalized text.</p>
    </div>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/nEBvSva.png>
- `.text-reset`
- `.initialism`
- `.list-unstyled`
- `.list-inline`
- `.pre-scrollable`