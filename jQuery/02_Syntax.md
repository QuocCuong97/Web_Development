# Cú pháp jQuery
## **1) Cú pháp**
- Cú pháp của **jQuery** được tạo thành từ việc chọn phần tử **HTML** và thực hiện hành động lên phần tử đó :
- Cú pháp cơ bản :
    ```js
    $(selector).action()
    ```
    - Trong đó : 
        - `$` định nghĩa cấu trúc **jQuery**
        - `(selector)` là biểu thức truy vấn phần tử HTML
        - `action()` là hành động áp dụng lên phần tử được chọn
### **Selector**
- `$("*")` : chọn tất cả các phần tử
- `$(this)` : chọn phần tử hiện tại
- `$(".test")` : chọn tất cả các phần tử có class "`test`"
- `$("#test")` : chọn phần tử có id là "`test`"
- `$("p.intro")` : chọn tất cả các phần tử `<p>` có class "`intro`"
- `$("p:first")` : chọn phần tử `<p>` đầu tiên
- `$("ul li:first")` : chọn phần tử `<li>` đầu tiên của phần tử `<ul>` đầu tiên
- `$("ul li:first-child")` : chọn phần tử `<li>` đầu tiên của tất cả các phần tử `<ul>`
- `$("[href]")` : chọn tất cả các phần tử có thuộc tính `href`
- `$("a[target='_blank']")` : chọn tất cả các phần tử `<a>` với thuộc tính `target` có giá trị là "`_blank`"
- `$("a[target!='_blank'])` : chọn tất cả các phần tử `<a>` với thuộc tính `target` có giá trị **KHÔNG PHẢI** là "`_blank`"
- `$(":button")` : chọn tất cả các phần tử `<button>` và `<input>` có `type="button"`
- `$("tr:even")` : chọn tất cả các phần tử `<tr>` chẵn
- `$("tr:odd")` : chọn tất cả các phần tử `<tr>` lẻ
> Tham khảo thêm : [jQuery Selector Tester](https://www.w3schools.com/jquery/trysel.asp)
## **2) Document Ready Event**
- Tất cả cá phương thức **jQuery** sẽ được đặt trong **document ready event** :
    ```js
    $(document).ready(function(){
        // jQuery methods....
    });
    ```
- Việc này là để ngăn cho đoạn code **JQuery** chạy trước khi trang được load toàn bộ => Giúp tránh được một số lỗi như :
    - Cố gắng ẩn một phần tử chưa được tạo ra
    - Cố gắng lấy kích cỡ 1 ảnh chưa được load,.....
- **jQuery** đã tạo nên 1 phương thức rút gọn hơn cho **document ready event** :
    ```js
    $(function(){
        // jQuery methods....
    })