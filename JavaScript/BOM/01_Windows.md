# Window - BOM
- **BOM - Browser Object Model** cho phép **JavaScript** giao tiếp với trình duyệt .
- Chưa có một chuẩn chính thức nào cho **BOM** .
- Do hầu hết các trình duyệt hiện đại đã triển khai các phương thức và thuộc tính tương tự cho tính tương tác **JavaScript**, nên nó thường được gọi là phương thức và thuộc tính của **BOM** .
## **1) Window Object**
- **Window object** được hỗ trợ bởi tất cả các trình duyệt . Nó đạu diện cho cửa sổ trình duyệt .
- Tất cả các **object** , **function**, biến **global** của **JavaScript** tự động trở thành phần tử của **window object** .
- Các biến **global** là các thuộc tính của **window object** .
- Các hàm **global** là cac phương thức của **window object** .
- Thậm chí các **document object** ( **DOM** ) cũng là thuộc tính của **window object** :
    ```js
    window.document.getElementById("header");
    ```
    tương tự với :
    ```js
    document.getElementById("header");
    ```
## **2) Window Size**
- Có hai thuộc tính được sử dụng để xác định kích thước của cửa sổ trình duyệt . 2 thuộc tính này sẽ trả về kích cỡ theo đơn vị `pixels` :
    - `window.innerHeight` - Chiều cao của cửa sổ trình duyệt (`pixel`)
    - `window.innerWidth` - Chiều rộng của cửa sổ trình duyệt (`pixel`)
    > Cửa sổ trình duyệt ở đây chỉ tính phần web được hiển thị, không tính thanh **toolbar** và **scrollbar** .
- **VD :**
    ```js
    var w = window.innerWidth

    var h = window.innerHeight

    var x = document.getElementById("demo");
    x.innerHTML = "Browser inner window width: " + w + ", height: " + h + ".";
    ```
    => Kết quả : `Browser inner window width: 753, height: 573.`
## **3) Các phương thức window khác**
- `window.open()` - mở 1 cửa sổ mới
- `window.close()` - đóng cửa sổ hiện tại
- `window.moveTo()` - di chuyển cửa sổ hiện tại
- `window.resizeTo()` - thay đổi kích cỡ cửa sổ hiện tại .
