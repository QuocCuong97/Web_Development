# Dropdowns
## **1) Cơ bản về dropdown**
- Một **dropdown** menu là một menu có thể mở rộng cho phép user chọn 1 giá trị từ list cho trước :
- Sử dụng class "`.dropdown`" để định nghĩa 1 menu dropdown .
- Để mở menu dropdown ,  sử dụng một button hoặc một link với class "`.dropdown-toggle`" và thuộc tính `data-toggle="dropdown"`
- Thêm class "`.dropdown-menu`" vào phần tử `<div>` để thực sự tạo 1 dropdown menu . Sau đó thêm các class "`.dropdown-item`" vào mỗi phần tử bên trong menu dropdown
    ```html
    <div class="dropdown">
      <button type="button" class="btn btn-primary dropdown-toggle" data-toggle="dropdown">Dropdown button</button>
      <div class="dropdown-menu">
        <a class="dropdown-item" href="#">Link 1</a>
        <a class="dropdown-item" href="#">Link 2</a>
        <a class="dropdown-item" href="#">Link 3</a>
      </div>
    </div>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/RZNQ0U7.png>
## **2) Dropdown Divider**
- Class "`.dropdown-divider`" được sử dụng để ngăn cách giữa các link bên trong menu dropdown với một đường border nét mảnh :
    ```html
    <div class="dropdown">
      <button type="button" class="btn btn-primary dropdown-toggle" data-toggle="dropdown">Dropdown button</button>
      <div class="dropdown-menu">
        <a class="dropdown-item" href="#">Link 1</a>
        <div class="dropdown-divider"></div>
        <a class="dropdown-item" href="#">Link 2</a>
        <div class="dropdown-divider"></div>
        <a class="dropdown-item" href="#">Link 3</a>
      </div>
    </div>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/OVRt8kR.png>
## **3) Dropdown Header**
- Sử dụng class "`.dropdown-header`" để thêm header vào bên trong dropdown menu :
    ```html
    <div class="dropdown">
      <button type="button" class="btn btn-primary dropdown-toggle" data-toggle="dropdown">Dropdown button</button>
      <div class="dropdown-menu">
        <h5 class="dropdown-header">Dropdown header</h5>
        <a class="dropdown-item" href="#">Link 1</a>
        <a class="dropdown-item" href="#">Link 2</a>
        <a class="dropdown-item" href="#">Link 3</a>
        <h5 class="dropdown-header">Dropdown header</h5>
        <a class="dropdown-item" href="#">Another link</a>
      </div>
    </div>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/KWBtxsu.png>

## **4) Disable and Active items**
- Có thể highlight những item đặc biệt với class "`.active`" ( item được highlight sẽ có nền màu xanh )
- Để disable một item trong dropdown menu, sử dụng class "`.disabled`" ( item bị disabled sẽ có chữ màu xám trắng và không thể click )
- **VD :**
    ```html
    <div class="dropdown">
      <button type="button" class="btn btn-primary dropdown-toggle" data-toggle="dropdown">Dropdown button</button>
      <div class="dropdown-menu">
        <a class="dropdown-item" href="#">Normal</a>
        <a class="dropdown-item active" href="#">Active</a>
        <a class="dropdown-item disabled" href="#">Disabled</a>
      </div>
    </div>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/gkPFSeB.png>
## **5) Dropdown Position**
- Có thể tạo ra menu "dropright" hoặc "dropleft", bằng cách thêm class "`.dropright`" hoặc "`.dropleft`" vào phần tử dropdown :
- **VD1 :** Dropright :
    ```html
    <div class="dropdown dropright">
      <button type="button" class="btn btn-primary dropdown-toggle" data-toggle="dropdown">Dropright button</button>
      <div class="dropdown-menu">
        <a class="dropdown-item" href="#">Link 1</a>
        <a class="dropdown-item" href="#">Link 2</a>
        <a class="dropdown-item" href="#">Link 3</a>
      </div>
    </div>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/nOyx5TX.png>
- **VD2 :** Dropleft :
    ```html
    <div class="dropdown dropleft">
      <button type="button" class="btn btn-primary dropdown-toggle" data-toggle="dropdown">Dropright button</button>
      <div class="dropdown-menu">
        <a class="dropdown-item" href="#">Link 1</a>
        <a class="dropdown-item" href="#">Link 2</a>
        <a class="dropdown-item" href="#">Link 3</a>
      </div>
    </div>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/tqNK1AR.png>

## **6) Dropdown Menu Right**
- Để căn chỉnh sang phải cho dropdown menu, thêm class "`.dropdown-menu-right`" vào phần tử có class "`.dropdown-menu`"
- **VD :**
    ```html
    <div class="dropdown">
      <button type="button" class="btn btn-primary dropdown-toggle" data-toggle="dropdown">Wide dropdown button to demonstrate this example</button>
      <div class="dropdown-menu dropdown-menu-right">
        <a class="dropdown-item" href="#">Link 1</a>
        <a class="dropdown-item" href="#">Link 2</a>
        <a class="dropdown-item" href="#">Link 3</a>
      </div> 
    </div>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/WbH479n.png>

## **7) Dropup**
- Nếu muốn dropdown menu mở rộng theo hướng lên trên thay vì xuống dưới , thay phần tử `<div>` với class "`.dropdown`" thành phần tử `<div>` với class là "`.dropup`" 
- **VD :**
    ```html
    <div class="dropup">
      <button type="button" class="btn btn-primary dropdown-toggle" data-toggle="dropdown">Dropup button<button>
      <div class="dropdown-menu">
        <a class="dropdown-item" href="#">Link 1</a>
        <a class="dropdown-item" href="#">Link 2</a>
      </div>
    </div>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/R8h0b3q.png>

## **8) Dropdown Text**
- Class "`.dropdown-item-text`" được sử dụng để thêm đoạn text vào dropdown item ( không click được - không phải link ).
- **VD :**
    ```html
    <div class="dropdown-menu">
      <a class="dropdown-item" href="#">Link 1</a>
      <a class="dropdown-item" href="#">Link 2</a>
      <a class="dropdown-item-text" href="#">Text Link</a>
      <span class="dropdown-item-text">Just Text</span>
    </div>
    ```
    - Hiển thị trên trình duyệt

        <img src=https://i.imgur.com/GdgP5YU.png>
## **9) Grouped Buttons with a Dropdown**
- **VD :**
    ```html
    <div class="btn-group">
      <button type="button" class="btn btn-primary">Apple</button>
      <button type="button" class="btn btn-primary">Samsung</button>
      <div class="btn-group">
        <button type="button" class="btn btn-primary dropdown-toggle" data-toggle="dropdown">
        Sony
        </button>
        <div class="dropdown-menu">
          <a class="dropdown-item" href="#">Tablet</a>
          <a class="dropdown-item" href="#">Smartphone</a>
        </div>
      </div>
    </div>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/eWmXxo4.png>
## **10) Split Button Dropdowns**
- **VD :**
    ```html
    <div class="btn-group">
      <button type="button" class="btn btn-primary">Primary</button>
      <button type="button" class="btn btn-primary dropdown-toggle dropdown-toggle-split" data-toggle="dropdown">
      </button>
      <div class="dropdown-menu">
        <a class="dropdown-item" href="#">Link 1</a>
        <a class="dropdown-item" href="#">Link 2</a>
      </div>
    </div>
    ```
## **11) Vertical Button Group Dropdown**
- **VD :**
    ```html
    <div class="btn-group-vertical">
      <button type="button" class="btn btn-primary">Apple</button>
      <button type="button" class="btn btn-primary">Samsung</button>
      <div class="btn-group">
        <button type="button" class="btn btn-primary dropdown-toggle" data-toggle="dropdown">
        Sony
        </button>
        <div class="dropdown-menu">
          <a class="dropdown-item" href="#">Tablet</a>
          <a class="dropdown-item" href="#">Smartphone</a>
        </div>
      </div>
    </div>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/sF1Y7Ai.png>