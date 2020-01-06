# Popup Box
- **JavaScript** có 3 loại popup box : **Alert box**, **Confirm box** và **Prompt box** .
## **1) Alert Box**
- **Alert box** thường được sử dụng khi muốn đảm bảo một thông tin đến tận mắt user .
- Khi **alert box** xuất hiện, user cần click "`OK`" để tắt nó .
- Cú pháp :
    ```js
    window.alert("sometext");
    ```
- Phương thức `window.alert()` có thể được gọi mà không cần tiền tố `window` .
- **VD :**
    ```js
    alert("I am an alert box!");
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/9sSu9Pl.png>
## **2) Confirm Box**
- **Confirm box** thường được sử dụng khi muốn user xác nhận hoặc đồng ý một điều gì đó .
- Khi **confirm box** xuất hiện , user phải click vào "`OK`" hoặc "`Cancel`" để kết thúc nó .
- Nếu user click "`OK`", box sẽ trả về `true` . Nếu user click "`Cancel`", box sẽ trả về `false` .
- Cú pháp :
    ```js
    window.confirm("sometext");
    ```
- Phương thức `window.confirm()` có thể được gọi mà không cần tiền tố `window` .
- **VD :**
    ```js
    if (confirm("Press a button!")) {
      txt = "You pressed OK!";
    } else {
      txt = "You pressed Cancel!";
    }
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/bdq7nXq.png>

## **3) Prompt Box**
- **Prompt box** thường được sử dụng nếu muốn user nhập vào một số giá trị trước khi đi vào trang web .
- Khi **prompt box** xuất hiện , user sẽ phải click vào "`OK`" hoặc "`Cancel`" để kết thúc sau khi nhập giá trị vào trường input .
- Nếu user click "`OK`" , box sẽ trả về giá trị trường input . Nếu user click "`Cancel`", box sẽ trả về `null` .
- Cú pháp :
    ```js
    window.prompt("sometext","defaultText");
    ```
- Phương thức `window.prompt()` có thể được gọi mà không cần tiền tố `window` .
- **VD :**
    ```js
    var person = prompt("Please enter your name", "Harry Potter");

    if (person == null || person == "") {
      txt = "User cancelled the prompt.";
    } else {
      txt = "Hello " + person + "! How are you today?";
    }
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/arRkMJ2.png>