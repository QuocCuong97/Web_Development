# jQuery Events
## **1) Các phương thức event thông dụng**
### **`click()`**
- Phương thức `click()` đính kèm một hàm xử lý event vào phần tử HTML .
- Hàm sẽ được thực thi khi user click vào phần tử
- **VD :**
    ```js
    $("p").click(function(){
      $(this).hide();
    });
    ```
### **`dbclick()`**
- Phương thức `dbclick()` đính kèm một hàm xử lý event vào phần tử HTML .
- Hàm sẽ được thực thi khi user click đúp vào phần tử
- **VD :**
    ```js
    $("p").dblclick(function(){
      $(this).hide();
    });
    ```
### **`mouseenter()`**
- Phương thức `mouseenter()` đính kèm một hàm xử lý event vào phần tử HTML .
- Hàm sẽ được thực hiện khi con trỏ chuột chạm tới phần tử
- **VD :**
    ```js
    $("#p1").mouseenter(function(){
      alert("You entered p1!");
    });
### **`mouseleave()`**
- Phương thức `mouseleave()` đính kèm một hàm xử lý event vào phần tử HTML .
- Hàm sẽ được thực thi khi con trỏ chuột rời khỏi phần tử .
- **VD :**
    ```js
    $("#p1").mouseleave(function(){
      alert("Bye! You now leave p1!");
    });
    ```
### **`mousedown()`**
- Phương thức `mousedown()` đính kèm một hàm xử lý event vào phần tử HTML .
- Hàm sẽ được thực thi khi chuột trái, chuột giữa, chuột phải giữ lì tại phần tử .
- **VD :**
    ```js
    $("#p1").mousedown(function(){
      alert("Mouse down over p1!");
    });
### **`mouseup()`**
- Phương thức `mouseup()` đính kèm một hàm xử lý event vào phần tử HTML .
- Hàm sẽ được thực thi khi chuột trái, chuột giữa, chuột phải nhả ra sau khi giữ lì tại phần tử .
- **VD :**
    ```js
    $("#p1").mouseup(function(){
      alert("Mouse up over p1!");
    });
    ```
### **`hover()`**
- Phương thức `hover()` nhận vào 2 hàm và kết hợp chúng thành 2 phương thức `mouseenter()` và `mouseleave()` .
- Hàm đầu tiên sẽ được thực thi khi con trỏ chuột chạm tới phần tử và hàm thứ 2 sẽ thực thi khi con trỏ chuột rời khỏi phần tử
- **VD :**
    ```js
    $("#p1").hover(function(){
      alert("You entered p1!");
    },
    function(){
      alert("Bye! You now leave p1!");
    });
    ```
### **`focus()`**
- Phương thức `focus()` đính kèm một hàm xử lý event vào HTML form field .
- Hàm sẽ được thực thi khi focus vào form field .
- **VD :**
    ```js
    $("input").focus(function(){
      $(this).css("background-color", "#cccccc");
    });
    ```
### **`blur()`**
- Phương thức `focus()` đính kèm một hàm xử lý event vào HTML form field .
- Hàm sẽ được thực thi khi mất focus trên form field .
- **VD :**
    ```js
    $("input").blur(function(){
      $(this).css("background-color", "#ffffff");
    });
    ```
## **2) Phương thức `on()`**
- Phương thức `on()` đính kèm một hoặc nhiều hàm xử lý event vào phần tử HTML .
- **VD1 :** Đính kèm 1 event click vào phần tử `<p>` :
    ```js
    $("p").on("click", function(){
      $(this).hide();
    });
    ```
- **VD2 :** Đính kèm trình xử lý event vào phần tử `<p>` :
    ```js
    $("p").on({
    mouseenter: function(){
      $(this).css("background-color", "lightgray");
    },
    mouseleave: function(){
      $(this).css("background-color", "lightblue");
    },
    click: function(){
      $(this).css("background-color", "yellow");
    }
    });
    ```