# Button
## **1) Button Styles**
- **Bootstrap4** cung cấp các kiểu button sau, ý nghĩa màu sắc cũng giống với alert :
    ```html
    <button type="button" class="btn">Basic</button>
    <button type="button" class="btn btn-primary">Primary</button>
    <button type="button" class="btn btn-secondary">Secondary</button>
    <button type="button" class="btn btn-success">Success</button>
    <button type="button" class="btn btn-info">Info</button>
    <button type="button" class="btn btn-warning">Warning</button>
    <button type="button" class="btn btn-danger">Danger</button>
    <button type="button" class="btn btn-dark">Dark</button>
    <button type="button" class="btn btn-light">Light</button>
    <button type="button" class="btn btn-link">Link</button>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/e0jSftr.png>

- Các class button có thể được sử dụng trong phần tử `<a>`, `<button>`, hoặc `<input>` :
    ```html
    <a href="#" class="btn btn-info" role="button">Link Button</a>
    <button type="button" class="btn btn-info">Button</button>
    <input type="button" class="btn btn-info" value="Input Button">
    <input type="submit" class="btn btn-info" value="Submit Button">
    ```
    - Hiển thi trên trình duyệt :

        <img src=https://i.imgur.com/fBBSPHe.png>

## **2) Button Outline**
- **Bootstrap4** cung cấp 8 màu outline cho 1 button :
    ```html
    <button type="button" class="btn btn-outline-primary">Primary</button>
    <button type="button" class="btn btn-outline-secondary">Secondary</button>
    <button type="button" class="btn btn-outline-success">Success</button>
    <button type="button" class="btn btn-outline-info">Info</button>
    <button type="button" class="btn btn-outline-warning">Warning</button>
    <button type="button" class="btn btn-outline-danger">Danger</button>
    <button type="button" class="btn btn-outline-dark">Dark</button>
    <button type="button" class="btn btn-outline-light text-dark">Light</button>
    ```
    - Hiển thị trên trình duyệt :
        
        <img src=https://i.imgur.com/3511iwQ.png>

## **3) Button Sizes**
- **Bootstrap4** cho phép thay đổi kích cỡ button bằng cách sử dụng class :
    - `.btn-lg` : button to
    - `.btn-sm` : button nhỏ
    - Nếu không được khai báo, kích cỡ của button sẽ là mặc định .
- **VD :**
    ```html
    <button type="button" class="btn btn-primary btn-lg">Large</button>
    <button type="button" class="btn btn-primary">Default</button>
    <button type="button" class="btn btn-primary btn-sm">Small</button>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/4b8J6os.png>

## **4) Block Level Button**
- Thêm class "`.btn-block`" để tạo block button với chiều rộng trải dài bằng phần tử chứa nó .
- **VD :**
    ```html
    <button type="button" class="btn btn-primary btn-block">Full-Width Button</button>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/aoyBH4r.png>

## **5) Active/Disabled Buttons**
- Một button có thể được đặt là ***active*** ( có thể click được ) hoặc ở trạng thái ***disabled*** ( không thể click được ) .
- Sử dụng class "`.active`" để cho button có thể click được ( trạng thái ***active*** ) .
- Sử dụng thuộc tính `disabled` để button không thể click được ( trạng thái ***disabled*** )
> Thẻ `<a>` không hỗ trợ thuộc tính `disabled` vì vậy cần phải sử dụng class "`.disabled`"
- **VD :**
    ```html
    <button type="button" class="btn btn-primary">Primary Button</button>
    <button type="button" class="btn btn-primary active">Active Primary</button>
    <button type="button" class="btn btn-primary" disabled>Disabled Primary</button>
    <a href="#" class="btn btn-primary disabled">Disabled Link</a>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/oaTdMVF.png>

## **6) Button Groups**



