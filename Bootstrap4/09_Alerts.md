# Alerts
## **1) Các kiểu hộp thoại alert**
- Các nội dung thông báo được tạo bởi class "`.alert`" , theo đó là các màu sắc đặc trưng cho các kiểu thông báo khác nhau :
    - "`.alert-success`" : class này thông báo một hành động thành công :
        ```html
        <div class="alert alert-success">
          <strong>Success!</strong> This alert box could indicate a successful or positive action.
        </div>
        ```
        - Hiển thị trên trình duyệt :

            <img src=https://i.imgur.com/2m6wOhM.png>
    - "`.alert-info`" : class này thông báo một sự thay đổi nội dung :
        ```html
        <div class="alert alert-info">
          <strong>Info!</strong> This alert box could indicate a neutral informative change or action.
        </div>
        ```
        - Hiển thị trên trình duyệt :

            <img src=https://i.imgur.com/7262WxJ.png>
    - "`.alert-warning`" : class này đưa ra một cảnh báo cần chú ý :
        ```html
        <div class="alert alert-warning">
          <strong>Warning!</strong> This alert box could indicate a warning that might need attention.
        </div>
        ```
        - Hiển thị trên trình duyệt :   

            <img src=https://i.imgur.com/5pBKLcr.png>
    - "`.alert-danger`" : class này thông báo một hành động nguy hiểm hoặc có tính tiêu cực :
        ```html
        <div class="alert alert-danger">
          <strong>Danger!</strong> This alert box could indicate a dangerous or potentially negative action.
        </div>
        ```
        - Hiển thị trên trình duyệt :

            <img src=https://i.imgur.com/yKq0N4C.png>
    - "`.alert-primary`" : class này thông báo một hành động quan trọng :
        ```html
        <div class="alert alert-primary">
          <strong>Primary!</strong> Indicates an important action.
        </div>
        ```
        - Hiển thị trên trình duyệt :

            <img src=https://i.imgur.com/cC7FBki.png>
    - "`.alert-secondary`" : class này thông báo một hành động kém quan trọng hơn : 
        ```html
        <div class="alert alert-secondary">
          <strong>Secondary!</strong> Indicates a slightly less important action.
        </div>
        ```
        - Hiển thị trên trình duyệt :

            <img src=https://i.imgur.com/cIxJMh3.png>
    - "`.alert-dark`" : class này đưa ra 1 thông báo với nền xám đen :
        ```html
        <div class="alert alert-dark">
          <strong>Dark!</strong> Dark grey alert.
        </div>
        ```
        - Hiển thị trên trình duyệt :

            <img src=https://i.imgur.com/AKvQF8D.png>
    - "`.alert-light`" class này đưa ra một thông báo với nền sáng :
        ```html
        <div class="alert alert-light">
          <strong>Light!</strong> Light grey alert.
        </div>
        ```
        - Hiển thị trên trình duyệt :

            <img src=https://i.imgur.com/jjBwsDh.png>

## **2) Alert Link**
- Thêm class "`alert-link`" vào bất cứ link nào trong hộp thoại alert để tạo link cho user có thể click vào .
- **VD :**
    ```html
    <div class="alert alert-warning">
      <strong>Warning!</strong> You should <a href="https://stackoverflow.com/" class="alert-link">read this message</a>.
    </div>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/pjotMRa.png>

## **3) Đóng hộp thoại alert**
- Để đóng hộp thoại alert , thêm class "`.alert-dismissible`" vào trong container chứa class "`.alert`" . Sau đó thêm `class="close"` và `data-dimiss="alert"` vào link hoặc button sử dụng để user click khi muốn đóng hộp thoại .
- Sử dụng thực thể **HTML** `&times;` ( <code>&times;</code> ) được khuyến nghị sử dụng để đóng thông báo thay cho ký tự ( `x` ) .
- **VD :**
    ```html
    <div class="alert alert-success alert-dismissible">
      <button type="button" class="close" data-dismiss="alert">&times;</button>
      <strong>Success!</strong> This alert box could indicate a successful or positive action.
    </div>
    <div class="alert alert-info alert-dismissible">
      <button type="button" class="close" data-dismiss="alert">&rarr;</button>
      <strong>Info!</strong> This alert box could indicate a neutral informative change or action.
    </div>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/5wy4hGD.png>
## **4) Animated Alert**
- Class `.fade` và `.show` thêm hiệu ứng ẩn/hiện khi đóng hộp thoại alert .
- **VD :**
    ```html
    <div class="alert alert-danger alert-dismissible fade show">
    ```
