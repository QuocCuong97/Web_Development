# Phương thức `get()` và `post()`
## **1) `GET` và `POST` trong HTTP Request**
- Có 2 phương thức phổ biến được sử dụng cho một quá trình request - response giữa client và server là `GET` và `POST` .
    - `GET` - Request dữ liệu từ một nguồn được chỉ định
    - `POST` - Submit dữ liệu để được xử lý tới một nguồn được chỉ định
- `GET` đơn giản chỉ được sử dụng để lấy dữ liệu về từ server
    > **Lưu ý :** `GET` cũng có thể trả về dữ liệu cached
- `POST` cũng có thể được sử dụng để lấy dữ liệu về từ server . Tuy nhiên, phương thức `POST` sẽ không lưu cached data, và thường được sử dụng để gửi data kèm theo trong request
## **2) Phương thức `$.get()`**
- Phương thức `$.get()` request dữ liệu về từ server với một request `GET` HTTP
- Cú pháp :
    ```js
    $.get(URL,callback);
    ```
    - Trong đó :
        - `URL` : đường dẫn muốn lấy dữ liệu (bắt buộc)
        - `callback` : tên hàm sẽ được thực hiện sau khi phương thức `$.get()` được hoàn thành . Hàm `callback` cũng có mang 2 tham số tùy chọn :
            - `data` : nội dung response từ server
            - `status` : trạng thái của quá trình request - response
- **VD :**
    - File `demo_test.asp` :
        ```asp
        <%
        response.write("This is some text from an external ASP file.")
        %>
        ```
    - Dùng phương thức `get()` lấy dữ liệu về từ file `demo_test.asp` và trả về status :
        ```js
        $("button").click(function(){
        $.get("demo_test.asp", function(data, status){
            alert("Data: " + data + "\nStatus: " + status);
        });
        });
        ```
## **3) Phương thức `$.post()`**
- Phương thức `$.post()` request dữ liệu về từ server với một request `POST` HTTP
- Cú pháp :
    ```js
    $.post(URL,data,callback);
    ```
    - Trong đó :
        - `URL` : đường dẫn muốn lấy dữ liệu (bắt buộc)
        - `data` : dữ liệu muốn gửi kèm request
        - `callback` : tên hàm sẽ được thực hiện sau khi phương thức `$.get()` được hoàn thành . Hàm `callback` cũng có mang 2 tham số tùy chọn :
            - `data` : nội dung response từ server
            - `status` : trạng thái của quá trình request - response
- **VD :**
    - File `demo_test_post.asp` :
        ```asp
        <%
        dim fname,city
        fname=Request.Form("name")
        city=Request.Form("city")
        Response.Write("Dear " & fname & ". ")
        Response.Write("Hope you live well in " & city & ".")
        %>
        ```
    - Dùng phương thức `post()` để đẩy dữ liệu lên file `demo_test_post.asp` xử lý và lấy dữ liệu về :
        ```js
        $("button").click(function(){
          $.post("demo_test_post.asp",
          {
            name: "Donald Duck",
            city: "Duckburg"
          },
          function(data, status){
            alert("Data: " + data + "\nStatus: " + status);
          });
        });
        ```
    - Kết quả :

        <img src=https://i.imgur.com/ceIy08p.png>