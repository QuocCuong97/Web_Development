# Lists
## **1) Giới thiệu**
- **HTML** hỗ trợ 3 kiểu list : 
    - List có thứ tự
    - List không thứ tự 
    - List mô tả
## **2) List không thứ tự ( *Unordered HTML List* )**
- Một list không theo thứ tự được bắt đầu bằng thẻ `<ul>` ( *unordered list* ) . Bên trong thẻ này sẽ có các thẻ `<li>` với mỗi thẻ `<li>` ứng với một mục trong list .
    ```html
    <ul>
      <li>Iron Man</li>
      <li>Hawkeye</li>
      <li>Captain America</li>
      <li>Falcon</li>
    </ul>
    ```
    => Hiển thị trên trình duyệt :

    <img src=https://i.imgur.com/Enlw6cv.png>

- Các kiểu đánh dấu list : Với đặc tính `list-style-type` trong **CSS** , có thể sử dụng một trong các kiểu đánh dấu sau dành cho list không có thứ tự :
    - `list-style-type: disc` : đánh dấu list sử dụng dấu chấm ( &#9679; ) ở phía trước (kiểu mặc định) .
        ```html
        <ul style="list-style-type: disc;">
          <li>Iron Man</li>
          <li>Hawkeye</li>
          <li>Captain America</li>
          <li>Falcon</li>
        </ul>
        ```
        <img src=https://i.imgur.com/Enlw6cv.png>
    - `list-style-type: circle`: đánh dấu list sử dụng dấu hình tròn ( &#9675; ) ở phía trước .
        ```html
        <ul style="list-style-type: circle;">
          <li>Iron Man</li>
          <li>Hawkeye</li>
          <li>Captain America</li>
          <li>Falcon</li>
        </ul>
        ```
        <img src=https://i.imgur.com/5oqxMgf.png>
    - `list-style-type: square` : đánh dấu list sử dụng dấu hình vuông ( &#9632; ) ở phía trước .
        ```html
        <ul style="list-style-type: square;">
          <li>Iron Man</li>
          <li>Hawkeye</li>
          <li>Captain America</li>
          <li>Falcon</li>
        </ul>
        ```
        <img src=https://i.imgur.com/vhr4zmE.png>
    - `list-style-type: none` : không đánh dấu bất cứ hạng mục nào trong list .
        ```html
        <ul style="list-style-type: none;">
          <li>Iron Man</li>
          <li>Hawkeye</li>
          <li>Captain America</li>
          <li>Falcon</li>
        </ul>
        ```
        <img src=https://i.imgur.com/oO92q3i.png>


