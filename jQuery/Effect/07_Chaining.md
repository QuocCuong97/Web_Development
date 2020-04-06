# jQuery Chaining
- Cho đến giờ, ta có thể viết các mệnh đề **jQuery** từng dòng một . 
- Tuy nhiên, có một công nghệ gọi là ***chaining**, cho phép ta chạy nhiều lệnh **jQuery**, lệnh này xong đến lệnh kia ngay trên cùng 1 phần tử .
- Để xâu chuỗi các lệnh, ta chỉ cần thêm lệnh sau vào ngay sau lệnh trước .
- **VD :**
    ```js
    $("#p1").css("color", "red").slideUp(2000).slideDown(2000);
    ```
    hoặc cũng có thể viết :
    ```js
    $("#p1").css("color", "red")
      .slideUp(2000)
      .slideDown(2000);
    ```