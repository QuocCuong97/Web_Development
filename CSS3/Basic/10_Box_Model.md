# Box Model
- Tất cả các phần tử **HTML** có thể được coi như các box . Trong **CSS**, luật "box model" được nói đến trong thiết kết bố cục .
- **CSS box model** là một cấu trúc box thiết yếu đối với mọi phần tử **HTML** . Nó bao gồm : **margins**, **borders**, **paddings**, và nội dung của phần tử :

    <img src=https://i.imgur.com/vqBPChI.png>

- Trong đó :
    - **Content** : nội dung của phần tử ( ví dụ : text, hình ảnh...)
    - **Padding** : phần không gian trống bao quanh **content** . **Padding** là hoàn toàn trong suốt .
    - **Border** : là phần đường viền bao quanh **padding** và **content** .
    - **Margin** : là phần không gian trống bên ngoài **border** . **Margin** là hoàn toàn trong suốt .
- **Box model** cho phép ta định nghĩa border quanh phần tử , định nghĩa khoảng cách giữa các phần tử .
- **VD :** 
    ```css
    div {
      width: 300px;
      border: 15px solid green;
      padding: 50px;
      margin: 20px;
    }
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/AZJensv.png>

## **Chiều rộng và chiều dài của phần tử**
- Để set chính xác chiều cao và chiều rộng của 1 phần tử, cần biết chính xác cách hoạt động của **box model** .
- Tổng chiều rộng của phần tử sẽ được tính theo công thức :
    ```
    Tổng chiều rộng phần tử = width + padding-left + padding-right + border-left + border-right + margin-left + margin-right
    ```
- Tổng chiều cao của phần tử sẽ được tính theo công thức :
    ```
    Tổng chiều cao phần tử = height + padding-top + padding-bottom + border-top + border-bottom + margin-top + margin-bottom
    ```
- **VD :**
    ```css
    div {
      width: 320px;
      padding: 10px;
      border: 5px solid gray;
      margin: 0;
    }
    ```
    - Trong trường hợp này :
        ```
        Tổng chiều rộng = 320px + 10px*2 + 5px*2 + 0*2 = 350px
        ```