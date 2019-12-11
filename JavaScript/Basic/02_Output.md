# Cách hiển thị dữ liệu ra màn hình
- **JavaScript** có thể hiển thị dữ liệu theo các cách khác nhau :
    - Ghi đè phần tử HTML - sử dụng `innerHTML`
    - Ghi ra output của trag HTML - sử dụng `document.write()`
    - Đưa ra cửa sổ cảnh báo - sử dụng `window.alert()`
    - Writing into the browser console, using `console.log()`
### **1) Sử dụng `innerHTML`**
- Để access một phần tử **HTML**, **JavaScript** cần sử dụng phương thức `document.getElementById(id)` .
- Thuộc tính `id` sẽ định nghĩa tên phần tử **HTML** cần áp dụng . 
- **VD :**
    ```html
    <p id="demo"></p>
    <script>
    document.getElementById("demo").innerHTML = 5 + 6;
    </script>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/On21tDC.png>

### **2) Sử dụng `document.write()`**
- Không nên sử dụng `document.write()` sau khi trang web đã được load, vì nó sẽ reset tất cả trang HTML và chỉ hiển thị kết quả `document.write()` 
- **VD :**
    ```html
    <script>
    document.write(5 + 6);
    </script>
    ```
### **3) Sử dụng `window.alert()`**
- **VD :**
    ```html
    <script>
    window.alert(5 + 6);
    </script>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/JE5NMTF.png>

### **4) Sử dụng `console.log()`**
- Để phục vụ cho mục đính debug, có thể sử dụng phương thức `console.log()` để hiển thị dữ liệu .
- **VD :**
    ```html
    <script>
    console.log(5 + 6);
    </script>
    ```
