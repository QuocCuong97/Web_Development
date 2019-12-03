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
### **Giá trị `inherit`**
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
