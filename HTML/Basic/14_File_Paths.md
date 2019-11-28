# File Paths
- Đường dẫn file mô tả vị trí của 1 file trong cấu trúc thư mục của website .
- Đường dẫn file thường được sử dụng để link đến các file ngoài như :
    - Trang web
    - Ảnh
    - File style ( CSS )
    - JavaScripts

- Các kiểu đường dẫn file : 
    - `<img src="picture.jpg">` : file `picture.jpg` được đặt cùng thư mục với page ( file `index.html` )
    - `<img src="images/picture.jpg">` : file `picture.jpg` được đặt tạo thư mục `images` ở cùng thư mục với page ( file `index.html` )
    - `<img src="/images/picture.jpg">` : file `picture.jpg` 
    được đặt trong thư mục `images` ở trong thư mục root của page
    - `<img src="../picture.jpg">` : file `picture.jpg` được đặt ở thư mục cha của thư mục hiện tại đang chứa page

- **Đường dẫn tuyệt đối** : là đường dẫn full địa chỉ URL trên internet của file .
    ```html
    <img src="https://www.w3schools.com/images/picture.jpg" alt="Mountain">
    ```
- **Đường dẫn tương đối** : là đường dẫn trỏ đến file local có mỗi quan hệ với file `index.html` của website .
    ```html
    <img src="/images/picture.jpg" alt="Mountain">
    ```
