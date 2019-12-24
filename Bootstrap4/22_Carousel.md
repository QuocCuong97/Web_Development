# Carousel
## **1) Cơ bản về carousel**
- **Carousel** là một slideshow trình chiếu vòng tròn các phần tử :
- Các class sử dụng để tạo 1 **carousel** :
    - "`.carousel`"  : tạo ra 1 **carousel**
    - "`.carousel-indicators`" : thêm indicator cho **carousel** . Chúng là những thanh nhỏ ở phía dưới mỗi slide ( chỉ ra có bao nhiêu slide trong **carousel** , đồng thời chỉ ra user đang xem slide nào )
    - "`.carousel-inner`" : thêm slide vào **carousel**
    - "`.carousel-item`" : thêm nội dung cho slide
    - "`.carousel-control-prev`" : thêm button "previous" vào bên trái **carousel** , cho phép user quay lại slide trước
    - "`.carousel-control-next`" : thêm button "next" vào bên phải **carousel** , cho phép user qua slide tiếp theo
    - "`.carousel-control-prev-icon`" : sử dụng cùng với "`.carousel-control-prev`" để tạo button "previous"
    - "`.carousel-control-next-icon`" : sử dụng cùng với "`.carousel-control-next`" để tạo button "next"
    - "`.slide`" : thêm hiệu ứng di chuyển **CSS** khi di chuyển giữa các slide . Nếu không cần có thể bỏ qua .
- **VD :**
    ```html
    <div id="demo" class="carousel slide" data-ride="carousel">

    <!-- Indicators -->
      <ul class="carousel-indicators">
        <li data-target="#demo" data-slide-to="0" class="active"></li>
        <li data-target="#demo" data-slide-to="1"></li>
        <li data-target="#demo" data-slide-to="2"></li>
      </ul>

    <!-- The slideshow -->
      <div class="carousel-inner">
        <div class="carousel-item active">
          <img src="la.jpg" alt="Los Angeles">
        </div>
        <div class="carousel-item">
          <img src="chicago.jpg" alt="Chicago">
        </div>
        <div class="carousel-item">
          <img src="ny.jpg" alt="New York">
        </div>
      </div>

    <!-- Left and right controls -->
      <a class="carousel-control-prev" href="#demo" data-slide="prev">
        <span class="carousel-control-prev-icon"></span>
      </a>
      <a class="carousel-control-next" href="#demo" data-slide="next">
        <span class="carousel-control-next-icon"></span>
      </a>
    </div>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/kqlh3LB.png>

## **2) Thêm caption cho slide**
- Thêm phần tử trong `<div class="carousel-caption">` bên trong mỗi `<div class="carousel-item">` để tạo caption cho mỗi slide :
    ```html
    <div class="carousel-item">
      <img src="la.jpg" alt="Los Angeles">
      <div class="carousel-caption">
        <h3>Los Angeles</h3>
        <p>We had such a great time in LA!</p>
      </div>
    </div>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/fL5THiO.png>

