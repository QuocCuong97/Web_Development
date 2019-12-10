# CSS Forms
## **1) Styling Input Fields**
### **1.1) Độ rộng trường input**
- Sử dụng thuộc tính `width` để định nghĩa độ rộng trường input .
- **VD :**
    ```css
    input {
      width: 100%;
    }
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/IfMOXPw.png>

### **1.2) Phân loại trường input**
- Sử dụng selector `type` để xác định rõ trường input nào được áp dụng CSS :
    - `input[type=text]` : chỉ áp dụng cho các trường text
    - `input[type=password]` : chỉ áp dụng cho các trường password
    - `input[type=number]` : chỉ áp dụng cho các trường nhập số
### **1.3) Thêm padding - margin**
- Sử dụng thuộc tính `padding` để thêm không gian bên trong trường input .
- Sử dụng thuộc tính `margin` để thêm không gian giữa các trường input khác nhau .
- **VD :**
    ```html
    <style> 
    input[type=text] {
      width: 100%;
      padding: 12px 20px;
      margin: 8px 0;
      box-sizing: border-box;
    }
    </style>
    <form>
      <label for="fname">First Name</label>
      <input type="text" id="fname" name="fname">
      <label for="lname">Last Name</label>
      <input type="text" id="lname" name="lname">
    </form>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/Biko6y6.png>

### **1.4) Thêm border**
- Sử dụng thuộc tính `border` để thay đổi kích cỡ và màu sắc border .
- Sử dụng thuộc tính `border-radius` để bo cong góc border .
- **VD :**
    ```css
    <style> 
    input[type=text] {
      width: 100%;
      padding: 12px 20px;
      margin: 8px 0;
      box-sizing: border-box;
      border: 2px solid red;
      border-radius: 4px;
    }
    </style>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/3X78aQB.png>

### **1.5) Thêm background color**
- Sử dụng thuộc tính `background` để thêm màu nền cho trường input
- Thuộc tính `color` để thêm màu chữ cho trường input .
- **VD :**
    ```css
    input[type=text] {
      width: 100%;
      padding: 12px 20px;
      margin: 8px 0;
      box-sizing: border-box;
      border: none;
      background-color: #3CBC8D;
      color: white;
    }
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/ofKJh4k.png>

### **1.6) Focus input**
- Mặc định, trình duyệt sẽ thêm 1 đường outline màu xanh quanh trường input khi nó được focus (được click) . Có thể bỏ chức năng này bằng cách thêm thuộc tính "`outline: none;`"
- Sử dụng selector "`:focus`" để thêm **CSS** khi trường input được focus .
- **VD :**
    ```css
    input[type=text] {
      width: 100%;
      padding: 12px 20px;
      margin: 8px 0;
      box-sizing: border-box;
      border: 1px solid #555;
      outline: none;
    }

    input[type=text]:focus {
      background-color: lightblue;
    }
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/kuuG4qh.png>

### **1.7) Animated Search Input**
- Sử dụng thuộc tính `transition` để tự động thay đổi độ rộng của trường search khi được focus .
- **VD :**
    ```css
    input[type=text] {
      -webkit-transition: width 0.4s ease-in-out;
      transition: width 0.4s ease-in-out;
    }

    input[type=text]:focus {
      width: 100%;
    }
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/zi1bdRN.png>

## **2) Styling Textareas**
- Sử dụng thuộc tính `resize` để chống cho `textarea` bị thay đổi kích cỡ (bằng cách này sẽ xóa được dấu `grabber` ở góc dưới textarea )
- **VD :**
    ```html
    <style>
    textarea {
      width: 100%;
      height: 150px;
      padding: 12px 20px;
      box-sizing: border-box;
      border: 2px solid #ccc;
      border-radius: 4px;
      background-color: #f8f8f8;
      resize: none;
    }
    </style>
    <form>
      <textarea>Some text...</textarea>
    </form>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/7C5xhVg.png>

## **3) Styling Select Menus**
- **VD :**
    ```html
    <style>
    select {
      width: 100%;
      padding: 16px 20px;
      border: none;
      border-radius: 4px;
      background-color: #f1f1f1;
    }
    </style>
    <form>
      <select id="country" name="country">
        <option value="au">Australia</option>
        <option value="ca">Canada</option>
        <option value="usa">USA</option>
      </select>
    </form>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/ssu0NPl.png>

## **4) Styling Input Buttons**
- **VD :**
    ```html
    <style>
    input[type=button], input[type=submit], input[type=reset] {
      background-color: #4CAF50;
      border: none;
      color: white;
      padding: 16px 32px;
      text-decoration: none;
      margin: 4px 2px;
      cursor: pointer;
    }
    </style>
    <input type="button" value="Button">
    <input type="reset" value="Reset">
    <input type="submit" value="Submit">
    ```
    - Hiển thị trên trình duyệt :   

        <img src=https://i.imgur.com/PMHUSm4.png>
