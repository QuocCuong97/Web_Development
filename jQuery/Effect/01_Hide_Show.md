# jQuery Hide and Show
## **`hide()`** và **`show()`**
- Với **jQuery**, có thể ẩn và hiện phần tử HTML bằng phương thức `hide()` và `show()`
- Cú pháp :
    ```js
    $(selector).hide(speed,callback);

    $(selector).show(speed,callback);
    ```
    - Trong đó : 
        - `speed` : tốc độ ẩn, hiện phần tử . Có thể nhận các giá trị "`slow`", "`fast`" hoặc miliseconds .
        - `callback` : là hàm được thực hiện sau khi phương thức `hide()` và `show()` được thực hiện .
    > Cả 2 tham số này đều là optional, có thể không thêm cũng được .
- **VD :**
    ```js
    $("button").click(function(){
      $("p").hide(1000);
    });
    ```
## **`toggle()`**
- Có thể thực hiện di chuyển qua lại giữa thao tác `hide()` và `show()` bằng cách sử dụng phương thức `toggle()` .
- Cú pháp :
    ```js
    $(selector).toggle(speed,callback);
    ```
    - Trong đó : 
        - `speed` : tốc độ ẩn, hiện phần tử . Có thể nhận các giá trị "`slow`", "`fast`" hoặc miliseconds .
        - `callback` : là hàm được thực hiện sau khi phương thức `toggle()` được thực hiện .
    > Cả 2 tham số này đều là optional, có thể không thêm cũng được .
- **VD :** Gán phương thức `toggle()` vào button để ẩn/hiện phần tử `<p>` :
    ```js
    $("button").click(function(){
      $("p").toggle();
    });
    ```
