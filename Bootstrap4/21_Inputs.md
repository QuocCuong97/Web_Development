# Inputs
## **1) Bootstrap Form Input**
- **Bootstrap4** hỗ trợ các trường input sau :
    - **input**
    - **textarea**
    - **checkbox**
    - **radio**
    - **select** 
### **1.1) Input**
- Hỗ trợ tất cả các kiểu input của **HTML5** : ***text***, ***password***, ***datetime***, ***datetime-local***, ***date***, ***month***, ***time***, ***week***, ***number***, ***email***, ***url***, ***search***, ***tel***, ***color***  .
- **VD :**
    ```html
    <div class="form-group">
      <label for="usr">Name:</label>
      <input type="text" class="form-control" id="usr">
    </div>
    <div class="form-group">
      <label for="pwd">Password:</label>
      <input type="password" class="form-control" id="pwd">
    </div>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/xyLRiTe.png>
### **1.2) Textarea**
- **VD :**
    ```html
    <div class="form-group">
      <label for="comment">Comment:</label>
      <textarea class="form-control" rows="5" id="comment"></textarea>
    </div>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/UVqYOUQ.png>
### **1.3) Checkbox**
- Sử dụng phần tử container với class "`.form-check`" để tạo 1 form checkbox . Thêm class "`.form-check-label`" để vào phần tử `<label>`, class "`.form-check-input`" vào các dòng checkbox .
- **VD :**
    ```html
    <div class="form-check">
      <label class="form-check-label">
        <input type="checkbox" class="form-check-input" value="">Option 1
      </label>
    </div>
    <div class="form-check">
      <label class="form-check-label">
        <input type="checkbox" class="form-check-input" value="">Option 2
      </label>
    </div>
    <div class="form-check">
      <label class="form-check-label">
        <input type="checkbox" class="form-check-input" value="" disabled>Option 3
      </label>
    </div>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/D4H98fL.png>
- Có thể sử dụng class "`.form-check-inline`" nếu muốn các dòng checkbox hiển thị trên cùng 1 dòng :
    ```html
    <div class="form-check-inline">
      <label class="form-check-label">
        <input type="checkbox" class="form-check-input" value="">Option 1
      </label>
    </div>
    <div class="form-check-inline">
      <label class="form-check-label">
        <input type="checkbox" class="form-check-input" value="">Option 2
      </label>
    </div>
    <div class="form-check-inline">
      <label class="form-check-label">
        <input type="checkbox" class="form-check-input" value="" disabled>Option 3
      </label>
    </div>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/wFWRM6i.png>
### **1.4) Radio Buttons**
- **VD :**
    ```html
    <div class="form-check">
      <label class="form-check-label">
        <input type="radio" class="form-check-input" name="optradio">Option 1
      </label>
    </div>
    <div class="form-check">
      <label class="form-check-label">
        <input type="radio" class="form-check-input" name="optradio">Option 2
      </label>
    </div>
    <div class="form-check disabled">
      <label class="form-check-label">
        <input type="radio" class="form-check-input" name="optradio" disabled>Option 3
      </label>
    </div>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/ySbWxPa.png>
- Sử dụng class "`.form-check-inline`" nếu muốn các dòng radio button đứng trên cùng 1 dòng :
    ```html
    <div class="form-check-inline">
      <label class="form-check-label">
        <input type="radio" class="form-check-input" name="optradio">Option 1
      </label>
    </div>
    <div class="form-check-inline">
      <label class="form-check-label">
        <input type="radio" class="form-check-input" name="optradio">Option 2
      </label>
    </div>
    <div class="form-check-inline disabled">
      <label class="form-check-label">
        <input type="radio" class="form-check-input" name="optradio" disabled>Option 3
      </label>
    </div>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/diMzYnK.png>
### **1.5) Select List**
- **VD :**
    ```html
    <div class="form-group">
      <label for="sel1">Select list (select one):</label>
      <select class="form-control" id="sel1" name="sellist1">
        <option>1</option>
        <option>2</option>
        <option>3</option>
        <option>4</option>
      </select>
      <br>
      <label for="sel2">Mutiple select list (hold shift to select more than one):</label>
      <select multiple class="form-control" id="sel2" name="sellist2">
        <option>1</option>
        <option>2</option>
        <option>3</option>
        <option>4</option>
        <option>5</option>
      </select>
    </div>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/ansAhJA.png>

### **1.6) File và Range**
- Thêm class "`.form-control-range`" vào phần tử `<input>` có `type="range"` và class "`.form-control-file`" vào phần tử `<input>` có `type="file"` :
    ```html
    <input type="range" class="form-control-range">
    <input type="file" class="form-control-file border">
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/F7hSC0k.png>
### **1.7) Kích cỡ trường input**
- Thay đổi kích cỡ trường input với các class "`.form-control-sm`" và "`.form-control-lg`"
- **VD :**
    ```html
    <input type="text" class="form-control form-control-sm">
    <input type="text" class="form-control form-control">
    <input type="text" class="form-control form-control-lg">
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/mJ1ufMz.png>
## **2) Custom Form Input**
- **Bootstrap4** cho phép cá nhân hóa cách hiển thị của các phần tử form :

    <img src=https://i.imgur.com/uqUYyNA.png>
### **2.1) Custom Checkbox**
- Để tạo 1 custom checkbox , đặt chúng trong một phần tử container như `<div>` , sử dụng class "`.custom-control` và "`.custom-checkbox`" quanh checkbox . Sau đó thêm class "`.custom-control-input` vào trường input có `type="checkbox"` .
- **VD :**
    ```html
    <form>
      <div class="custom-control custom-checkbox">
        <input type="checkbox" class="custom-control-input" id="customCheck" name="example1">
        <label class="custom-control-label" for="customCheck">Custom checkbox</label>
      </div>
    </form>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/aDeriX0.png>
### **2.2) Custom Switch**
- Để tạo một custom "toggle switch", đặt chúng trong một phần tử container như `<div>` , sử dụng class "`.custom-control` và "`.custom-switch`" quanh checkbox . Sau đó thêm class "`.custom-control-input` vào trường input có `type="checkbox"` .
- **VD :**
    ```html
    <form>
      <div class="custom-control custom-switch">
        <input type="checkbox" class="custom-control-input" id="switch1">
        <label class="custom-control-label" for="switch1">Toggle me</label>
      </div>
    </form>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/QKdzFrE.png>
### **2.3) Custom Radio buttons**
- Để tạo một custom radio button, đặt chúng trong một phần tử container như `<div>` , sử dụng class "`.custom-control` và "`.custom-radio`" quanh checkbox . Sau đó thêm class "`.custom-control-input` vào trường input có `type="radio"` .
- **VD :**
    ```html
    <form>
      <div class="custom-control custom-radio">
        <input type="radio" class="custom-control-input" id="customRadio" name="example1" value="customEx">
        <label class="custom-control-label" for="customRadio">Custom radio</label>
      </div>
    </form>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/9UCoF1S.png>
### **2.4) Custom Select Menu**
- Để tạo một custom select menu , thêm class "`.custom-select`" vào phần tử `<select>` .
    ```html
    <form>
      <select name="cars" class="custom-select">
        <option selected>Custom Select Menu</option>
        <option value="volvo">Volvo</option>
        <option value="fiat">Fiat</option>
        <option value="audi">Audi</option>
      </select>
    </form>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/R6cTUKp.png>
- Sử dụng class "`.custom-select-sm`" để tạo select menu cỡ nhỏ hơn hoặc "`.custom-select-lg`" để tạo cỡ lớn hơn .
    ```html
    <form>
      <!-- Small -->
      <select name="cars" class="custom-select-sm">
        <option selected>Small Custom Select Menu</option>
        <option value="volvo">Volvo</option>
        <option value="fiat">Fiat</option>
        <option value="audi">Audi</option>
      </select>

      <!-- Large -->
      <select name="cars" class="custom-select-lg">
        <option selected>Large Custom Select Menu</option>
        <option value="volvo">Volvo</option>
        <option value="fiat">Fiat</option>
        <option value="audi">Audi</option>
      </select>
    </form>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/xp5uHWA.png>

### **2.5) Custom Range**
- Để tạo một custom range menu , thêm class "`.custom-range`" vào trường input có `type="range"` :
- **VD :**
    ```html
    <form>
      <label for="customRange">Custom range</label>
      <input type="range" class="custom-range" id="customRange" name="points1">
    </form>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/vpOcFvu.png>

### **2.6) Custom File Upload**
- Để tạo một custom file upload, đặt chúng trong một phần tử container như `<div>` , sử dụng class "`.custom-file`" quanh trường input có `type="file"` . Sau đó thêm class "`.custom-file-input`" vào nó .
- **VD :**
    ```html
    <form>
      <div class="custom-file">
        <input type="file" class="custom-file-input" id="customFile">
        <label class="custom-file-label" for="customFile">Choose file</label>
      </div>
    </form>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/d2ptEkS.png>

### **2.7) Inline Custom Form Controls**
- Nếu muốn các custom form đứng cạnh nhau trên 1 dòng , sử dụng class "`.custom-control-inline`" cho phần tử container .
- **VD :**
    ```html
    <form>
      <div class="custom-control custom-radio custom-control-inline">
        <input type="radio" class="custom-control-input" id="customRadio" name="example" value="customEx">
        <label class="custom-control-label" for="customRadio">Custom radio 1</label>
      </div>
      <div class="custom-control custom-radio custom-control-inline">
        <input type="radio" class="custom-control-input" id="customRadio2" name="example" value="customEx">
        <label class="custom-control-label" for="customRadio2">Custom radio 2</label>
      </div>
    </form>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/Ms4CzTW.png>
## **3) Inputs Groups**
### **3.1) Input Group**
- Class "`.input-group`" là container nâng cao cho trường input bằng cách thêm icon, text hoặc button trước hoặc sau trường input .
- Class "`.input-group-prepend`" dùng để thêm các đoạn text vào trước trường input .
- Class "`.input-group-append`" dùng để thêm các đoạn text vào sau trường input .
- Class "`.input-group-text`" dùng để chứa các đoạn text này .
- **VD :**
    ```html
    <form>
      <div class="input-group mb-3">
        <div class="input-group-prepend">
          <span class="input-group-text">@</span>
        </div>
        <input type="text" class="form-control" placeholder="Username">
      </div>

      <div class="input-group mb-3">
        <input type="text" class="form-control" placeholder="Your Email">
        <div class="input-group-append">
          <span class="input-group-text">@example.com</span>
        </div>
      </div>
    </form>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/XIUAVKA.png>
### **3.2) Kích cỡ Input Group**
- Sử dụng class "`.input-group-sm`" cho input group cỡ nhỏ và "`.input-group-lg`" cho input group cỡ lớn .
- **VD :**
    ```html
    <form>
      <div class="input-group mb-3 input-group-sm">
        <div class="input-group-prepend">
          <span class="input-group-text">Small</span>
        </div>
        <input type="text" class="form-control">
      </div>
    </form>
    <form>
      <div class="input-group mb-3">
        <div class="input-group-prepend">
          <span class="input-group-text">Default</span>
        </div>
        <input type="text" class="form-control">
      </div>
    </form>
    <form>
      <div class="input-group mb-3 input-group-lg">
        <div class="input-group-prepend">
          <span class="input-group-text">Large</span>
        </div>
        <input type="text" class="form-control">
      </div>
    </form>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/HbjkPVR.png>
### **3.3) Multiple Inputs and Helpers**
- **VD :**
    ```html
    <!-- Multiple inputs -->
    <form>
      <div class="input-group mb-3">
        <div class="input-group-prepend">
          <span class="input-group-text">Person</span>
        </div>
        <input type="text" class="form-control" placeholder="First Name">
        <input type="text" class="form-control" placeholder="Last Name">
      </div>
    </form>

    <!-- Multiple addons / help text -->
    <form>
      <div class="input-group mb-3">
        <div class="input-group-prepend">
          <span class="input-group-text">One</span>
          <span class="input-group-text">Two</span>
          <span class="input-group-text">Three</span>
        </div>
        <input type="text" class="form-control">
      </div>
    </form>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/99vzjhh.png>
### **3.4) Input Group với Checkbox và Radio**
- **VD :**
    ```html
    <div class="input-group mb-3">
      <div class="input-group-prepend">
        <div class="input-group-text">
        <input type="checkbox">
        </div>
      </div>
      <input type="text" class="form-control" placeholder="Some text">
    </div>

    <div class="input-group mb-3">
      <div class="input-group-prepend">
        <div class="input-group-text">
          <input type="radio">
        </div>
      </div>
      <input type="text" class="form-control" placeholder="Some text">
    </div>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/7KQWrr0.png>
### **3.5) Input Group Buttons**
- **VD :**
    ```html
    <div class="input-group mb-3">
      <div class="input-group-prepend">
        <button class="btn btn-outline-primary" type="button">Basic Button</button>
      </div>
      <input type="text" class="form-control" placeholder="Some text">
    </div>

    <div class="input-group mb-3">
      <input type="text" class="form-control" placeholder="Search">
      <div class="input-group-append">
        <button class="btn btn-success" type="submit">Go</button>
      </div>
    </div>

    <div class="input-group mb-3">
      <input type="text" class="form-control" placeholder="Something clever..">
      <div class="input-group-append">
        <button class="btn btn-primary" type="button">OK</button>
        <button class="btn btn-danger" type="button">Cancel</button>
      </div>
    </div>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/coFpEV1.png>
### **3.6) Input Group với Dropdown Button**
- **VD :**
    ```html
    <div class="input-group mt-3 mb-3">
      <div class="input-group-prepend">
        <button type="button" class="btn btn-outline-secondary dropdown-toggle" data-toggle="dropdown">
        Dropdown button
        </button>
        <div class="dropdown-menu">
          <a class="dropdown-item" href="#">Link 1</a>
          <a class="dropdown-item" href="#">Link 2</a>
          <a class="dropdown-item" href="#">Link 3</a>
        </div>
      </div>
      <input type="text" class="form-control" placeholder="Username">
    </div>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/O0E6UdY.png>
### **3.7) Input Group Labels**
- **VD :**
    ```html
    <label for="demo">Write your email here:</label>
    <div class="input-group mb-3">
      <input type="text" class="form-control" placeholder="Email" id="demo" name="email">
      <div class="input-group-append">
        <span class="input-group-text">@example.com</span>
      </div>
    </div>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/dS8gYQU.png>