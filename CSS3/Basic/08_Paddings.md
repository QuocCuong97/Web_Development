# CSS Paddings
## **1) CSS `padding`**
- Thuộc tính `padding` được sử dụng để tạo khoảng cách giữa nội dung của phần tử với border của phần tử .
- Với **CSS** , người lập trình có toàn quyền kiểm soát padding . Có rất nhiều thuộc tính để đặt padding cho mỗi phía của phần tử :
    - `padding-top`
    - `padding-right`
    - `padding-bottom`
    - `padding-left`
- Mỗi thuộc tính trên có thể chứa các giá trị sau :
    - `length` - chỉ định padding theo đơn vị `px`, `pt`, `cm`, ...
    - `%` - chỉ định padding theo `%` chiều rộng của phần tử chứa nó 
    - `inherit` - chỉ định padding sẽ kế thừa thông số padding của phần tử cha ( phần tử mà nó bị lồng ở trong )
- **VD :**
    ```html
    <style>
    div {
      border: 1px solid black;
      background-color: lightblue;
      padding-top: 50px;
      padding-right: 30px;
      padding-bottom: 50px;
      padding-left: 80px;
    }
    </style>
    <div>This div element has a top padding of 50px, a right padding of 30px, a bottom padding of 50px, and a left padding of 80px.</div>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/tMmVfeh.png>

## **2) CSS `padding` - Rút ngắn code**
- Để rút ngắn code, có thể khai báo tất cả 4 padding trong 1 dòng thuộc tính .
- Thuộc tính `padding` là thuộc tính rút gọn của 4 thuộc tính `padding-top`, `padding-right` , `padding-bottom`, `padding-left` .
- Thuộc tính `padding` có thể có từ `1` đến `4` giá trị ( cho `padding-top`, `padding-right` , `padding-bottom`, `padding-left` )
- Nếu không được khai báo đầy đủ các thông số trên, mặc định **CSS** sẽ hiểu :
    - `padding-top` = `padding-bottom`
    - `padding-right` = `padding-left`
- **VD :**
    ```css
    div {
      border: 1px solid black;
      padding: 25px 50px;
      background-color: lightblue;
    }
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/43aRCqx.png>

## **3) Padding và chiều rộng phần tử**
- Thuộc tính `width` chỉ định chiều rộng của nội dung phần tử . 
- Phần nội dung của phần tử là phần lõi bên trong padding->border->margin ( theo cấu trúc `box-model` )

<p align=center><img src=https://i.imgur.com/T2G1A7F.png width=60%></p>

- Vì vậy, nếu phần tử được chỉ định `width` , phần padding thêm vào phần tử đó cũng sẽ cộng thêm vào tổng chiều rộng của phần tử . Đây thường là một kết quả không mong muốn .
- **VD :** Ở đây, phần tử `<div>` được gán `width` là `300px` . Tuy nhiên, giá trị `width` thực tế của phần tử `<div>` lại là `350px` ( `300px + 25px + 25px` ) :
    ```css
    div {
      width: 300px;
      padding: 25px;
    }
    ```
    - Để giữ chiều rộng của phần tử là `300px` cho dù là có padding , có thể sử dụng thuộc tính `box-sizing` . Việc này sẽ giúp phần tử duy trì được chiều rộng của nó . Nếu tăng thêm `padding` , phần không gian nội dung bên trong sẽ tự động bị co lại .
        ```css
        div {
          width: 300px;
          padding: 25px;
          box-sizing: border-box;
        }
        ```

