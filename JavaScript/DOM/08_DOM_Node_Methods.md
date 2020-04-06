# DOM Node Methods
## **1) Tạo node mới - phương thức `appendChild()`**
- Để tạo một **node** mới, trước tiên phải tạo phần tử ( **element node** ) trước , sau đó thêm nó vào phần tử đã có sẵn .
- **VD :**
    ```html
    <div id="div1">
      <p id="p1">This is a paragraph.</p>
      <p id="p2">This is another paragraph.</p>
    </div>

    <script>
    var para = document.createElement("p");
    var node = document.createTextNode("[This is new.]");
    para.appendChild(node);

    var element = document.getElementById("div1");
    element.appendChild(para);
    </script>
    ```
    => Kết quả :
    
    ```
    This is a paragraph.
    This is another paragraph.
    [This is new.]
    ```
    - Giải thích :
        - **B1 :** Tạo phần tử `<p>` mới :
            ```js
            var para = document.createElement("p");
            ```
        - **B2 :** Để thêm text vào phần tử `<p>`, phải tạo **text node** :
            ```js
            var node = document.createTextNode("This is new.");
            ```
        - **B3 :** Thêm **text node** vào phần tử `<p>` :
            ```js
            para.appendChild(node);
            ```
        - **B4 :** Thêm phần tử mới vào phần tử đã có . Tìm phần tử sẵn có :
            ```js
            var element = document.getElementById("div1");
            ```
        - **B5 :** Thêm phần tử mới vào phần tử đã có :
            ```js
            element.appendChild(para);
            ```
## **2) Tạo node mới - phương thức `insertBefore()`**
- Sử dụng để đặt **node** mới tạo đứng trước một phần tử nào đó :
- **VD :**
    ```js
    <div id="div1">
      <p id="p1">This is a paragraph.</p>
      <p id="p2">This is another paragraph.</p>
    </div>

    <script>
    var para = document.createElement("p");
    var node = document.createTextNode("[This is new.]");
    para.appendChild(node);

    var element = document.getElementById("div1");
    var child = document.getElementById("p1");
    element.insertBefore(para, child);
    </script>
    ```
    - Kết quả :
    ```
    [This is new.]
    This is a paragraph.
    This is another paragraph.
    ```
## **3) Xóa phần tử - phương thức `remove()`**
- Để xóa một phần tử, sử dụng phương thức `remove()`
- **VD :**
    ```html
    <div>
      <p id="p1">This is a paragraph.</p>
      <p id="p2">This is another paragraph.</p>
    </div>

    <script>
    var elmnt = document.getElementById("p1");
    elmnt.remove();
    </script>
    ```
    => Kết quả :
    ```
    This is another paragraph.
    ```
    - Giải thích :
        - **B1 :** Tìm phần tử muốn xóa :
            ```js
            var elmnt = document.getElementById("p1");
            ```
        - **B2 :** Xóa phần tử :
            ```js
            elmnt.remove();
            ```
- Đối với những trình duyệt cũ, phương thức `remove()` sẽ không được hỗ trợ, phải dùng phương thức `removeChild()` . **VD :**
    ```html
    <div id="div1">
      <p id="p1">This is a paragraph.</p>
      <p id="p2">This is another paragraph.</p>
    </div>

    <script>
    var parent = document.getElementById("div1");
    var child = document.getElementById("p1");
    parent.removeChild(child);
    </script>
    ```
## **4) Thay thế phần tử - phương thức `replaceChild()`**
- Để thay thế một phần tử trong HTML DOM, sử dụng phương thức `replaceChild()` :
    ```html
    <div id="div1">
      <p id="p1">This is a paragraph.</p>
      <p id="p2">This is another paragraph.</p>
    </div>

    <script>
    var para = document.createElement("p");
    var node = document.createTextNode("This is new.");
    para.appendChild(node);

    var parent = document.getElementById("div1");
    var child = document.getElementById("p1");
    parent.replaceChild(para, child);
    </script>
    ```