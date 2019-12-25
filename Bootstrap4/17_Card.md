# Card
## **1) Cơ bản về Card**
- **Card** trong **Bootstrap4** là thẻ có viền bao quanh với padding bao quanh nội dung của nó . **Card** bao gồm **headers**, **footers**, **content**, **colors**, ....
- Tạo một **card** cơ bản bằng class "`.card`" , đặt phần content bên trong class "`.card-body`"
    ```html
    <div class="card">
      <div class="card-body">Basic card</div>
    </div>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/33WCsvz.png>

- Class "`.card-header` thêm heading vào thẻ vào **card** và class "`.card-footer`" thêm footer vào **card**
    ```html
    <div class="card">
      <div class="card-header">Header</div>
      <div class="card-body">Content</div>
      <div class="card-footer">Footer</div>
    </div>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/EO0AMWq.png>

## **2) Sử dụng các class biểu thị màu sắc**
- Để thêm màu nền cho **card** , sử dụng các class biểu thị màu sắc ( "`.bg-primary`", "`.bg-success`", "`.bg-info`", "`.bg-warning`", "`.bg-danger`", "`.bg-secondary`", "`.bg-dark`", "`.bg-light`" )
- **VD :**
    ```html
    <div class="card">
      <div class="card-body">Basic card</div>
    </div>
    <br>
    <div class="card bg-primary text-white">
      <div class="card-body">Primary card</div>
    </div>
    <br>
    <div class="card bg-success text-white">
      <div class="card-body">Success card</div>
    </div>
    <br>
    <div class="card bg-info text-white">
      <div class="card-body">Info card</div>
    </div>
    <br>
    <div class="card bg-warning text-white">
      <div class="card-body">Warning card</div>
    </div>
    <br>
    <div class="card bg-danger text-white">
      <div class="card-body">Danger card</div>
    </div>
    <br>
    <div class="card bg-secondary text-white">
      <div class="card-body">Secondary card</div>
    </div>
    <br>
    <div class="card bg-dark text-white">
      <div class="card-body">Dark card</div>
    </div>
    <br>
    <div class="card bg-light text-dark">
      <div class="card-body">Light card</div>
    </div>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/NDZakRP.png>

## **3) Title , text và link**
- Class "`.card-title`" để thêm thêm **title** cho **card** vào bất cứ phần tử heading nào .
- Class "`.card-text` sử dụng để xóa bỏ margin-bottom cho phần tử `<p>` khi nó là phần tử cuối cùng (hoặc duy nhất) bên trong "`.card-body`" .
- Class "`.card-link`" thêm nền màu chữ xanh vào bất cứ link nào, đồng thời với hiệu ứng di chuột ( hover )
- **VD :**
    ```html
    <div class="card">
      <div class="card-body">
        <h4 class="card-title">Card title</h4>
        <p class="card-text">Some example text. Some example text.</p>
        <a href="#" class="card-link">Card link</a>
        <a href="#" class="card-link">Another link</a>
      </div>
    </div>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/NZgF4wN.png>

## **4) Card Image**
- Thêm class "`.card-img-top`" hoặc "`.card-img-bottom`" vào phần tử `<img>` để đặt hình ảnh phía trên hoặc dưới bên trong **card** .
    > Phải thêm hình ảnh bên ngoài "`.card-body`" để có thể trải dài hết chiều rộng .
- **VD :**
    ```html
    <div class="card" style="width:200px">
      <img class="card-img-top" src="https://i.imgur.com/ZuSsjIT.jpg" alt="Card image">
      <div class="card-body">
        <h4 class="card-title">Ngo Quoc Cuong</h4>
        <p class="card-text">Some example text.</p>
        <a href="#" class="btn btn-primary">See Profile</a>
      </div>
    </div>
    ```
    - Hiển thị trên trình duyệt :
        
        <img src=https://i.imgur.com/ztOEBY5.png>

## **5) Stretched Link**
- Thêm class "`.stretched-link`" vào **link** bên trong **card** , nó sẽ khiến toàn bộ **card** có thể click được và có hiệu ứng di chuột => Click vào **card** chính là click vào **link** 
- **VD :**
    ```html
    <a href="#" class="btn btn-primary stretched-link">See Profile</a>
    ```
## **6) Card Image Overlays**
- Biến một hình ảnh thành hình nền cho **card** bằng cách sử dụng class "`.card-img-overlay`" để đặt text lên đầu của ảnh .
- **VD :**
    ```html
    <div class="card" style="width:300px">
      <img class="card-img-top" src="img_avatar1.png" alt="Card image">
      <div class="card-img-overlay">
        <h4 class="card-title">John Doe</h4>
        <p class="card-text">Some example text.</p>
        <a href="#" class="btn btn-primary">See Profile</a>
      </div>
    </div>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/0fcjfhr.png>

## **7) Card Column**
- Class "`.card-columns`" tạo ra một khung lưới đan xen các **card** với nhau .
- Bố cục sẽ được tự động được căn chỉnh mỗi khi chèn thêm **card** mới .
> Các card sẽ hiển thị theo chiều dọc đối với các màn hình nhỏ ( `width < 576px` )
- **VD :**
    ```html
    <div class="card-columns">
      <div class="card bg-primary">
        <div class="card-body text-center">
          <p class="card-text">Some text inside the first card</p>
        </div>
      </div>
      <div class="card bg-warning">
        <div class="card-body text-center">
        <p class="card-text">Some text inside the second card</p>
        </div>
      </div>
      <div class="card bg-success">
        <div class="card-body text-center">
          <p class="card-text">Some text inside the third card</p>
        </div>
      </div>
      <div class="card bg-danger">
        <div class="card-body text-center">
          <p class="card-text">Some text inside the fourth card</p>
        </div>
      </div>
      <div class="card bg-light">
        <div class="card-body text-center">
        <p class="card-text">Some text inside the fifth card</p>
        </div>
      </div>
      <div class="card bg-info">
        <div class="card-body text-center">
          <p class="card-text">Some text inside the sixth card</p>
        </div>
      </div>
    </div>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/Akd090f.png>

## **8) Card Deck**
- Class "`.card-deck`" tạo ra một khung lưới các card nối tiếp nhau , có cùng chiều cao và chiều rộng . 
- Bố cục sẽ được tự động được căn chỉnh mỗi khi chèn thêm **card** mới .
> Các card sẽ hiển thị theo chiều dọc đối với các màn hình nhỏ ( `width < 576px` )
- **VD :**
    ```html
    <div class="card-deck">
      <div class="card bg-primary">
        <div class="card-body text-center">
          <p class="card-text">Some text inside the first card</p>
        </div>
      </div>
      <div class="card bg-warning">
        <div class="card-body text-center">
          <p class="card-text">Some text inside the second card</p>
        </div>
      </div>
      <div class="card bg-success">
        <div class="card-body text-center">
          <p class="card-text">Some text inside the third card</p>
        </div>
      </div>
      <div class="card bg-danger">
        <div class="card-body text-center">
          <p class="card-text">Some text inside the fourth card</p>
        </div>
      </div>
    </div>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/KpgQQEC.png>

## 9) Card Group**
- Class "`.card-group`" tương tự như "`.card-deck`" . Khác biệt duy nhất là class "`.card-group` sẽ bỏ hết margin-left và margin-right giữa các card .
> Các card sẽ hiển thị theo chiều dọc đối với các màn hình nhỏ ( `width < 576px` ) - ***kèm theo margin-top và margin-bottom*** 
- **VD :**
    ```html
    <div class="card-group">
      <div class="card bg-primary">
        <div class="card-body text-center">
          <p class="card-text">Some text inside the first card</p>
        </div>
      </div>
      <div class="card bg-warning">
        <div class="card-body text-center">
          <p class="card-text">Some text inside the second card</p>
        </div>
      </div>
      <div class="card bg-success">
        <div class="card-body text-center">
          <p class="card-text">Some text inside the third card</p>
        </div>
      </div>
      <div class="card bg-danger">
        <div class="card-body text-center">
          <p class="card-text">Some text inside the fourth card</p>
        </div>
      </div>
    </div>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/sa06Kty.png>

        