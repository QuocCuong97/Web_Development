# Grids
## **1) Hệ thống grid của Bootstrap4**
- Hệ thống các **grid** trong **Bootstrap4** được tạo ra bởi các flexbox và cho phép tối đa 12 cột theo chiều ngang .
- Nếu không muốn sử dụng riêng rẽ 12 cột , có thể nhóm các cột lại với nhau tạo thành cột rộng hơn .
- Hệ thống **grid** là responsive , các cột có thể tự động được sắp xếp lại dựa theo kích cỡ màn hình .

    <img src=https://i.imgur.com/o6sSh40.png>

## **2) Grid Classes**
- Hệ thống **grid** trong **Bootstrap4** có 5 class :
    - `.col` - ( thiết bị siêu nhỏ - chiều rộng màn hình `<576px` )
    - `.col-sm` - ( thiết bị trung bình - chiều rộng màn hình <code>&ge;576px</code> )
    - `.col-md` - ( thiết bị trung bình - chiều rộng màn hình <code>&ge;768px</code> )
    - `.col-lg` - ( thiết bị lớn - chiều rộng màn hình <code>&ge;992px</code> )
    - `.col-xl` - ( thiết bị siêu lớn - chiều rộng màn hình <code>&ge;1200px</code> )
- Các class có thể được kết hợp với nhau để tạo ra các layout động và linh hoạt .
- Code tạo **grid** cơ bản :
    ```html
    <!-- Control the column width, and how they should appear on different devices -->
    <div class="row">
      <div class="col-*-*"></div>
      <div class="col-*-*"></div>
    </div>
    <div class="row">
      <div class="col-*-*"></div>
      <div class="col-*-*"></div>
      <div class="col-*-*"></div>
    </div>

    <!-- Or let Bootstrap automatically handle the layout -->
    <div class="row">
      <div class="col"></div>
      <div class="col"></div>
      <div class="col"></div>
    </div>
    ```
    - Trong đó "`col-*-*`" : 
        - Dấu `*` thứ nhất đại diện cho responsive : các giá trị : `sm`, `md`, `lg`, `xl` 
        - Dấu `*` thứ hai đại diện cho loại chiều rộng cột ( `1 -> 12` ) .
        Tổng chiều rộng các cột phải là `12` cho mỗi dòng .
- **VD1 :** Tạo 3 cột bằng nhau :
    ```html
    <div class="row">
      <div class="col">.col</div>
      <div class="col">.col</div>
      <div class="col">.col</div>
    </div>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/D3EoVGR.png>
- **VD2 :** Tạo các cột responsive bằng nhau :
    ```html
    <div class="row">
      <div class="col-sm-3">.col-sm-3</div>
      <div class="col-sm-3">.col-sm-3</div>
      <div class="col-sm-3">.col-sm-3</div>
      <div class="col-sm-3">.col-sm-3</div>
    </div>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/fTTr59d.png>
- **VD3 :** Tạo các cột responsive không bằng nhau :
    ```html
    <div class="row">
      <div class="col-sm-4">.col-sm-4</div>
      <div class="col-sm-8">.col-sm-8</div>
    </div>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/Arwu7sl.png>

