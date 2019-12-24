# Popover
## **1) Cơ bản về Popover**
- **Popover** về cơ bản giống với **tooltip** , là một hộp thoại pop-up xuất hiện khi user click vào phần tử .
- Điểm khác biệt là **popover** có thể chứa nhiều nội dung hơn **tooltip** .
- Để tạo ra một **popover** , thêm thuộc tính `data-toggle="popover"` vào phần tử .
- Sử dụng thuộc tính `title` để chỉ định header cho đoạn text trong **popover**, thuộc tính `data-content` để chỉ định đoạn text xuất hiện ở phần body trong **popover** .
- **VD :**
    ```html
    <a href="#" data-toggle="popover" title="Popover Header" data-content="Some content inside the popover">Toggle popover</a>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/H7nYO0V.png>

## **2) Vị trí của Popover**
- Mặc định, **popover** sẽ xuất hiện ở phía trên của phần tử .
- Sử dụng thuộc tính `data-placement` để set position cho **popover** sẽ xuất hiện ở trên, dưới , trái, phải của phần tử :
    ```html
    <a href="#" title="Header" data-toggle="popover" data-placement="top" data-content="Content">Click</a>
    <a href="#" title="Header" data-toggle="popover" data-placement="bottom" data-content="Content">Click</a>
    <a href="#" title="Header" data-toggle="popover" data-placement="left" data-content="Content">Click</a>
    <a href="#" title="Header" data-toggle="popover" data-placement="right" data-content="Content">Click</a>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/EJacROR.png>
## **3) Đóng Popover**
- Mặc định, **popover** sẽ được đóng khi user click vào phần tử 1 lần nữa .
- Tuy nhiên, có thể sử dụng thuộc tính `data-trigger="focus"` để đóng **popover** bất cứ khi nào user click ra ngoài phần tử .
    ```html
    <a href="#" title="Dismissible popover" data-toggle="popover" data-trigger="focus" data-content="Click anywhere in the document to close this popover">Click me</a>
    ```
- Nếu muốn **popover** được hiển thị khi di chuyển chuột qua phần tử giống như **tooltip**, có thể sử dụng thuộc tính `data-trigger="hover"` :
    ```html
    <a href="#" title="Header" data-toggle="popover" data-trigger="hover" data-content="Some content">Hover over me</a>
    ```