# Media Object
## **1) Cơ bản về Media Object**
- **Bootstrap** cung cấp một cách dễ dàng để căn chỉnh các **media object** ( như images và video ) cùng với nội dung . 
- **Media object** thường được sử dụng phổ biến để hiển thị các comment :
    
    <img src=https://i.imgur.com/dmlFCu5.png>

- Để tạo một **media object**, thêm class "`.media`" vào phần tử container , đặt các **media content** bên trong các phần tử child với class "`.media-body`" . Thêm padding và margin nếu cần - sử dụng tiện ích `spacing` :
    ```html
    <div class="container mt-3">
      <div class="media border p-3">
        <img src="img_avatar3.png" alt="John Doe" class="mr-3 mt-3 rounded-circle" style="width:60px;">
        <div class="media-body">
          <h4>John Doe <small><i>Posted on February 19, 2016</i></small></h4>
          <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</p>      
        </div>
      </div>
    </div>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/WJA6r6c.png>

## **2) Lồng các Media Object**
- **Media Object** có thể lồng lẫn vào nhau ( **media object** trong **media object** )
- Để lồng thêm **media object** , đặt container "`.media`" mới bên trong container "`.media container`"
- **VD :**
    ```html
    <div class="media border p-3">
      <img src="img_avatar3.png" alt="John Doe" class="mr-3 mt-3 rounded-circle" style="width:60px;">
      <div class="media-body">
        <h4>John Doe <small><i>Posted on February 19, 2016</i></small></h4>
        <p>Lorem ipsum...</p>
        <div class="media p-3">
          <img src="img_avatar2.png" alt="Jane Doe" class="mr-3 mt-3 rounded-circle" style="width:45px;">
          <div class="media-body">
            <h4>Jane Doe <small><i>Posted on February 20 2016</i></small></h4>
            <p>Lorem ipsum...</p>
          </div>
        </div> 
      </div>
    </div>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/ZqecJ7V.png>

## **3) Right-Aligned Media Image**
- Để căn chỉnh sang phải cho **media image**, xếp **image** sau phần tử "`.media-body`"
    ```html
    <div class="media border p-3">
      <div class="media-body">
        <h4>John Doe <small><i>Posted on February 19, 2016</i></small></h4>
        <p>Lorem ipsum...</p>
      </div>
      <img src="img_avatar3.png" alt="John Doe" class="ml-3 mt-3 rounded-circle" style="width:60px;">
    </div>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/YNlb21a.png>

## **4) Top, Middle or Bottom Alignment**
- Sử dụng các thuộc tính flex , class "`.align-self-*`" để đặt **media object** ở trên , dưới hoặc giữa :
- **VD :**
    ```html
    <!-- Media top -->
    <div class="media">
      <img src="img_avatar1.png" class="align-self-start mr-3" style="width:60px">
      <div class="media-body">
        <h4>Media Top</h4>
        <p>Lorem ipsum...</p>
      </div>
    </div>

    <!-- Media middle -->
    <div class="media">
      <img src="img_avatar1.png" class="align-self-center mr-3" style="width:60px">
      <div class="media-body">
        <h4>Media Middle</h4>
        <p>Lorem ipsum...</p>
      </div>
    </div>

    <!-- Media bottom -->
    <div class="media">
      <img src="img_avatar1.png" class="align-self-end mr-3" style="width:60px">
      <div class="media-body">
        <h4>Media Bottom</h4>
        <p>Lorem ipsum...</p>
      </div>
    </div>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/McSf3wc.png>

