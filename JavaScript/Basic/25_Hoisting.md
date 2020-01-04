# Hoisting

- "`Hoisting`" là hành động mặc định của JavaScript, nó sẽ di chuyển những câu lệnh khai báo tên biến lên vị trí đầu tiên trong phạm vi (lên đầu tập tin hiện tại hoặc lên đầu hàm hiện tại)
- Một biến có thể được khai báo sau khi nó được sử dụng .
- **VD :**
    ```html
    <script>
      text = "Hello";
      document.write(text);
      var text;
    </script>
    ```
- Có 2 trường hợp đặc biệt sẽ không được `hoisting` là lệnh `let` và lệnh `const`
- `Hoisting` chỉ chuyển phần khai báo biến lên đầu, chứ khai báo biến cùng giá trị khởi tạo thì không .
    ```html
    <script>
      document.write(text);
      var text = "Lập Trình Web";
    </script>
    ```
    => Đoạn code này sẽ gây ra lỗi .
- `Hoisting` giúp ta tránh tình trạng bị lỗi khi sử dụng những biến chưa được khai báo .
- Nếu đang ở trong một hàm mà ta gán giá trị cho biến chưa được khai báo thì biến đó sẽ trở thành biến **global** . `Hoisting` giúp ta tránh tình trạng tạo ra những biến **global** không mong muốn .
    ```html
    <script>
    function hello(){
        text = "Hello World";
        document.write(text);

    }
    hello();
    document.write("<br>Xin chào: " + text);
    </script>
    ```
    => Kết quả : `Hello World`