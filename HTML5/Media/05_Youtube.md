# HTML Youtube Video
## **1) Giới thiệu**
- Cách tốt nhất để chạy video trên **HTML** , là sử dụng **Youtube** .
- **Youtube** sẽ hiển thị 1 id ( giống như `tgbNymZ7vqY` ) khi lưu lại ( hoặc play ) một video . Lưu lại id này để gắn vào HTML code .

    <img src=https://i.imgur.com/T3HHnbg.png>

## **2) Chạy Youtube Video trong HTML**
- Để chạy mội video trong trang web, làm theo các bước sau :
    - Upload video lên **Youtube** 
    - Ghi chú lại id của video 
    - Định nghĩa 1 phần tử `<iframe>` trong trang web
    - Trỏ thuộc tính `src` vào URL của video 
    - Sử dụng thuộc tính `width` và `height` để xác định kích cỡ của iframe 
    - Thêm các tham số khác vào URL
- **VD :**
    ```html
    <iframe width="620" height="315"
    src="https://www.youtube.com/embed/GQ4F9k4USfA">
    </iframe>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/oviHlfU.png>

### **2.1) Youtube Autoplay**
- Có thể cho phép video tự động khởi chạy khi có người dùng mở trang web bằng cách thêm tham số `autoplay` vào đường dẫn **Youtube** .
    - `autoplay=0` ( mặc định ) : video sẽ không tự động chạy khi user load trang web .
    - `autoplay=1` : video sẽ tự động chạy khi có user load trang web .
- **VD :**
    ```html
    <iframe width="420" height="315"
    src="https://www.youtube.com/embed/GQ4F9k4USfA?autoplay=1">
    </iframe>
    ```
### **2.2) Youtube Playlist**
- Có thể khởi tạo 1 playlist các video youtube được phát bằng cách thêm tham số `playlist` vào đường dẫn URL, mỗi id được ngăn cách với nhau bằng 1 dấu phẩy "`,`" .
- **VD :**
    ```html
    <iframe width="420" height="345" src="https://www.youtube.com/embed/tgbNymZ7vqY?playlist=GQ4F9k4USfA,AiD1a2fFFLw">
    </iframe>
    ```
### **2.3) Youtube Loop**
- Có thể cài đặt tính năng lặp lại tự động một 1 video bằng cách thêm tham số `loop` :
    - `loop=0` ( mặc định ) : video sẽ chỉ chạy 1 lần
    - `loop=1` : video sẽ tự động lặp lại (mãi mãi)
- **VD :**
    ```html
    <iframe width="420" height="315"
    src="https://www.youtube.com/embed/GQ4F9k4USfA?playlist=GQ4F9k4USfA&loop=1">
    </iframe>
    ```
### **2.4) Youtube Controls**
- Có thể cho phép thanh điều khiển video được hiển thị hoặc không hiển thị bằng cách thêm tham số `controls` :
    - `controls=0` : không hiển thị thanh điều khiển
    - `controls=1` ( mặc định ) :  hiển thị thanh điều khiển 

        <img src=https://i.imgur.com/0pAxJl9.png>

- **VD :**
    ```html
    <iframe width="420" height="315"
    src="https://www.youtube.com/embed/GQ4F9k4USfA?controls=0">
    </iframe>
    ```
