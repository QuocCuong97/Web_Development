# Colors
## **1) Giới thiệu**
- Màu sắc trong **CSS** được diễn tả qua tên màu , hoặc giá trị **RGB** , **HEX** , **HSL** , **RGBA** , **HSLA** .
## **2) Tên màu**
- **HTML** hỗ trợ tới `140` chuẩn tên màu ( [Danh sách các tên màu](https://www.w3schools.com/colors/colors_names.asp) ) :

    <img src=https://i.imgur.com/P4Flfjg.png>

- Có thể tìm màu mong muốn qua công cụ [**Color Picker**](https://www.w3schools.com/colors/colors_picker.asp) của **W3Schools**
## **3) Các giá trị màu**
### **3.1) RGB**
- Trong **HTML** , màu có thể được đặc tả qua giá trị **RGB** , sử dụng công thức :
    ```html
    rgb(red, green, blue)
    ```
- Mỗi tham số `red` , `green` , `blue` định nghĩa cho cường độ màu , có giá trị từ `0 -> 255` .
- **VD :**
    - Màu đỏ ( `red` ) : `(255, 0, 0)`
    - Màu đen ( `black` ) : `(0, 0, 0)`
    - Màu trắng ( `white` ) : `(255, 255, 255)`

        <img src=https://i.imgur.com/604XOPd.png>

- Các gam màu xám , đen , trắng được định nghĩa với 3 giá trị `red` , `green` , `blue` bằng nhau :

    <img src=https://i.imgur.com/Jo65m7D.png>

### **3.2) HEX**
- Trong **HTML** , màu có thể được đặc tả qua giá trị thập lục phân ( *hexadecimal* ) , sử dụng công thức :
    ```html
    #rrggbb
    ```
- Trong đó , `rr` - red , `gg` - green , `bb` - blue là các giá trị thập lục phân từ `00 -> ff` ( tương tự như `0 -> 255` ) .
- **VD :** 
    - `#ff0000` : màu đỏ
    - `#000000` : màu đen
    - `#ffffff` : màu trắng

        <img src=https://i.imgur.com/4bPDq8K.png>

- Các gam màu xám , đen , trắng được định nghĩa với 3 giá trị `rr` , `gg` , `bb` bằng nhau :

    <img src=https://i.imgur.com/fWeEeOK.png>

### **3.3) HSL**
- Trong **HTML** , màu có thể được đặc tả qua giá trị tông màu ( ***hue*** ) , độ bão hòa màu ( ***saturation*** ) , độ sáng ( ***lightness*** ) sử dụng công thức :
    ```html
    hsl(hue, saturation, lightness)
    ```
#### **3.3.1) Hue - Tông màu**
- **Hue** là giá trị góc của màu tính trên vòng màu từ `0 -> 360` . `0` là red , `120` là green , `240` là blue .

<p align=center><img src=https://i.imgur.com/TbGKe2R.png width=50%></p>

- **VD :**
    
    <img src=https://i.imgur.com/WSdaDun.png>

#### **3.3.2) Saturation - Độ bão hòa màu**
- **Saturation** là giá trị phần trăm :
    - `100%` là màu nguyên chất
    - `%50%` là `50%` màu pha với `50%` màu xám , tuy nhiên vẫn có thể nhìn thấy màu .
    - `0%` thể hiện gam màu đen , xám , trắng , không còn nhìn thấy màu sắc nữa .
- **VD :**

    <img src=https://i.imgur.com/F550yFI.png>

#### **3.3.3) Lightness - Độ sáng**
- **Lightness** cũng là giá trị phần trăm :
    - `0%` là màu đen
    - `%50` là bình thường , không sáng cũng không tối
    - `100%` là màu trắng
- **VD :**

    <img src=https://i.imgur.com/yYvO40A.png>

- Gam màu đen , xám , trắng thường được định nghĩa bằng cách đặt giá trị **hue** và **saturation** thành `0` , sau đó điều chỉnh độ sáng từ `0%` đến `100%` :

    <img src=https://i.imgur.com/JmEwtww.png>

### **3.4) RGBA**
- Giá trị màu **RGBA** là mở rộng của **RGB** với tham số `alpha` thể hiện sự trong suốt ( ***opacity*** ) của màu được thêm vào .
- Công thức :
    ```html
    rgba(red, green, blue, alpha)
    ```
- Tham số `alpha` có giá trị từ `0.0` ( hoàn toàn trong suốt - ***fully transparent*** ) đến `1` ( đặc màu )

    <img src=https://i.imgur.com/C7JKnbB.png>

### **3.5) HSLA**
- Giá trị màu **HSLA** là mở rộng của **HSL** với tham số `alpha` thể hiện sự trong suốt ( ***opacity*** ) của màu được thêm vào .
- Công thức :
    ```html
    hsl(hue, saturation, lightness, alpha)
    ```
- Tham số `alpha` có giá trị từ `0.0` ( hoàn toàn trong suốt - ***fully transparent*** ) đến `1` ( đặc màu )

    <img src=https://i.imgur.com/ofC94cc.png>

## **4) Cách biểu diễn màu**
- Sử dụng thuộc tính `<style>` với tham số `color` để biểu diễn màu theo công thức :
    ```html
    <style="color:color_value;">Text</style>
    ```
### **4.1) Màu chữ - Text Color**
- **VD :**
    ```html
    <h1 style="color:Tomato;">Hello World</h1>
    <p style="color:DodgerBlue;">Lorem ipsum...</p>
    <p style="color:MediumSeaGreen;">Ut wisi enim...</p>
    ```
    => Hiển thị trên trình duyệt :

    <img src=https://i.imgur.com/ZhAhvDr.png>

### **4.2) Màu viền - Border Color**
- **VD :**
    ```html
    <h1 style="border:2px solid Tomato;">Hello World</h1>
    <h1 style="border:2px solid DodgerBlue;">Hello World</h1>
    <h1 style="border:2px solid Violet;">Hello World</h1>
    ```
    => Hiển thị trên trình duyệt :

    <img src=https://i.imgur.com/a9gb7oL.png>

### **4.3) Màu nền - Background Color**
- **VD :**
    ```html
    <h1 style="background-color:DodgerBlue;">Hello World</h1>
    <p style="background-color:Tomato;">Lorem ipsum...</p>
    ```
    => Hiển thị trên trình duyệt :

    <img src=https://i.imgur.com/JvAHrUJ.png>