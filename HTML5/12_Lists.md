# Lists
## **1) Giới thiệu**
- **HTML** hỗ trợ 3 kiểu list : 
    - List có thứ tự
    - List không thứ tự 
    - List mô tả
## **2) List không thứ tự ( *unordered list* )**
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

## **3) List có thứ tự ( *ordered list* )**
- Một list theo thứ tự được bắt đầu bằng thẻ `<ol>` ( *ordered list* ) . Bên trong thẻ này sẽ có các thẻ `<li>` với mỗi thẻ `<li>` ứng với một mục trong list .
- Khi hiển thị list có thứ tự trên trình duyệt mỗi hạng mục trong list sẽ được hiển thị mặc định với số thứ tự tăng dần bắt đầu từ `1` ở phía trước .
### **Kiểu đánh số thứ tự**
- Các kiểu đánh số list : có thể sử dụng thuộc tính `type` để hiển thị một trong các kiểu đánh dấu sau dành cho list có thứ tự :
    - `type="1"` : đánh số theo số tự nhiên bắt đầu từ `1 -> 2 -> 3...` Đây là kiểu đánh số thứ tự mặc định.
        ```html
        <ol type="1">
          <li>Iron Man</li>
          <li>Hawkeye</li>
          <li>Captain America</li>
          <li>Falcon</li>
        </ol>
        ```
        <img src=https://i.imgur.com/5dxAsgC.png>
    - `type="A"` : đánh số theo chữ cái in hoa bắt đầu từ `A -> B -> C...`
        ```html
        <ol type="A">
          <li>Iron Man</li>
          <li>Hawkeye</li>
          <li>Captain America</li>
          <li>Falcon</li>
        </ol>
        ```
        <img src=https://i.imgur.com/0iJwmVh.png>
    - `type="a"` : đánh số theo chữ cái in thường bắt đầu từ `a -> b -> c...`
        ```html
        <ol type="a">
          <li>Iron Man</li>
          <li>Hawkeye</li>
          <li>Captain America</li>
          <li>Falcon</li>
        </ol>
        ```
        <img src=https://i.imgur.com/J6SH82w.png>
    - `type="I"` : đánh số theo chữ số la mã in hoa bắt đầu từ `I -> II -> III...`
        ```html
        <ol type="I">
          <li>Iron Man</li>
          <li>Hawkeye</li>
          <li>Captain America</li>
          <li>Falcon</li>
        </ol>
        ```
        <img src=https://i.imgur.com/nzRifV0.png>
    - `type="i"` : đánh số theo chữ số la mã in thường bắt đầu từ `i -> ii -> iii...`
        ```html
        <ol type="i">
          <li>Iron Man</li>
          <li>Hawkeye</li>
          <li>Captain America</li>
          <li>Falcon</li>
        </ol>
        ```
        <img src=https://i.imgur.com/by3nLmi.png>

### **Thay đổi số thứ tự bắt đầu hạng mục**
- Sử dụng thuộc tính `start` chúng ta có thể thay đổi số thứ thự của hạng mục đầu tiên trong list có thứ tự .
- **VD1 :** kiểu đánh số với số tự nhiên , bắt đầu từ `11` :
    ```html
    <ol type="1" start="11">
      <li>Iron Man</li>
      <li>Hawkeye</li>
      <li>Captain America</li>
      <li>Falcon</li>
    </ol>
    ```
    <img src=https://i.imgur.com/SgWFZW0.png>
- **VD2 :** kiểu đánh số theo chữ cái in thường , bắt đầu từ `e` ( là chữ cái thứ `5` ) :
    ```html
    <ol type="a" start="5">
      <li>Iron Man</li>
      <li>Hawkeye</li>
      <li>Captain America</li>
      <li>Falcon</li>
    </ol>
    ```
    <img src=https://i.imgur.com/d1sydEu.png>
## **4) List mô tả**
- Với list mô tả mỗi một mục sẽ được thêm một mô tả phía trước thay vì đánh số hoặc dấu chấm tròn .
- List mô tả được bắt đầu bằng thẻ `<dl>` ( *definition list* ) . Bên trong thẻ này sẽ có các thẻ `<dd>` với mỗi thẻ `<dd>` ứng với một mục trong danh sách . Trước mỗi hạng mục để thêm mô tả sử dụng thẻ `<dt>` .
    ```html
    <dl>
      <dt>Năm 2008</dt>
        <dd>Iron Man</dd>
      <dt>Năm 2011</dt>
        <dd>Captain America</dd>
      <dt>Năm 2019</dt>
        <dd>Hawkeye</dd>
        <dd>Falcon</dd>
    </dl>
    ```
    <img src=https://i.imgur.com/ocJdp5T.png>
