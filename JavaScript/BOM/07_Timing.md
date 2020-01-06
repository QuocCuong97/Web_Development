# Timing Events
- **Object** `window` cho phép thực thi câu lệnh vào 1 khoảng thời gian được chỉ định trước .
- Những khoảng thời gian này được gọi là **timing events** .
- Có 2 phương thức để sử dụng **timing event** trong **JavaScript** :
    - `setTimeout()`
    - `setInterval()`
## **1) Phương thức `setTimeout()`**
- Được sử dụng để thực hiện 1 hàm, sau khi chờ một khoảng thời gian tính bằng ***miliseconds*** .
- Cú pháp :
    ```js
    window.setTimeout(function, milliseconds);
    ```
- Phương thức `window.setTimeout()` có thể được gọi mà không cần tiền tố `window` .
- **VD :** Sau khi click button, 3s sau sẽ xuất hiện **alert box** :
    ```html
    <button onclick="setTimeout(myFunction, 3000)">Try it</button>

    <script>
    function myFunction() {
      alert('Hello');
    }
    </script>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/DWGeYdv.png>
## **2) Phương thức `clearTimeout()`**
- Được sử dụng để dừng thực thi hàm đã chỉ định trong `setTimeout()` .
    ```js
    window.clearTimeout(timeoutVariable)
    ```
- Phương thức `window.clearTimeout()` có thể được gọi mà không cần tiền tố `window` .
- Phương thức `clearTimeout()` sử dụng biến trả về từ `setTimeout()` :
    ```js
    myVar = setTimeout(function, milliseconds);
    clearTimeout(myVar);
    ```
    => Trong khoảng thời gian hàm chưa được thực thi, có thể sử dụng `clearTimeout()` để dừng hàm lại .
- **VD :**
    ```html
    <button onclick="myVar = setTimeout(myFunction, 3000)">Try it</button>

    <button onclick="clearTimeout(myVar)">Stop it</button>
    ```
## **3) Phương thức `setInterval()`**
- Được sử dụng để lặp lại 1 hàm cho trước vào từng khoảng thời gian ***miliseconds*** cho trước .
- Cú pháp :
    ```js
    window.setInterval(function, milliseconds);
    ```
- Phương thức `window.setInterval()` có thể được gọi mà không cần tiền tố `window` .
- **VD :** Tạo đồng hồ điện tử :
    ```js
    var myVar = setInterval(myTimer, 1000);

    function myTimer() {
    var d = new Date();
      document.getElementById("demo").innerHTML = d.toLocaleTimeString();
    }
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/SxdFa84.png>

## **4) Phương thức `clearInterval()`**
- Được sử dụng để dừng thực thi hàm đã chỉ định trong `setInterval()` .
    ```js
    window.clearInterval(timerVariable)
    ```
- Phương thức `window.clearInterval()` có thể được gọi mà không cần tiền tố `window` .
- Phương thức `clearInterval()` sử dụng biến trả về từ `setInterval()` :
    ```js
    myVar = setInterval(function, milliseconds);
    clearInterval(myVar);
    ```
    => Trong khoảng thời gian hàm chưa được thực thi, có thể sử dụng `clearInterval()` để dừng hàm lại .
- **VD :**
    ```html
    <p id="demo"></p>

    <button onclick="clearInterval(myVar)">Stop time</button>

    <script>
    var myVar = setInterval(myTimer, 1000);
    function myTimer() {
      var d = new Date();
      document.getElementById("demo").innerHTML = d.toLocaleTimeString();
    }
    </script>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/pUrSPnV.png>