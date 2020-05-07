# Phương thức `ajax()`
- Phương thức `ajax()` được dùng để thực hiện các request HTTP bất đồng bộ .
- Tất cả các phương thức **jQuery AJAX** thực ra đều sử dụng phương thức `ajax()`. Phương thức này hầu hết được sử dụng cho các request mà không thể sử dụng được các phương thức khác .
- Cú pháp :
    ```js
    $.ajax({name:value, name:value, ... })
    ```
    - Trong đó, các tham số chỉ ra các cặp tên:giá trị cho request **AJAX**
- Các tham số tên trong cú pháp có thể là :
    - `accepts`: Nội dung được gửi trong request header giúp server biết được kiểu response server sẽ chấp nhận khi trả về.
    - `async`: Thiết lập giá trị false để thực hiện một request đồng bộ.
    - `beforeSend`: Một hàm pre-request gọi lại có thể dùng để điều chỉnh object jqXHR trước khi nó được gửi.
    - `cache`: Thiết lập giá trị false để buộc browser không lưu cache các trang được request.
    - `complete`: Một hàm được thực thi khi request kết thúc (sau khi hàm gọi lại success và error được thực thi).
    - `contents`: Một object của string hoặc REGEX dùng để xác định xem JQuery sẽ phân tích response như thế nào.
    - `contentType`: Kiểu nội dung của dữ liệu được gửi lên server.
    - `context`: Một object được dùng làm ngữ cảnh (this) của tất cả các hàm gọi lại liên quan đến Ajax.
    - `crossDomain`: Thiết lập thuộc tính này là true để buộc thực hiện request chéo giữa các domain (như là JSONP) trên cùng một domain.
    - `data`: Dữ liệu được gửi lên server khi thực thi một request Ajax.
    - `dataFilter`: Một hàm được dùng để xử lý các dữ liệu response thuần của một XMLHttpRequest.
    - `dataType`: Kiểu của dữ liệu mong muốn được trả về từ server.
    - `error`: Một hàm sẽ được gọi khi request fails.
    - `global`: Dùng để thiết lập xem có gọi các hàm xử lý sự kiện Ajax toàn cục cho request này hay không.
    - `headers`: Một object để viết thêm vào các header gửi lên server.
    - `ifModified`: Thiết lập giá trị này là true nếu bạn muốn buộc JQuery nhận diện môi trường hiện tại là "local".
    - `jsonp`: Một chuỗi dùng để override tên hàm gọi lại trong một request JSONP.
    - `jsonpCallback`: Chỉ định tên hàm gọi lại cho một request JSONP.
    - `mimeType`: Một chuỗi chỉ định kiểu mime dùng để override lại kiểu mime của XHR.
    - `password`: Mật khẩu được sử dụng với XMLHttpRequest cho response của một request yêu cầu xác thực truy nhập HTTP.
    - `processData`: Set giá trị này là false nếu bạn không muốn dữ liệu được truyền vào thiết lập data sẽ được xử lý và biến thành một query kiểu chuỗi.
    - `criptCharset`: Thiết lập thuộc tính charset của một thẻ script dùng cho một request nhưng chỉ áp dụng khi transport script (ví dụ: request chéo giữa các domain với jsonp) được sử dụng.
    - `statusCode`: Một object chứa các mã HTTP ở dạng số và các hàm được gọi khi response trả về có chứa một mã tương ứng.
    - `success`: Một hàm được gọi khi request thành công.
    - `timeout`: Số được thiết lập chỉ định thời gian hết hạn cho một request.
    - `traditional`: Thiết lập giá trị true nếu bạn mong muốn param được serialize theo kiểu truyền thống.
    - `type`: Kiểu request muốn thực hiện, có thể là POST hay GET …
    - `url`: Chuỗi chứa URL mà request được gửi đến.
    - `username`: Tên người dùng được sử dụng với XMLHttpRequest cho response của một request yêu cầu xác thực truy nhập HTTP.
    - `xhr`: Một hàm gọi lại dùng để tạo một object XMLHttpRequest.
    - `xhrFields`: Một object các key-value được thiết lập cho object XHR native.
- **VD1 :**
    - Khi sử dụng `load()` :
        ```js
        $('#main-menu a').click(function(event) {
          event.preventDefault();
          $('#main').load(this.href + ' #main *', function(responseText, status) {
            if (status === 'success') {
              $('#notification-bar').text('The page has been successfully loaded');
            } else {
              $('#notification-bar').text('An error occurred');
            }
          });
        });
        ```
    - Khi sử dụng `ajax()` :
        ```js
        $('#main-menu a').click(function(event) {
          event.preventDefault();
          $.ajax(this.href, {
            success: function(data) {
              $('#main').html($(data).find('#main *'));
              $('#notification-bar').text('The page has been successfully loaded');
            },
            error: function() {
                $('#notification-bar').text('An error occurred');
            }
          });
        });
        ```
- **VD2 :**
    - API : `https://api.joind.in/v2.1/talks/10889`
        
        <img src=https://i.imgur.com/d8nJO6r.png>

    - Lấy dữ liệu về từ API: 
        ```js
        $.ajax({
          url: 'http://api.joind.in/v2.1/talks/10889',
          data: {
            format: 'json'
          },
          error: function() {
            $('#info').html('<p>An error has occurred</p>');
          },
          dataType: 'jsonp',
          success: function(data) {
            var $title = $('<h1>').text(data.talks[0].talk_title);
            var $description = $('<p>').text(data.talks[0].talk_description);
            $('#info')
              .append($title)
              .append($description);
          },
          type: 'GET'
        });
        ```