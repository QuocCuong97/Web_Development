# Screen
- **Object** `window.screen` bao hàm thông tin về màn hình mà user sử dụng .
- **Object** `window.screen` có thể được gọi mà không cần tiền tố `window` .
## **1) Chiều rộng màn hình**
- Thuộc tính `screen.width` trả về chiều rộng màn hình của user bằng đơn vị `pixels` . ( ở tỉ lệ màn hình `100%` )
- **VD :**
    ```js
    document.getElementById("demo").innerHTML = "Screen Width: " + screen.width;
    ```
    => Kết quả : `Screen Width: 1536`
## **2) Chiều cao màn hình**
- Thuộc tính `screen.height` trả về chiều cao màn hình cao màn hình của user bằng đơn vị `pixels` . ( ở tỉ lệ màn hình `100%` )
- **VD :**
    ```js
    document.getElementById("demo").innerHTML = "Screen Height: " + screen.height;
    ```
    => Kết quả : `Screen Height: 864`
## **3) Chiều rộng màn hình sẵn có**
- Thuộc tính `screen.availWidth` trả về chiều rộng màn hình của user bằng đơn vị `pixels`, trừ đi những yếu tố cố định ( như thanh **taskbar** ) . ( ở tỉ lệ màn hình `100%` )
> Thường thì kết quả trả về sẽ bằng với `screen.width`
- **VD :**
    ```js
    document.getElementById("demo").innerHTML = "Screen Available Width: " + screen.availWidth;
    ```
    => Kết quả : `Screen Available Width: 1536`
## **4) Chiều cao màn hình sẵn có**
- Thuộc tính `screen.availHeight` trả về chiều cao màn hình của user bằng đơn vị `pixels`, trừ đi những yếu tố cố định ( như thanh **taskbar** ) . ( ở tỉ lệ màn hình `100%` )
- **VD :**
    ```js
    document.getElementById("demo").innerHTML = "Screen Available Height: " + screen.availHeight;
    ```
    => Kết quả : `Screen Available Height: 824`
## **5) Độ sâu của màu (Color Depth)**
- Thuộc tính `screen.colorDepth` trả về số bit được sử dụng để hiển thị 1 màu .
- Tất cả các máy tính hiện đại ngày nay đều sử dụng phần cứng `24bit` hoặc `32bit` cho độ phân giải màu :
    - `24bit` - **True Colors** - Hiển thị `16,777,216` màu .
    - `30/32/36/48bit` - **Deep Colors** - Hiển thị `4,294,967,296` màu .
    - `8bit` - **VGA Colors** - Hiển thị `256` màu (điện thoại và máy tính đời cũ)
- **VD :**
    ```js
    document.getElementById("demo").innerHTML = "Screen Color Depth: " + screen.colorDepth;
    ```
    => Kết quả : `Screen Color Depth: 24`
