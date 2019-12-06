# CSS Selector
- **CSS selectors** được sử dụng để tìm kiếm ( hoặc chọn ) phần tử **HTML** muốn áp dụng style
- Có thể chia **CSS selectors** thành 5 mục :
    - **Simple selectors** - chọn phần tử dựa trên `name`, `id`, `class`
    - **Combinator selectors** - chọn phần tử dựa trên những mối quan hệ đặc biệt giữa chúng 
    - **Pseudo-class selectors** - chọn phần tử dựa trên những trạng thái nhất định
    - **Pseudo-elements selectors** - chọn và áp dụng style cho 1 phần của phần tử
    - **Attribute selectors** - chọn phần tử dựa trên thuộc tính và giá trị của thuộc tính
## **1) Simple selectors**
### **1.1) Chọn phần tử dựa theo tên**
- **VD :**
    ```css
    p {
      text-align: center;
      color: red;
    }
    ```
### **1.2) Chọn phần tử dựa theo `id`**
- **VD :**
    ```css
    #para1 {
      text-align: center;
      color: red;
    }
    ```
### **1.3) Chọn phần tử dựa theo `class`**
- **VD :**
    ```css
    .center {
      text-align: center;
      color: red;
    }
    ```
## **2) Combinator selectors**
### **2.1) Universal Selectors**
- Ký hiệu universal selector ( "`*`" ) chọn tất cả các phần tử **HTML** trên page .
- **VD :**
    ```css
    * {
      text-align: center;
      color: blue;
    }
    ```
### **2.2) Grouping Selectors**
- Grouping selector sẽ chọn tất cả các phần tử có cùng kiểu style .
- **VD :**
    ```css
    h1 {
      text-align: center;
      color: red;
    }

    h2 {
      text-align: center;
      color: red;
    }

    p {
      text-align: center;
      color: red;
    }
    ```
    - Có thể viết gọn lại thành :
    ```css
    h1, h2, p {
      text-align: center;
      color: red;
    }
    ```
### **2.3) Descendant Selectors**
- **Descendant selector** sẽ match tất cả các phần tử là hậu duệ của phần tử cho trước :
- **VD :** Chỉ có phần tử `<p>` là hậu duệ của phần tử `<div>` mới dính **CSS** :
    ```html
    <style>
    div p {
      background-color: yellow;
    }
    </style>
    <div>
      <p>Paragraph 1 in the div.</p>
      <p>Paragraph 2 in the div.</p>
      <section><p>Paragraph 3 in the div.</p></section>
    </div>

    <p>Paragraph 4. Not in a div.</p>
    <p>Paragraph 5. Not in a div.</p>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/gUkHcme.png>

### **2.4) Child Selectors**
- **Child selector** chọn tất cả các phần tử là phần tử con (liền sát) với phần tử cho trước .
- **VD :**
    ```html
    <style>
    div > p {
      background-color: yellow;
    }
    </style>
    <div>
      <p>Paragraph 1 in the div.</p>
      <p>Paragraph 2 in the div.</p>
      <section><p>Paragraph 3 in the div.</p></section> <!-- not Child but Descendant -->
      <p>Paragraph 4 in the div.</p>
    </div>
    <p>Paragraph 5. Not in a div.</p>
    <p>Paragraph 6. Not in a div.</p>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/A4XM9Bq.png>

### **2.5) Adjacent Sibling Selector**
- **Adjacent Sibling selector** chọn tất cả các phần tử liền kề với phần tử cho trước .
- **VD :**
    ```html
    <style>
    div + p {
      background-color: yellow;
    }
    </style>
    <div>
      <p>Paragraph 1 in the div.</p>
      <p>Paragraph 2 in the div.</p>
    </div>

    <p>Paragraph 3. Not in a div.</p>
    <p>Paragraph 4. Not in a div.</p>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/lZFUsEi.png>

### **2.6) General Sibling Selector**
- **General sibling selector** chọn tất cả các phần tử là anh em của phần tử cho trước ( tính từ phía sau ) :
- **VD :**
    ```html
    <style>
    div ~ p {
      background-color: yellow;
    }
    </style>
    <p>Paragraph 1.</p>
    <div>
      <p>Paragraph 2.</p>
    </div>

    <p>Paragraph 3.</p>
    <code>Some code.</code>
    <p>Paragraph 4.</p>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/qF5o99z.png>

## **3) Pseudo-class selectors**
- Chọn phần tử dựa trên những trạng thái nhất định
- Cú pháp :
    ```css
    selector:pseudo-class {
      property:value;
    }
    ```
### **3.1) Selector là các trạng thái của phần tử**
- **VD :**
    ```css
    /* unvisited link */
    a:link {
      color: #FF0000;
    }

    /* visited link */
    a:visited {
      color: #00FF00;
    }

    /* mouse over link */
    a:hover {
      color: #FF00FF;
    }

    /* selected link */
    a:active {
      color: #0000FF;
    }
    ```
### **3.2) Selector là các trạng thái của phần tử đi kèm với class** 
- **VD :**
    ```css
    a.highlight:hover {
      color: #ff0000;
    }
    ```
### **3.3) Selector hover để hiện phần tử khác**
- **VD :**
    ```html
    <style>
    p {
      display: none;
      background-color: yellow;
      padding: 20px;
    }

    div:hover p {
      display: block;
    }
    </style>
    <div>Hover over me to show the p element
      <p>Tada! Here I am!</p>
    </div>
    ```
    - **VD :**

        <img src=https://i.imgur.com/56n3pNf.png>

### **3.4) `:first-child`**
- `:first-child` selector chọn phần tử được khai báo là phần tử con đầu tiên của phần tử khác .
- **VD1 :** Chọn phần tử `<p>` đầu tiên :
    ```html
    <style>
    p:first-child {
      color: blue;
    } 
    </style>
    <body>
    <p>This is some text.</p>
    <p>This is some text.</p>
    </body>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/4UN59XW.png>

- **VD2 :** Chọn phần tử `<i>` đầu tiên trong tất cả các phần tử `<p>` :
    ```html
    <style>
    p i:first-child {
      color: blue;
    } 
    </style>
    <body>
    <p>I am a <i>strong</i> person. I am a <i>strong</i> person.</p>
    <p>I am a <i>strong</i> person. I am a <i>strong</i> person.</p>
    </body>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/9yCRy09.png>

## **4) Pseudo-elements selectors**
- Sử dụng để chọn và áp dụng style cho 1 phần của phần tử .
- Cú pháp :
    ```css
    selector::pseudo-element {
      property:value;
    }
    ```
### **4.1) `::first-line`**
- Sử dụng để chèn CSS vào dòng đầu tiên của đoạn text .
- Các thuộc tính có thể áp dụng trong `::first-line` :
    - Các thuộc tính `font`
    - Các thuộc tính `color`
    - Các thuộc tính `background`
    - `word-spacing`
    - `letter-spacing`
    - `text-decoration`
    - `vertical-align`
    - `text-transform`
    - `line-height`
    - `clear`
- **VD :**
    ```html
    <style>
    p::first-line {
      color: #ff0000;
      font-variant: small-caps;
    }
    </style>
    <p>You can use the ::first-line pseudo-element to add a special effect to the first line of a text. Some more text. And even more, and more, and more, and more, and more, and more, and more, and more, and more, and more, and more, and more.</p>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/rCxgpSt.png>

### **4.2) `::first-letter`**
- Sử dụng để chèn CSS vào chữ đầu tiên của đoạn text .
- Các thuộc tính có thể áp dụng trong `::first-letter` :
    - Các thuộc tính `font`
    - Các thuộc tính `color`
    - Các thuộc tính `background`
    - Các thuộc tính `margin`
    - Các thuộc tính `padding`
    - Các thuộc tính `border`
    - `text-decoration`
    - `vertical-align` ( `float: none` )
    - `text-transform`
    - `line-height`
    - `float`
    - `clear`
- **VD :**
    ```html
    <style>
    p::first-letter {
      color: #ff0000;
      font-size: xx-large;
    }
    </style>
    <p>You can use the ::first-letter pseudo-element to add a special effect to the first character of a text!</p>
    ```
    - Hiển thị trên trình duyệt :
        
        <img src=https://i.imgur.com/UKo2czm.png>

### **4.3) `::before`**
- Sử dụng để chèn một nội dung vào trước nội dung của phần tử .
- **VD :**
    ```html
    <style>
    h1::before {
      content: url(smiley.gif);
    }
    </style>
    <h1>This is a heading</h1>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/y3NQTEW.png>

### **4.4) `::after`**
- Sử dụng để chèn một nội dung vào sau nội dung của phần tử .
- **VD :**
    ```html
    <style>
    h1::after {
      content: url(smiley.gif);
    }
    </style>
    <h1>This is a heading</h1>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/gD9CPv6.png>

### **4.5) `::selection`**
- Sử dụng để chọn một phần của phần tử được chọn bởi user .
- **VD :**
    ```html
    <style>
    ::-moz-selection { /* Code for Firefox */
      color: red;
      background: yellow;
    }

    ::selection {
      color: red;
      background: yellow;
    }
    </style>
    <p>This is a paragraph.</p>
    <div>This is some text in a div element.</div>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/3146gBw.png>

### **4.6) Sử dụng pseudo-elements kết hợp với class**
- **VD :**
    ```css
    p.intro::first-letter {
      color: #ff0000;
      font-size:200%;
    }
    ```
### **4.7) Sử dụng nhiều pseudo-elements cho một phần tử**
- **VD :**
    ```css
    p::first-letter {
      color: #ff0000;
      font-size: xx-large;
    }

    p::first-line {
      color: #0000ff;
      font-variant: small-caps;
    }
    ```



