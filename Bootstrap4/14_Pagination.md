# Pagination
## **1) Basic Pagination**
- Nếu website có nhiều trang, cần đến việc sắp xếp, phân chia thứ tự cho từng trang .
- Để tạo 1 thanh phân trang cơ bản , thêm class "`.pagination`" vào phần tử `<ul>` . Sau đó thêm các page-item vào mỗi phần tử `<li>` và class "`.page-link`" bên trong các phần tử `<li>` đó :
    ```html
    <ul class="pagination">
      <li class="page-item"><a class="page-link" href="#">Previous</a></li>
      <li class="page-item"><a class="page-link" href="#">1</a></li>
      <li class="page-item"><a class="page-link" href="#">2</a></li>
      <li class="page-item"><a class="page-link" href="#">3</a></li>
      <li class="page-item"><a class="page-link" href="#">Next</a></li>
    </ul>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/hYVFVoN.png>
## **2) Trạng thái `active` và `disabled`**
- Class "`.active`" được sử dụng để highlight trang hiện hành :
    ```html
    <li class="page-item active"><a class="page-link" href="#">2</a></li>
    ```
    - Hiển thị trên trình duyệt :  

        <img src=https://i.imgur.com/lnIBkmA.png>
- Class "`.disabled`" được sử dụng cho những link không thể click :
    ```html
    <li class="page-item disabled"><a class="page-link" href="#">Previous</a></li>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/4gg4odI.png>
## **3) Pagination Sizing**
- Thanh phân trang có thể có kích cỡ to hoặc nhỏ tùy ý :
    - Class "`.pagination-lg`" hiển thị thanh phân trang lớn hơn
    - Class "`.pagination-sm`" hiển thị thanh phân trang nhỏ hơn
    - Nếu không được khai báo, thanh phân trang sẽ hiển thị với kích cỡ mặc định .
- **VD :**
    ```html
    <ul class="pagination pagination-lg">
      <li class="page-item"><a class="page-link" href="#">1</a></li>
      <li class="page-item"><a class="page-link" href="#">2</a></li>
      <li class="page-item"><a class="page-link" href="#">Next</a></li>
    </ul>

    <ul class="pagination">
      <li class="page-item"><a class="page-link" href="#">1</a></li>
      <li class="page-item"><a class="page-link" href="#">2</a></li>
      <li class="page-item"><a class="page-link" href="#">Next</a></li>
    </ul>

    <ul class="pagination pagination-sm">
      <li class="page-item"><a class="page-link" href="#">1</a></li>
      <li class="page-item"><a class="page-link" href="#">2</a></li>
      <li class="page-item"><a class="page-link" href="#">Next</a></li>
    </ul>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/qCMLktj.png>

## **4) Pagination Alignment**
- Có thể sử dụng các tiện ích căn chỉnh của **Bootstrap4** để căn chỉnh cho thanh phân trang :
    - Mặc định : căn chỉnh trái
    - Class "`.justify-content-center`" : căn chỉnh giữa
    - Class " `.justify-content-end`" : căn chỉnh phải
- **VD :**
    ```html
    <!-- Default (left-aligned) -->
    <ul class="pagination" style="margin:20px 0">
      <li class="page-item">...</li>
    </ul>

    <!-- Center-aligned -->
    <ul class="pagination justify-content-center" style="margin:20px 0">
      <li class="page-item">...</li>
    </ul>

    <!-- Right-aligned -->
    <ul class="pagination justify-content-end" style="margin:20px 0">
      <li class="page-item">...</li>
    </ul>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/c2qHSIG.png>

## **5) Breadcrumbs**
- Một dạng khác của phân trang là **breadcrumb** .
- Class "`.breadcrumb`" và "`.breadcrumb-item`" chỉ ra vị trí của trang hiện hành trong một cấu trúc web phân cấp :
    ```html
    <ul class="breadcrumb">
      <li class="breadcrumb-item"><a href="#">Photos</a></li>
      <li class="breadcrumb-item"><a href="#">Summer 2017</a></li>
      <li class="breadcrumb-item"><a href="#">Italy</a></li>
      <li class="breadcrumb-item active">Rome</li>
    </ul>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/gVLbCgL.png>
