# Tables
## **1) Class "`.table`"**
- Một table cơ bản trong **Bootstrap4** có một chút padding và kẻ ngang giữa các dòng .
- Class cơ bản để định kiểu như vậy cho table là "`.table`"
- **VD :**
    ```html
    <div class="container">       
      <table class="table">
        <thead>
          <tr>
            <th>Firstname</th>
            <th>Lastname</th>
            <th>Email</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td>John</td>
            <td>Doe</td>
            <td>john@example.com</td>
          </tr>
          <tr>
            <td>Mary</td>
            <td>Moe</td>
            <td>mary@example.com</td>
          </tr>
          <tr>
            <td>July</td>
            <td>Dooley</td>
            <td>july@example.com</td>
          </tr>
        </tbody>
      </table>
    </div>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/G9IKD8q.png>

## **2) Class "`.table-stripped`"**
- Class "`.table-stripped`" sẽ thêm màu đậm nhạt xen kẽ cho các hàng :
- **VD :**
    ```html
    <table class="table table-striped">
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/8Zaopor.png>

## **3) Class "`.table-bordered`"**
- Class "`.table-bordered`" sẽ thêm các đường border vào tất cả các phía của các ô và cả table .
- **VD :**
    ```html
    <table class="table table-bordered">
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/LrRIctq.png>

## **4) Class "`.table-hover`"**
- Class "`.table-hover`" sẽ thêm hiệu ứng ( nền màu xám ) cho hàng nào có con trỏ chuột di qua .
- **VD :**
    ```html
    <table class="table table-hover">
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/CiUCDk0.png>

## **5) Class "`.table-dark`"**
- Class "`.table-dark`" sẽ thêm nền đen cho table .
- **VD1 :**
    ```html
    <table class="table table-dark">
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/57RC6cp.png>
- **VD2 :**
    ```html
    <table class="table table-dark table-striped">
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/a0hIsEq.png>

## **6) Class "`.table-borderless`"**
- Class "`.table-borderless`" sẽ xóa bỏ hết các đường border trong table kể cả các border có sẵn từ đầu .
- **VD :**
    ```html
    <table class="table table-borderless">
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/e45aEVS.png>

## **7) Class "`.thead-dark`" và "`.thead-light`"**
- Class "`.thead-dark`" thêm nền đen vào hàng tiêu đề của table .
- Class "`.thead-light`" thêm nền xám vào hàng tiêu để của table .
- **VD1 :**
    ```html
    <table class="table">
      <thead class="thead-dark">
        <tr>
          <th>Firstname</th>
          <th>Lastname</th>
          <th>Email</th>
        </tr>
      </thead>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/fZEe6nk.png>

- **VD2 :**
    ```html
    <table class="table">
      <thead class="thead-light">
        <tr>
          <th>Firstname</th>
          <th>Lastname</th>
          <th>Email</th>
        </tr>
      </thead>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/H6Sm6iY.png>

## **8) Class "`.table-sm`"**
- Class "`.table-sm`" làm cho table nhỏ hơn bằng cách giảm padding của các cell đi một nửa .
- **VD :**
    ```html
    <table class="table table-bordered table-sm">
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/2GLwxbz.png>

## **9) Contextual Classes**
## **10) Class "`.table-responsive`"**
- Class "`.table-responsive`" sẽ tạo ra một responsive table : một thanh trượt ngang sẽ được thêm vào nếu chiều rộng màn hình nhỏ hơn `992px` ( nếu cần thiết ) . Còn các màn hình rộng hơn `992px` thì không có gì khác biệt .
- **VD :**
    ```html
    <div class="container">
      <div class="table-responsive">
        <table class="table table-bordered">
        ....
        </table>
      </div>
    </div>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/pQ5TpCt.png>

- Có thể tự quyết định khi nào table sẽ hiện cùng thanh trượt ngang dựa vào chiều rộng màn hình :

    | Class | Chiều rộng màn hình |
    |-------|---------------------|
    | `.table-responsive-sm` | `< 576px` |
    | `.table-responsive-md` | `< 768px` |
    | `.table-responsive-lg` | `< 992px` |
    | `.table-responsive-xl` | `< 1200px` |

- **VD2 :**
    ```html
    <div class="container">
      <div class="table-responsive-sm">
        <table class="table table-bordered">
        ....
        </table>
      </div>
    </div>
    ```
