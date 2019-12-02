# CSS Selector
## **1) Giới thiệu**
- **CSS selectors** được sử dụng để tìm kiếm ( hoặc chọn ) phần tử **HTML** muốn áp dụng style
- Có thể chia **CSS selectors** thành 5 mục :
    - **Simple selectors** - chọn phần tử dựa trên `name`, `id`, `class`
    - **Combinator selectors** - chọn phần tử dựa trên những mối quan hệ đặc biệt giữa chúng 
    - **Pseudo-class selectors** - chọn phần tử dựa trên những trạng thái nhất định
    - **Pseudo-elements selectors** - chọn và áp dụng style cho 1 phần của phần tử
    - **Attribute selectors** - chọn phần tử dựa trên thuộc tính và giá trị của thuộc tính
## **2) Simple selectors**
### **2.1) Chọn phần tử dựa theo tên**
- **VD :**
    ```css
    p {
      text-align: center;
      color: red;
    }
    ```
### **2.2) Chọn phần tử dựa theo `id`**
- **VD :**
    ```css
    #para1 {
      text-align: center;
      color: red;
    }
    ```
### **2.3) Chọn phần tử dựa theo `class`**
- **VD :**
    ```css
    .center {
      text-align: center;
      color: red;
    }
    ```
## **3) Combinator selectors**
- Ký hiệu universal selector ( "`*`" ) chọn tất cả các phần tử **HTML** trên page .
- **VD :**
    ```css
    * {
      text-align: center;
      color: blue;
    }
    ```
## **4) Grouping Selector**
- Grouping selector sẽ chọn tất cả các phần tử có cùng kiểu style .
- **VD :**
    ```css
    h1 {
      text-align: center;
      color: red;
    }

    h2 {
      text-align: center;
      color: red;
    }

    p {
      text-align: center;
      color: red;
    }
    ```
    - Có thể viết gọn lại thành :
    ```css
    h1, h2, p {
      text-align: center;
      color: red;
    }
    ```



