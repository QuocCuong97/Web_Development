# Computer Code
## **1) Phần tử `<kbd>`**
- Phần tử `<kbd>` đại diện cho input của người dùng, như input từ bàn phím, hoặc input từ giọng nói .
- Phần chữ trong cặp thẻ `<kbd>` sẽ được hiển thị bằng font `monospace` .
- **VD :**
    ```html
    <p>Save the document by pressing <kbd>Ctrl + S</kbd></p>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/1MUg8n4.png>

## **2) Phần tử `<samp>`**
- Phần tử `<samp>` đại diện cho phần output từ 1 chương trình hoặc một hệ thống máy tính .
- Phần chữ trong cặp thẻ `<samp>` sẽ được hiển thị bằng font `monospace` .
- **VD :**
    ```html
    <p>If you input wrong value, the program will return <samp>Error!</samp></p>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/NakDlss.png>

## **3) Phần tử `<code>`**
- Phần tử `<code>` định nghĩa 1 đoạn code máy tính .
- Phần chữ trong cặp thẻ `<code>` được hiển thị bằng font `monospace` .
- **VD :**
    ```html
    <code>
    x = 5;
    y = 6;
    z = x + y;
    </code>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/gW4MAkf.png>

- Chú ý : Phần tử `<code>` không bảo toàn khoảng trắng và ngắt dòng bổ sung . Để sửa việc này, đặt phần tử `<code>` trong cặp thẻ `<pre>` .
    ```html
    <pre>
    <code>
    x = 5;
    y = 6;
    z = x + y;
    </code>
    </pre>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/hKTB4BD.png>

## **4) Phần tử `<var>`**
- Phần tử `<var>` định nghĩa 1 biến .
- Biến ở đây có thể là biến trong biểu thức toán học hoặc biến trong ngữ cảnh lập trình .
- **VD :**
    ```html
    <p>Einstein wrote: <var>E</var> = <var>mc</var><sup>2</sup></p>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/aab7Tkh.png>
