# Debugging
## **1) Trình debugger**
- Code luôn có thể ẩn chứa các lỗi cú pháp, hoặc lỗi logic .
- Nhiều lỗi rất khó để phân tích .
- Thông thường , khi code chứa lỗi, không có gì xảy ra . Sẽ không có tin nhắn cảnh báo lỗi hoặc chỉ thị để tìm kiếm lỗi .
- Việc tìm kiếm và sửa lỗi trong lập trình được gọi là **code debugging** .
- **Debug** là một việc không dễ . Nhưng may mắn thay, các trình duyệt hiện đại đã tích hợp sẵn 1 trình debug **JavaScript** .
- Trình **debug** có thể được bật hoặc tắt đi, bám theo lỗi để cảnh báo tới user .
- Với trình **debug** , có thể đặt các **breakpoint** (nơi mà phần code thực thi sẽ bị dừng lại ) để kiểm tra phần lỗi bên trong nó .
- Có thể kích hoạt trình **debug** trên trình duyệt bằng cách ấn phím `F12` , chọn `Console` trong menu debug :
    
    <img src=https://i.imgur.com/U9fCR7a.png>

## **2) Từ khóa `debugger`**
- Từ khóa `debugger` sẽ dừng thực thi các đoạn code **JavaScript** bên dưới nó, và gọi các hàm debug, nếu có thể .
- Việc này tương tự như đặt dấu breakpoint trong trình **debug** .
- **VD :**
    ```js
    var x = 15 * 5;
    debugger;
    document.getElementById("demo").innerHTML = x;
    ```