# Callback Function
- Các lệnh **JavaScript** được thực hiện theo từng dòng một . Tuy nhiên, khi sử dụng hiệu ứng, dòng code tiếp theo có thể được chạy ngay cả khi hiệu ứng chưa kết thúc => Điều này gây ra lỗi .
- Để ngăn chặn điều này, ta sẽ tạo ra ***callback function*** .
- ***Callback function*** sẽ được thực thi sau khi hiệu ứng kết thúc hoàn toàn .
- **VD :**
    ```js
    $("button").click(function(){
      $("p").hide("slow", function(){
        alert("The paragraph is now hidden");
      });
    });
    ```
- Khi không sử dụng ***callback*** , alertbox sẽ xuất hiện trước khi hiệu ứng kết thúc :
    ```js
    $("button").click(function(){
      $("p").hide(1000);
      alert("The paragraph is now hidden");
    });
    ```
    