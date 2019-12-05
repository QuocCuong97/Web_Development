# CSS  Layout - Thuộc tính `overflow`
## **1) CSS `overflow`**
- Thuộc tính `overflow` kiểm soát việc gì sẽ xảy ra khi phần nội dung của phần tử quá lớn và không thể fit được diện tích của phần tử .
- Thuộc tính `overflow` có các giá trị sau :
    - `visible`
    - `hidden`
    - `scroll`
    - `auto`
> Thuộc tính `overflow` chỉ làm việc với phần tử block với `height` cho sẵn .
### **1.1) `overflow: visible`**
- Giá trị `visible` là mặc định . Phần content nếu quá khổ sẽ không bị cắt đi mà tràn ra ngoài phần tử .
- **VD :**
    ```html
    <style>
    div {
      width: 200px;
      height: 50px;
      background-color: #eee;
      overflow: visible;
    }
    </style>
    <div>You can use the overflow property when you want to have better control of the layout. The overflow property specifies what happens if content overflows an element's box.</div>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/KEDpsuT.png>

### **1.2) `overflow: hidden`**
- Với giá trị `hidden` , phần nội dung không thể fit với phần tử sẽ bị cắt đi và không nhìn thấy được .
- **VD :**
    ```html
    <style>
    div {
      background-color: #eee;
      width: 200px;
      height: 50px;
      border: 1px dotted black;
      overflow: hidden;
    }
    </style>
    <div>You can use the overflow property when you want to have better control of the layout. The overflow property specifies what happens if content overflows an element's box.</div>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/8hur20I.png>

### **1.3) `overflow: scroll`**
- Với giá trị `scroll`, phần nội dung không thể fit với phần tử sẽ bị cắt đi , tuy nhiên vẫn có thanh scrollbar để kéo xuống dưới và nhìn thấy chúng .
- **VD :**
    ```html
    <style>
    div {
      background-color: #eee;
      width: 200px;
      height: 100px;
      border: 1px dotted black;
      overflow: scroll;
    }
    </style>
    <div>You can use the overflow property when you want to have better control of the layout. The overflow property specifies what happens if content overflows an element's box.</div>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/rzOevsR.png>

### **1.4) `overflow: auto`**
- Giá trị `auto` cũng tương tự như `scroll`, nhưng chỉ thêm scrollbar khi cần thiết .
- **VD :**
    ```html
    <style>
    div {
      background-color: #eee;
      width: 200px;
      height: 100px;
      border: 1px dotted black;
      overflow: auto;
    }
    </style>
    <div>You can use the overflow property when you want to have better control of the layout. The overflow property specifies what happens if content overflows an element's box.</div>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/fhEGUB4.png>

## **2) Thuộc tính `overflow-x` và `overflow-y`**
- Thuộc tính `overflow-x` và `overflow-y` sẽ cho phép luồng content được cuộn lên xuống hay cuộn ngang ( hoặc cả hai ) :
    - `overflow-x` : thanh cuộn (scrollbar) ngang
    - `overflow-y` : thanh cuộn (scrollbar) dọc
- Các giá trị có thể :
    - `hidden` : ẩn scrollbar
    - `scroll` : mặc định . hiện scrollbar
- **VD :**
    ```html
    <style>
    div {
      background-color: #eee;
      width: 200px;
      height: 50px;
      border: 1px dotted black;
      overflow-x: hidden;
      overflow-y: scroll;
    }
    </style>
    <div>You can use the overflow property when you want to have better control of the layout. The overflow property specifies what happens if content overflows an element's box.</div>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/7vYL4AR.png>
