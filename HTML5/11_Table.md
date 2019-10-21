# Table
## **1) Giới thiệu**
- Trong **HTML** thẻ `<table>` được sử dụng để đánh dấu một bảng .
- Thẻ `<table>` được sử dụng kết hợp cùng các thẻ khác như `<thead>`, `<tbody>`, `<tr>` và `<td>` để tạo thành các phần nội dung cụ thể của bảng .
    - Thẻ `<tbody>` dùng để đánh dấu phần nội dung của bảng
    - Thẻ `<tr>` dùng để đánh dấu các dòng (row) trong bảng
    - Thẻ `<th>` dùng để đánh dấu tên các cột trong bảng. Nội dung bên trong thẻ này được trình duyệt hiển thị với chữ in đậm.
    - Thẻ `<td>` dùng để đánh dấu giá trị của các cột trong từng dòng
    > Giá trị đặt trong các cặp thẻ `<td>` và `<th>` không nhất thiết phải là văn bản mà có thể là link hoặc hình ảnh...
- **VD :**
    ```html
    <table>
        <tbody>
            <tr>
                <th>Tên Cột 1</th>
                <th>Tên Cột 2</th>
                <th>Tên Cột 3</th>
            <tr>
            <tr>
                <td>Giá Trị Cột 1</td>
                <td>Giá Trị Cột 2</td>
                <td>Giá Trị Cột 3</td>
            </tr> 
        </tbody>
    </table>
    ```
    => Hiển thị trên trình duyệt :

    <img src=https://i.imgur.com/wgvhzXB.png>

## **2) Thẻ `<thread>`**
- Thông thường , ta sẽ nhóm dòng chứa tên cột trong bảng trong thẻ `<thead>` để phân biệt với phần nội dung chính của bảng được đặt trong thẻ `<tbody>` :
    ```html
    <table>
        <thead>
            <tr>
                <th>Tên Cột 1</th>
                <th>Tên Cột 2</th>
                <th>Tên Cột 3</th>
            <tr>
        </thead>
        <tbody>
            <tr>
                <td>Giá Trị Cột 1</td>
                <td>Giá Trị Cột 2</td>
                <td>Giá Trị Cột 3</td>
            </tr> 
        </tbody>
    </table>
    ```
    => Hiển thị trên trình duyệt :

    <img src=https://i.imgur.com/wgvhzXB.png>

## **3) Tạo đường viền cho bảng**
- Trình duyệt sẽ không hiển thị đường viền của bảng trừ khi được thêm vào .
- Thêm đường viền cho bảng chúng ta cần sử dụng **CSS** với đặc tính `border` :
    ```html
    <style>
    table, th, td {
        border: 1px solid black;
    }
    </style>
    ```
    => Hiển thị trên trình duyệt :

    <img src=https://i.imgur.com/o9XrPn8.png>

- Như ví dụ trên , các đường viền của phần tử `<th>` và `<td>` được đặt cạnh đường viền của phần tử tbody và sẽ tạo ra 2 đường viền nằm cạnh nhau . Để gộp các đường viền cạnh nhau lại chúng ta có thể sử dụng thêm đặc tính `border-collapse` của **CSS** :
    ```html
    <style>
    table, th, td {
        border: 1px solid black;
        border-collapse: collapse;
    }
    </style>
    ```
    => Hiển thị trên trình duyệt :

    <img src=https://i.imgur.com/w5qApf4.png>

## **4) Thay đổi độ rộng của bảng**
- Để quy định động rộng của bảng chúng ta có thể sử dụng đặc tính `width` của **CSS** .
    ```html
    <table style="width: 100%">
    ```
## **5) Gộp các cột trong cùng dòng**
- Để gộp các cột trong cùng dòng chúng ta có thể sử dụng đặc tính `colspan` của **CSS** .
    ```html
    <table style="width: 30%">
        <tr>
            <th>Họ Tên</th>
            <th colspan="2">Số ĐT</th>
        </tr>
        <tr>
            <td>Ngô Quốc Cường</td>
            <td>0944693xxx</td>
            <td>0986048xxx</td>
        </tr>
    </table>
    ```
    => Hiển thị trên trình duyệt :

    <img src=https://i.imgur.com/B05k7aO.png>

## **6) Gộp các dòng trong cùng cột**
- Để gộp các cột trong cùng dòng chúng ta có thể sử dụng đặc tính `rowspan` của **CSS** .
    ```html
    <table style="width: 30%">
        <tr>
            <th>Họ Tên</th>
            <th>Số ĐT</th>
        </tr>
        <tr>
            <th rowspan="2">Số Điện Thoại:</th>
            <td>093421122</td>
        </tr>
        <tr>
            <td>012345678</td>
        </tr>
    </table>
    ```
    => Hiển thị trên trình duyệt :
    
    <img src=https://i.imgur.com/eRjZrJr.png>