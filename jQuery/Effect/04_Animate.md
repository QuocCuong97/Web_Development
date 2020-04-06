# jQuery Effect
## **`animate()`**
- Phương thức `animate()` được sử dụng để tạo các animation tùy ý .
- Cú pháp :
    ```js
    $(selector).animate({params},speed,callback);
    ```
    - Trong đó : 
        - `{param}` : định nghĩa các thuộc tính CSS cho mỗi animation . Tham số này là **BẮT BUỘC**
        - `speed` : tốc độ hiệu ứng fade . Có thể nhận các giá trị "`slow`", "`fast`" hoặc miliseconds . Tham số này là **KHÔNG BẮT BUỘC**
        - `callback` : là hàm được thực hiện sau khi phương thức `fadeIn()` được thực hiện . Tham số này là **KHÔNG BẮT BUỘC**
- **VD1 :** Sử dụng 1 thuộc tính CSS :
    ```js
    $("button").click(function(){
      $("div").animate({left: '250px'});
    }); 
    ```
- **VD2 :** Sử dụng nhiều thuộc tính CSS :
    ```js
    $("button").click(function(){
      $("div").animate({
        left: '250px',
        opacity: '0.5',
        height: '150px',
        width: '150px'
      });
    }); 
    ```
- **VD3 :** Sử dụng các giá trị tương đối :
    ```js
    $("button").click(function(){
      $("div").animate({
        left: '250px',
        height: '+=150px',
        width: '+=150px'
      });
    }); 
    ```
- **VD4 :** Sử dụng các giá trị được định nghĩa trước : `show`/`hide`/`toggle` :
    ```js
    $("button").click(function(){
      $("div").animate({
        height: 'toggle'
      });
    }); 
    ```
- **VD5 :** Sử dụng theo phương pháp dùng hàm :
    ```js
    $("button").click(function(){
      var div = $("div");
      div.animate({height: '300px', opacity: '0.4'}, "slow");
      div.animate({width: '300px', opacity: '0.8'}, "slow");
      div.animate({height: '100px', opacity: '0.4'}, "slow");
      div.animate({width: '100px', opacity: '0.8'}, "slow");
    }); 
    ```