# jQuery `stop()` method
- Phương thức `stop()` được dùng để dừng hiệu ứng hoặc animation trước khi nó kết thúc .
- Phương thức `stop()` hoạt động với tất cả các hàm hiệu ứng **jQuery**, bao gồm sliding, fading và custom animation .
- Cú pháp :
    ```js
    $(selector).stop(stopAll,goToEnd);
    ```
    - Trong đó :
        - `stopAll` : chỉ định những animations nào sẽ bị dừng . Mặc định có giá trị là `false`, có nghĩa nếu sử dụng thì nó chỉ dừng lại những animation đang hoạt động, còn những animation hoạt động sau thời điểm đó sẽ không bị ảnh hưởng .
        - `gotoEnd` : chỉ định xem có để animation chạy đến khi kết thúc không. Mặc định là `False` .
    > Cả 2 tham số này đều là optional, có thể không thêm cũng được .
- **VD :**
    ```js
    $("#stop").click(function(){
      $("#panel").stop();
    });
    ```
    