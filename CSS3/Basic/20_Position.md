# CSS Layout - Thuộc tính `position`
## **1) CSS `position`**
- Thuộc tính `position` khai báo phương thức vị trí được sử dụng bởi một phần tử .
- Có 5 giá trị của thuộc tính `position` :
    - `static`
    - `relative`
    - `fixed`
    - `absolute`
    - `sticky`
### **1.1) `position: static`**
- Phần tử **HTML** sử dụng `position: static` là mặc định .
- Phần tử được trỏ `static` sẽ không ảnh hưởng đến các thuộc tính `top`, `bottom`, `left`, `right` .
- Phần tử được trỏ `static` sẽ không thay đổi vị trí mà sẽ ở đúng vị trí đã code trong trang web .
- **VD :**
    ```css
    div.static {
      position: static;
      border: 3px solid #73AD21;
    }
    ```
### **1.2) `position: relative`**
- 