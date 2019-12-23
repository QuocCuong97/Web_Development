# Images
## **1) Image Shapes**
### **1.1) Class "`.rounded`"**
- Class "`.rounded`" thêm các đường bo góc cong cho hình ảnh .
- **VD :**
    ```html
    <img src="cinqueterre.jpg" class="rounded" alt="Cinque Terre">
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/Z3xjjiF.png>

### **1.2) Class"`.rounded-circle`"**
- Class "`.rounded-circle`" sẽ co hình ảnh lại gói gọn trong 1 đường tròn .
- **VD :**
    ```html
    <img src="cinqueterre.jpg" class="rounded-circle" alt="Cinque Terre">
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/lGzBP7s.png>

### **1.3) Class "`img-thumbnail`"**
- Class "`.img-thumbnail`" sẽ co hình ảnh lại thành 1 hình thumbnail ( có border )
- **VD :**
    ```html
    <img src="cinqueterre.jpg" class="img-thumbnail" alt="Cinque Terre">
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/Rvz5U0V.png>

## **2) Align Images**
### **2.1) Class "`.float-left`" và "`float-right`"**
- Sử dụng class "`.float-left`" để float hình ảnh sang trái và class "`.float-right`" để float hình ảnh sang phải .
- **VD :**
    ```html
    <img src="paris.jpg" class="float-left">
    <img src="paris.jpg" class="float-right">
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/W79UgXH.png>

### **2.2) Class "`.mx-auto`" và "`.d-block`"**
- Căn chỉnh giữa cho hình ảnh bằng cách sử dụng class "`.mx-auto`" ( margin:auto ) và "`.d-block`" ( display:block ) .
- **VD :**
    ```html
    <img src="paris.jpg" class="mx-auto d-block">
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/6vLARpG.png>
## **3) Responsive Images**
- Hình ảnh có nhiều kích cỡ . Màn hình cũng có nhiều kích cỡ . Các hình ảnh responsive sẽ tự động fit với kích cỡ của màn hình .
- Có thể tạo hình ảnh responsive bằng cách sử dụng class "`.img-fluid`" trong thẻ `<img>` .
- Class "`.img-fluid`" sẽ apply các thuộc tính "`max-width: 100%`" và "`height: auto`" vào hình ảnh :
- **VD :**
    ```html
    <img class="img-fluid" src="img_chania.jpg" alt="Chania">
    ```
    