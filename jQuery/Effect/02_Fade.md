# jQuery Fading
## **`fadeIn()`**
- Phương thức `fadeIn()` được sử dụng để làm hiện lên (fading) các phần tử đã bị ẩn đi từ trước .
- Cú pháp :
    ```js
    $(selector).fadeIn(speed,callback);
    ```
    - Trong đó : 
        - `speed` : tốc độ hiệu ứng fade . Có thể nhận các giá trị "`slow`", "`fast`" hoặc miliseconds .
        - `callback` : là hàm được thực hiện sau khi phương thức `fadeIn()` được thực hiện .
    > Cả 2 tham số này đều là optional, có thể không thêm cũng được .
- **VD :**
    ```js
    $("button").click(function(){
      $("#div1").fadeIn();
      $("#div2").fadeIn("slow");
      $("#div3").fadeIn(3000);
    });
    ```
## **`fadeOut()`**
- Phương thức `fadeOut()` được sử dụng để làm hiện lên (fading) các phần tử đang có sẵn .
- Cú pháp :
    ```js
    $(selector).fadeOut(speed,callback);
    ```
    - Trong đó : 
        - `speed` : tốc độ hiệu ứng fade . Có thể nhận các giá trị "`slow`", "`fast`" hoặc miliseconds .
        - `callback` : là hàm được thực hiện sau khi phương thức `fadeOut()` được thực hiện .
    > Cả 2 tham số này đều là optional, có thể không thêm cũng được .
- **VD :**
    ```js
    $("button").click(function(){
      $("#div1").fadeOut();
      $("#div2").fadeOut("slow");
      $("#div3").fadeOut(3000);
    });
    ```
## **`fadeToggle()`**
- Có thể thực hiện di chuyển qua lại giữa thao tác `fadeIn()` và `fadeOut()` bằng cách sử dụng phương thức `fadeToggle()` .
    - Nếu phần tử đã được fade out, phương thức sẽ là `fadeIn()` và ngược lại .
- Cú pháp :
    ```js
    $(selector).fadeToggle(speed,callback);
    ```
    - Trong đó : 
        - `speed` : tốc độ hiệu ứng fade . Có thể nhận các giá trị "`slow`", "`fast`" hoặc miliseconds .
        - `callback` : là hàm được thực hiện sau khi phương thức `fadeToggle()` được thực hiện .
    > Cả 2 tham số này đều là optional, có thể không thêm cũng được .
- **VD :**
    ```js
    $("button").click(function(){
      $("#div1").fadeToggle();
      $("#div2").fadeToggle("slow");
      $("#div3").fadeToggle(3000);
    });
    ```
## **`fadeTo()`**
- Phương thức `fadeTo()` cho phép fade phần tử với một giá trị opacity cho trước ( từ `0->1` )
- Cú pháp :
    ```js
    $(selector).fadeTo(speed,opacity,callback);
    ```
    - Trong đó : 
        - `speed` : tốc độ hiệu ứng fade . Có thể nhận các giá trị "`slow`", "`fast`" hoặc miliseconds . Tham số này là **BẮT BUỘC**
        - `opacity` : giá trị opacity (từ `0->1`) . Tham số này là **BẮT BUỘC**
        - `callback` : là hàm được thực hiện sau khi phương thức `fadeTo()` được thực hiện .
- **VD :**
    ```js
    $("button").click(function(){
      $("#div1").fadeTo("slow", 0.15);
      $("#div2").fadeTo("slow", 0.4);
      $("#div3").fadeTo("slow", 0.7);
    });
    ```
    