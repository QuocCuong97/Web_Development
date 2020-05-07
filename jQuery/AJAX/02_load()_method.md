# Phương thức `load()`
- Phương thức `load()` của **jQuery** vô cùng đơn giản, nhưng sử dụng với **AJAX** thì lại vô cùng quyền năng .
- Phương thức `load()` sẽ load dữ liệu từ một server khác và đẩy dữ liệu trả về vào thẳng phần tử được chọn .
- Cú pháp :
    ```js
    $(selector).load(URL,data,callback);
    ```
    - Trong đó :
        - `URL` : đường dẫn muốn lấy dữ liệu (bắt buộc)
        - `data` : chỉ ra cặp querystring key/value gửi đi cùng request (tùy chọn)
        - `callback` : tên hàm sẽ được thực hiện sau khi phương thức `load()` được hoàn thành .
- **VD :**
    - File `demo_test.txt` :
        ```html
        <h2>jQuery and AJAX is FUN!!!</h2>
        <p id="p1">This is some text in a paragraph.</p>
        ```
    - File `.html` : Chèn nội dung file `demo_test.txt` vào thẻ `<div>` :
        ```html
        <html>
          <head>
            <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.4.1/jquery.min.js"></script>
            <script>
              $(document).ready(function(){
                $("button").click(function(){
                  $("#div1").load("demo_test.txt");
                });
              });
            </script>
          </head>
          <body>
            <div id="div1"><h2>Let jQuery AJAX Change This Text</h2></div>
            <button>Get External Content</button>
          </body>
        </html>
        ```
    - Cũng có thể chỉ định chính xác phần tử được lấy ra trong file `demo_test` để chèn vào thẻ `<div>` :
        ```js
        $("#div1").load("demo_test.txt #p1");
        ```
- Tham số tùy chọn `callback` chỉ định tên hàm sẽ được thực hiện sau khi phương thức `load()` được hoàn thành . Hàm `callback` có thể có các tham số khác :
    - `responseTxt` - chứa nội dung response nếu quá trình request - response thành công .
    - `status` - chứa trạng thái của quá trình request - response .
    - `xhr` - chứa object `XMLHttpRequest`
- **VD2 :** 
    ```js
    $("button").click(function(){
      $("#div1").load("demo_test.txt", function(responseTxt, statusTxt, xhr){
        if(statusTxt == "success")
          alert("External content loaded successfully!");
        if(statusTxt == "error")
          alert("Error: " + xhr.status + ": " + xhr.statusText);
      });
    });
    ```