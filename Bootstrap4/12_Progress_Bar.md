# Progress Bar
## **1) Cơ bản về progress bar ( thanh tiến trình )**
- Một **progress bar** có thể được sử dụng để cho user thấy họ đang ở đoạn nào của một tiến trình .
- Để tạo ra một **progress bar** mặc định , thêm class "`.progress`" và phần tử container và thêm class "`.progress-bar`" vào các phần tử con của nó ( chính là các dòng tiến trình riêng biệt ) .
- Có thể sử dụng thuộc tính `width` để set chiều rộng đoạn tiến trình đã hoàn thành cho **progress bar** .
    ```html
    <div class="progress">
      <div class="progress-bar" style="width:70%"></div>
    </div>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/b6AYmjK.png>

- Chiều cao của **progress bar** mặc định là `16px` . Sử dụng thuộc tính `height` để thay đổi . 
    >Chiều cao của phần tử container và **progress bar** phải giống nhau .

    ```html
    <div class="progress" style="height:20px">
      <div class="progress-bar" style="width:40%;height:20px"></div>
    </div>
    ```
    - Hiển thị trên trình duyệt :   

        <img src=https://i.imgur.com/6R1jknG.png>
- Có thể thêm text ( hay còn được gọi là **label** - nhãn ) của **progress bar** để mô tả phần trăm của tiến trình :
    ```html
    <div class="progress">
      <div class="progress-bar" style="width:70%">70%</div>
    </div>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/fxS2dXc.png>

## **2) Màu progress bar**
- Mặc định, **progress bar** có màu xanh ( **primary** ) .
- Sử dụng các class nền màu của **Bootstrap4** để thay đổi màu của nó .
    ```html
    <!-- Blue -->
    <div class="progress">
      <div class="progress-bar" style="width:10%"></div>
    </div>

    <!-- Green -->
    <div class="progress">
      <div class="progress-bar bg-success" style="width:20%"></div>
    </div>

    <!-- Turquoise -->
    <div class="progress">
      <div class="progress-bar bg-info" style="width:30%"></div>
    </div>

    <!-- Orange -->
    <div class="progress">
      <div class="progress-bar bg-warning" style="width:40%"></div>
    </div>

    <!-- Red -->
    <div class="progress">
      <div class="progress-bar bg-danger" style="width:50%"></div>
    </div>

    <!-- White -->
    <div class="progress border">
      <div class="progress-bar bg-white" style="width:60%"></div>
    </div>

    <!-- Grey -->
    <div class="progress">
      <div class="progress-bar bg-secondary" style="width:70%"></div>
    </div>

    <!-- Light Grey -->
    <div class="progress border">
      <div class="progress-bar bg-light" style="width:80%"></div>
    </div>

    <!-- Dark Grey -->
    <div class="progress">
      <div class="progress-bar bg-dark" style="width:90%"></div>
    </div>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/rDEgpIa.png>

## **3) Striped Progress Bars**
- Sử dụng class "`.progress-bar-stripped`" để thêm các đường sọc chéo ( stripped ) vào **progress bar** :
    ```html
    <div class="progress">
      <div class="progress-bar progress-bar-striped" style="width:40%"></div>
    </div>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/HNzzHfR.png>
- Thêm class "`.progress-bar-animated`" để khiến **progress bar** sinh động hơn, giống như đang "chạy"
    ```html
    <div class="progress-bar progress-bar-striped progress-bar-animated" style="width:40%"></div>
    ```
## **4) Multiple Progress Bars**
- Các **progress bar** cũng có thể được xếp chồng lên nhau trên cùng 1 dòng .
- **VD :**
    ```html
    <div class="progress">
      <div class="progress-bar bg-success" style="width:40%">Free Space</div>
      <div class="progress-bar bg-warning" style="width:10%">Warning</div>
      <div class="progress-bar bg-danger" style="width:20%">Danger</div>
    </div>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/8wUDIqc.png>