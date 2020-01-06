# History
- **Object** `window.history` chứa lịch sử duyệt web của người dùng .
- **Object** `window.history` có thể được gọi mà không cần tiền tố `window` .
- Để bảo vệ quyền riêng tư cho user, **JavaScript** chỉ có thể tác động trong giới hạn với lịch sử duyệt web .
## **1) Phương thức `history.back()`**
- Phương thức `history.back()` sẽ load trang web trước trong list lịch sử URL .
- **VD :**
    ```js
    <html>
    <head>
    <script>
    function goBack() {
      window.history.back()
    }
    </script>
    </head>
    <body>

    <input type="button" value="Back" onclick="goBack()">

    </body>
    </html>
    ```
## **2) Phương thức `history.forward()`**
- Phương thức `history.forward()` sẽ load trang web kế tiếp trong list lịch sử URL .
- **VD :**
    ```js
    <html>
    <head>
    <script>
    function goForward() {
      window.history.forward()
    }
    </script>
    </head>
    <body>

    <input type="button" value="Forward" onclick="goForward()">

    </body>
    </html>
    ```
    