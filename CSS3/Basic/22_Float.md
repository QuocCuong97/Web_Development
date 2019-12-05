# CSS Layout - Thuộc tính `float` và `clear`
## **1) CSS `float`**
- Thuộc tính `float ` được sử dụng để khai báo cách phần tử được float
- Thuộc tính `float` có thể có các giá trị sau :
    - `left`
    - `right`
    - `none`
    - `inherit`
### **1.1) `float: right`**
- Với giá trị `right`, phần tử sẽ float sang bên phải của phần tử chứa nó .
- **VD :**
    ```html
    <style>
      img {
      float: right;
    }
    </style>
    <p><img src="pineapple.jpg" alt="Pineapple" style="width:170px;height:170px;margin-left:15px;">
    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus imperdiet, nulla et dictum interdum, nisi lorem egestas odio, vitae scelerisque enim ligula venenatis dolor. Maecenas nisl est, ultrices nec congue eget, auctor vitae massa. Fusce luctus vestibulum augue ut aliquet. Mauris ante ligula, facilisis sed ornare eu, lobortis in odio. Praesent convallis urna a lacus interdum ut hendrerit risus congue. Nunc sagittis dictum nisi, sed ullamcorper ipsum dignissim ac. In at libero sed nunc venenatis imperdiet sed ornare turpis. Donec vitae dui eget tellus gravida venenatis. Integer fringilla congue eros non fermentum. Sed dapibus pulvinar nibh tempor porta. Cras ac leo purus. Mauris quis diam velit.</p>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/YnWtZga.png>

### **1.2) `float: left`**
- Với giá trị `left`, phần tử sẽ float sang bên trái của phần tử chứa nó .
- **VD :**
    ```html
    <style>
      img {
      float: left;
    }
    </style>
    <p><img src="pineapple.jpg" alt="Pineapple" style="width:170px;height:170px;margin-right:15px;">
    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus imperdiet, nulla et dictum interdum, nisi lorem egestas odio, vitae scelerisque enim ligula venenatis dolor. Maecenas nisl est, ultrices nec congue eget, auctor vitae massa. Fusce luctus vestibulum augue ut aliquet. Mauris ante ligula, facilisis sed ornare eu, lobortis in odio. Praesent convallis urna a lacus interdum ut hendrerit risus congue. Nunc sagittis dictum nisi, sed ullamcorper ipsum dignissim ac. In at libero sed nunc venenatis imperdiet sed ornare turpis. Donec vitae dui eget tellus gravida venenatis. Integer fringilla congue eros non fermentum. Sed dapibus pulvinar nibh tempor porta. Cras ac leo purus. Mauris quis diam velit.</p>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/y6H7pJn.png>

### **1.3) `float: none`**
- Với giá trị `none`, phần tử sẽ không float mà sẽ hiển thị ở đúng vị trí của nó .
- **VD :**
    ```html
    <style>
    img {
      float: none;
    }
    </style>
    <p><img src="pineapple.jpg" alt="Pineapple" style="width:170px;height:170px;">
    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus imperdiet, nulla et dictum interdum, nisi lorem egestas odio, vitae scelerisque enim ligula venenatis dolor. Maecenas nisl est, ultrices nec congue eget, auctor vitae massa. Fusce luctus vestibulum augue ut aliquet. Mauris ante ligula, facilisis sed ornare eu, lobortis in odio. Praesent convallis urna a lacus interdum ut hendrerit risus congue. Nunc sagittis dictum nisi, sed ullamcorper ipsum dignissim ac. In at libero sed nunc venenatis imperdiet sed ornare turpis. Donec vitae dui eget tellus gravida venenatis. Integer fringilla congue eros non fermentum. Sed dapibus pulvinar nibh tempor porta. Cras ac leo purus. Mauris quis diam velit.</p>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/VUo1dPG.png>

### **1.4) `float: inherit`**
- Với giá trị `inherit`, phần tử sẽ thừa kế giá trị `float` từ phần tử cha .
## **2) Phần tử `clear`**
