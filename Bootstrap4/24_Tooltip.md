# Tooltip
## **1) Cơ bản về Tooltip**
- **Tooltip** là một hộp thoại pop-up nhỏ xuất hiện khi user di chuyển con trỏ chuột qua phần tử .
- Để tạo 1 **tooltip** , thêm thuộc tính `data-toggle="tooltip"` vào phần tử .
- Sử dụng thuộc tính `title` để chỉ định đoạn text sẽ hiển thị bên trong **tooltip** .
- **VD :**
    ```html
    <a href="#" data-toggle="tooltip" title="Hooray!">Hover over me</a>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/xuN20EZ.png>
## **2) Vị trí của tooltip**
- Mặc định, **tooltip** sẽ xuất hiện ở phía trên của phần tử .
- Sử dụng thuộc tính `data-placement` để set position cho **tooltip** sẽ xuất hiện ở trên, dưới , trái, phải của phần tử :
    ```html
    <a href="#" data-toggle="tooltip" data-placement="top" title="Hooray!">Hover</a>
    <a href="#" data-toggle="tooltip" data-placement="bottom" title="Hooray!">Hover</a>
    <a href="#" data-toggle="tooltip" data-placement="left" title="Hooray!">Hover</a>
    <a href="#" data-toggle="tooltip" data-placement="right" title="Hooray!">Hover</a>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/ottS9ll.png>
