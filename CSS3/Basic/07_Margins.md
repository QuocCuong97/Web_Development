# CSS Margins
## **1) CSS `margin`**
- Thuộc tính `margin` được sử dụng để tạo các khoảng trống quanh phần tử , tính từ rìa của border .
- Với **CSS** , người lập trình có toàn quyền kiểm soát margin (lề) . Có rất nhiều thuộc tính để đặt margin cho mỗi phía của phần tử :
    - `margin-top` : lề trên
    - `margin-right` : lề phải
    - `margin-bottom` : lề dưới
    - `margin-left` : lề trái
- Mỗi thuộc tính trên có thể chứa các giá trị sau :
    - `auto` - browser tự tính toán margin
    - `length` - chỉ định margin theo đơn vị `px`, `pt`, `cm`, ...
    - `%` - chỉ định margin theo `%` chiều rộng của phần tử chứa nó 
    - `inherit` - chỉ định margin sẽ kế thừa thông số margin của phần tử cha ( phần tử mà nó bị lồng ở trong )
- **VD :**
    ```css
    div {
      margin-top: 100px;
      margin-bottom: 100px;
      margin-right: 150px;
      margin-left: 80px;
    }
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/1JTKZl9.png>

### **Giá trị `auto`**
- Có thể để giá trị của thuộc tính `margin` là `auto` để căn giữa theo chiều ngang cho phần tử .
- Phần tử sẽ chiếm chiều rộng được chỉ định , phần không gian còn lại sẽ được chia đôi 1 cho lề trái và 1 cho lề phải .
- **VD :**
    ```css
    div {
      width: 300px;
      margin: auto;
      border: 1px solid red;
    }
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/WdBKwRQ.png>
### **Giá trị `inherit`**
- Phần tử có thuộc tính `margin: inherit` sẽ thừa kế thuộc tính `margin` của phần tử cha .
- **VD :**
    ```html
    <style>
    div {
      border: 1px solid red;
      margin-left: 100px;
    }

    p {
      margin-left: inherit;
    }
    </style>
    <div>
      <p>Ví dụ về Inherit</p>
    </div>
    ```
    - Trong ví dụ này , phần tử `<p>` sẽ kế thừa thuộc tính `margin-left: 100px` của phần tử `<div>`
## **2) CSS `margin` - Rút ngắn code**
- Để rút ngắn code, có thể khai báo tất cả 4 margin trong 1 dòng thuộc tính .
- Thuộc tính `margin` là thuộc tính rút gọn của 4 thuộc tính `margin-top`, `margin-right` , `margin-bottom`, `margin-left` .
- Thuộc tính `margin` có thể có từ `1` đến `4` giá trị ( cho `margin-top`, `margin-right` , `margin-bottom`, `margin-left` )
- Nếu không được khai báo đầy đủ các thông số trên, mặc định **CSS** sẽ hiểu :
    - `margin-top` = `margin-bottom`
    - `margin-right` = `margin-left`
- **VD :**
    ```css
    div {
      border: 1px solid black;
      margin: 25px 50px;
      background-color: lightblue;
    }
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/RAuKyFp.png>

## **3) Margin Collapse**
- `Top-margin` và `bottom-margin` của các phần tử đôi khi có sự xung đột và trở thành 1 margin có giá trị lớn nhất trong 2 margin .
- Trường hợp này chỉ xảy ra ở `top` và `bottom` , không xảy ra ở `left` và `right` .
- **VD :**
    ```html
    <style>
    h1 {
      margin: 0 0 50px 0;
    }

    h2 {
      margin: 20px 0 0 0;
    }
    </style>
    <h1>Heading 1</h1>
    <h2>Heading 2</h2>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/0l1BTtg.png>
        
    - Trong ví dụ này, thẻ `<h1>` có `margin-bottom` là `50px`, thẻ `<h2>` có `margin-top` là `20px` . Lẽ ra khoảng cách giữa chúng phải là `70px` nhưng vì hiện tượng **margin collapse** nên khoảng cách giữa chúng chỉ là `50px` .