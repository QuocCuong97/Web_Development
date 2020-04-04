# DOM Event Listener
- Phương thức `addEventListener()` đính kèm một trình xử lý event vào phần tử cho trước mà không ghi đè các trình xử lý event đã có .
- Có thể thêm nhiều trình xử lý event cùng loại vào một phần tử (VD: 2 event click,...)
- Phương thức `addEventListener()` giúp việc kiểm soát các event dễ dàng hơn .
- Có thể xóa bỏ event listener bằng phương thức `removeEventListener()` .
- Cú pháp :
    ```
    element.addEventListener(event, function);
    ```
    - Trong đó :
        - `event` : một HTML DOM event ( như click, mousedown,...)
        - `function` : function muốn gọi khi event xảy ra
### **Thêm một Event Handler vào phần tử**
- Cú pháp :
    ```js
    element.addEventListener("click", function(){ alert("Hello World!"); });
    ```
- **VD :** Tạo hộp thoại alert "`Hello World`" khi user click vào phần tử :
    ```html
    <button id="myBtn">Try it</button>
    <script>
    document.getElementById("myBtn").addEventListener("click", function() {
      alert("Hello World!");
    });
    </script>
    ```
    hoặc 
    ```html
    <button id="myBtn">Try it</button>
    <script>
    document.getElementById("myBtn").addEventListener("click", myFunction);
    function myFunction() {
      alert ("Hello World!");
    }
    </script>
    ```
    => Kết quả :

    <img src=https://i.imgur.com/vI8bIHa.png>

### **Thêm nhiều Event Handlers vào cùng một phần tử**
- Cú pháp 1 : Thêm nhiều event cùng loại vào 1 phần tử :
    ```js
    element.addEventListener("click", myFunction);
    element.addEventListener("click", mySecondFunction);
    ```
- **VD :**
    ```html
    <button id="myBtn">Try it</button>
    <script>
    var x = document.getElementById("myBtn");
    x.addEventListener("click", myFunction);
    x.addEventListener("click", someOtherFunction);
    function myFunction() {
      alert ("Hello World!");
    }
    function someOtherFunction() {
      alert ("This function was also executed!");
    }
    </script>
    ```
    => Kết quả : Click button "`Try it`" :

    <img src=https://i.imgur.com/yitoP8g.png>

    => Click button "`OK`" :

    <img src=https://i.imgur.com/ZXvNuEa.png>

- Cú pháp 2 : Thêm nhiều phần tử khác loại vào 1 phần tử :
    ```js
    element.addEventListener("mouseover", myFunction);
    element.addEventListener("click", mySecondFunction);
    element.addEventListener("mouseout", myThirdFunction);
    ```
### **Passing Parameter**
### **Phương thức `removeEventListener()`**
- Phương thức `removeEventListener()` xóa bỏ event handler đã được đính kèm bằng phương thức `addEventListener()` :
    ```js
    element.removeEventListener("mousemove", myFunction);
    ```
