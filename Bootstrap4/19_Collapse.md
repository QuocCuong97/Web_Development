# Collapse
## **1) Cơ bản về collapse**
- **Collapse** rất hữu ích trong việc muốn ẩn/hiện một đoạn content nào đó .
- Class "`.collapse`" chỉ ra phần tử muốn collapse . Nội dung của nó sẽ được ẩn/hiện khi người dùng click vào link hay button đã lập trình trước .
- Để ẩn/hiện nội dung collapse, thêm thuộc tính `data-toggle="collapse"` vào phần tử `<a>` hoặc phần tử `<button>` . Sau đó :
    - Thêm thuộc tính `data-target="#id"` để kết nối button với phần nội dung collapse .
    - Đối với phần tử `<a>` , sử dụng thuộc tính `href` thay cho `data-target` .
- **VD1 :** Sử dụng thẻ `<a>` :
    ```html
    <div class="container">
      <a href="#demo" class="btn btn-primary" data-toggle="collapse">Simple collapsible</a>
      <div id="demo" class="collapse">
        Lorem ipsum dolor sit amet, consectetur adipisicing elit,
        sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,
        quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
      </div>
    </div>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/BjVNXm2.png>

- **VD2 :** Sử dụng thẻ `<button>` :
    ```html
    <button data-toggle="collapse" data-target="#demo">Collapsible</button>

    <div id="demo" class="collapse">
    Lorem ipsum dolor text....
    </div>
    ```
- Mặc định , nội dung bị collapse sẽ bị ẩn ngay khi user load trang web và đợi cho user click vào button thì mới hiện ra . Để nội dung này hiển thị mặc định sau khi load trang web, thêm class "`.show`"
    ```html
    <div id="demo" class="collapse show">
    Lorem ipsum dolor text....
    </div>
    ```
## **2) Accordion**
- Sử dụng thuộc tính `data-parent` để đảm bảo rằng tất cả các phần tử collapse còn lại nằm trong một phần tử cha sẽ ẩn đi khi có 1 phần tử hiện lên .
- **VD :**
    ```html
    <div id="accordion">

      <div class="card">
        <div class="card-header">
          <a class="card-link" data-toggle="collapse" href="#collapseOne">
            Collapsible Group Item #1
          </a>
        </div>
        <div id="collapseOne" class="collapse show" data-parent="#accordion">
          <div class="card-body">
            Lorem ipsum..
          </div>
        </div>
    </div>

      <div class="card">
        <div class="card-header">
          <a class="collapsed card-link" data-toggle="collapse" href="#collapseTwo">
            Collapsible Group Item #2
          </a>
        </div>
        <div id="collapseTwo" class="collapse" data-parent="#accordion">
          <div class="card-body">
            Lorem ipsum..
          </div>
        </div>
      </div>

      <div class="card">
        <div class="card-header">
          <a class="collapsed card-link" data-toggle="collapse" href="#collapseThree">
            Collapsible Group Item #3
          </a>
        </div>
        <div id="collapseThree" class="collapse" data-parent="#accordion">
          <div class="card-body">
            Lorem ipsum..
          </div>
        </div>
      </div>

    </div>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/XlnzGDe.png>