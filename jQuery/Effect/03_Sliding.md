# jQuery Sliding
## **`slideDown()`**
- Phương thức `slideDown()` được sử dụng để trượt xuống (hiện) phần tử .
- Cú pháp :
    ```js
    $(selector).slideDown(speed,callback);
    ```
    - Trong đó : 
        - `speed` : tốc độ hiệu ứng fade . Có thể nhận các giá trị "`slow`", "`fast`" hoặc miliseconds .
        - `callback` : là hàm được thực hiện sau khi phương thức `slideDown()` được thực hiện .
    > Cả 2 tham số này đều là optional, có thể không thêm cũng được .
- **VD :**
    ```js
    $("#flip").click(function(){
      $("#panel").slideDown();
    });
    ```
## **`slideUp()`**
- Phương thức `slideUp()` được sử dụng để trượt lên (ẩn) phần tử .
- Cú pháp :
    ```js
    $(selector).slideUp(speed,callback);
    ```
    - Trong đó : 
        - `speed` : tốc độ hiệu ứng fade . Có thể nhận các giá trị "`slow`", "`fast`" hoặc miliseconds .
        - `callback` : là hàm được thực hiện sau khi phương thức `slideUp()` được thực hiện .
    > Cả 2 tham số này đều là optional, có thể không thêm cũng được .
- **VD :**
    ```js
    $("#flip").click(function(){
      $("#panel").slideUp();
    });
    ```
## **`slideToggle()`**
- Có thể thực hiện di chuyển qua lại giữa thao tác `slideUp()` và `slideDown()` bằng cách sử dụng phương thức `slideToggle()` .
    - Nếu phần tử đã bị ẩn, phương thức sẽ là `slideDown()` và ngược lại .
- Cú pháp :
    ```js
    $(selector).slideToggle(speed,callback);
    ```
    - Trong đó : 
        - `speed` : tốc độ hiệu ứng fade . Có thể nhận các giá trị "`slow`", "`fast`" hoặc miliseconds .
        - `callback` : là hàm được thực hiện sau khi phương thức `slideToggle()` được thực hiện .
    > Cả 2 tham số này đều là optional, có thể không thêm cũng được .