# Dates
## **1) JavaScript Date Output**
- Mặc định , **JavaScript** sẽ sử dụng time zone của trình duyệt và hiển thị thông tin ngày tháng ở dạng chuỗi :
    ```js
    Tue Dec 17 2019 00:49:13 GMT+0700 (Indochina Time)
    ```
## **2) Các cách khởi tạo một Date object**
- Một **date object** có thể được tạo ra qua cấu trúc `new Date()`
- Có 4 cách tạo **date object**  :
### **2.1) `new Date()`**
- Cấu trúc `new Date()` tạo ra một **date object** với giá trị là thời gian hiện tại .
- **Date object** là một dạng tĩnh . Nó chỉ nhận giá trị đúng thời gian nó chạy, sau đó sẽ không thay đổi cho dù thời gian trên máy tính có trôi đi .
- **VD :**
    ```js
    var d = new Date();
    ```
    => Kết quả : `d = Tue Dec 17 2019 00:57:26 GMT+0700 (Indochina Time)`
### **2.2) `new Date(`*`year, month, day, hours, minutes, seconds, milliseconds`*`)`**
- Cấu trúc này tạo ra một **date object** với ngày và thời gian được xác định trước .
- 7 tham số đi kèm tượng trưng cho năm, tháng, ngày, giờ, phút, giây, và miligiây .
- Giá trị của các tham số :
    - Tham số ***tháng*** được tính từ `0 - 11` với tháng 1 là `0` ... tháng `12` là `11` .
    - Tham số ***ngày*** được tính từ `1 - 31`
    - Tham số ***giờ*** được tính từ `0 - 23`
    - Tham số ***phút*** được tính từ `0 - 59`
    - Tham số ***giây*** được tính từ `0 - 59`
    - Tham số ***miligiây*** được tính từ `0 - 999`
- **VD1 :** Khai báo đầy đủ `7` tham số :
    ```js
    var d = new Date(2018, 11, 24, 10, 33, 30, 0);
    ```
    => Kết quả : `d = Mon Dec 24 2018 10:33:30 GMT+0700 (Indochina Time)`
- **VD2 :** Khai báo `6` tham số (bỏ qua miligiây) :
    ```js
    var d = new Date(2018, 11, 24, 10, 33, 30);
    ```
    => Kết quả : `d = Mon Dec 24 2018 10:33:30 GMT+0700 (Indochina Time)`
- **VD3 :** Khai báo `5` tham số (bỏ qua giây và miligiây) :
    ```js
    var d = new Date(2018, 11, 24, 10, 33);
    ```
    => Kết quả : `d = Mon Dec 24 2018 10:33:00 GMT+0700 (Indochina Time)`
- **VD4 :** Khai báo `4` tham số (bỏ qua phút, giây, miligiây) :
    ```js
    var d = new Date(2018, 11, 24, 10);
    ```
    => Kết quả : `d = Mon Dec 24 2018 10:00:00 GMT+0700 (Indochina Time)`
- **VD5 :** Khai báo `3` tham số (bỏ qua giờ, phút, giây, miligiây) :
    ```js
    var d = new Date(2018, 11, 24);
    ```
    => Kết quả : `d = Mon Dec 24 2018 00:00:00 GMT+0700 (Indochina Time)`
- **VD6 :** Khai báo `2` tham số (năm và tháng) :
    ```js
    var d = new Date(2018, 11);
    ```
    => Kết quả : `d = Sat Dec 01 2018 00:00:00 GMT+0700 (Indochina Time)`
- **VD7 :** Chỉ khai báo năm ( không được phép ) :
    ```js
    var d = new Date(2018);
    ```
    => Kết quả : `d = Thu Jan 01 1970 07:00:02 GMT+0700 (Indochina Time)`
- **VD8 :** Sử dụng 2 chữ số cuối của năm để khai báo năm `19xx` :
    ```js
    var d = new Date(9, 11, 24);
    ```
    => Kết quả : `d = Fri Dec 24 1909 00:00:00 GMT+0642 (Indochina Time)`
### **2.3) `new Date(`*`dateString`*`)`**
- Cấu trúc này tạo một **date object** từ một **date string** có sẵn .
- **VD :**
    ```js
    var d = new Date("October 13, 2014 11:13:00");
    ```
    => Kết quả : `d = Mon Oct 13 2014 11:13:00 GMT+0700 (Indochina Time)`
### **2.4) `new Date(`*`milliseconds`*`)`**
- Cấu trúc này tạo một **date object** với thời điểm là sau ngày `01/01/1970 00:00:00` ( theo giờ tiêu chuẩn `UTC` ) một khoảng thời gian ***`milliseconds`*** . Các thông tin về thời gian của **date object** sẽ được hệ thống tự động xác định dựa vào thời điểm đó.
- **VD :** 
    ```js
    var d = new Date(100000000000);
    ```
    => Kết quả : `d = Sat Mar 03 1973 16:46:40 GMT+0700 (Indochina Time)`
## **3) Các định dạng ngày tháng - Date Format**
- Không phụ thuộc vào cách input , **JavaScript** sẽ đưa ra output mặc định ở dạng full text string :
    ```js
    Wed Mar 25 2015 07:00:00 GMT+0700 (Indochina Time)
    ```
### **3.1) ISO Date**
- Chuẩn **ISO 8601** là chuẩn quốc tế để hiển thị ngày giờ .
- Cú pháp của chuẩn **ISO 8601** ( `YYYY-MM-DD` ) cũng được ưu tiên trong **JavaScript** :
    ```js
    var d = new Date("2015-03-25");
    ```
    => Kết quả : `d = Wed Mar 25 2015 07:00:00 GMT+0700 (Indochina Time)`
- Chuẩn **ISO** này cũng có thể được khai báo mà không cần ngày ( `YYYY-MM` ) kèm theo :
    ```js
    var d = new Date("2015-03");
    ```
    => Kết quả : `d = Sun Mar 01 2015 07:00:00 GMT+0700 (Indochina Time)`
- Hoặc cũng có thể khai báo với mỗi năm ( `YYYY` ) :
    ```js
    var d = new Date("2015");
    ```
    => Kết quả : `d = Thu Jan 01 2015 07:00:00 GMT+0700 (Indochina Time)`
- Có thể thêm giờ - phút - giây - miligiây theo cấu trúc ( `YYYY-MM-DDTHH:MM:SSZ` )
    - Trong giờ và ngày được ngăn cách với nhau bởi ký tự "`T`"
    - **UTC** time được định nghĩa bằng ký tự "`Z`" 
    - Thuật ngữ **UTC** ( **Universal Time Coordinated** ) tương đương với thuật ngữ **GMT** ( **Greenwich Mean Time** ) .
    - Khi khai báo date-time , kết quả trả về sẽ tùy theo múi giờ của trình duyệt .
    - Nếu không muốn sử dụng thời gian tương đối `UTC` , sử dụng theo cấu trúc `+HH:MM` hoặc `-HH:MM`
    - **VD1 :**
        ```js
        var d = new Date("2015-03-25T12:00:00Z");
        ```
        => Kết quả : `d = Wed Mar 25 2015 19:00:00 GMT+0700 (Indochina Time)`
    - **VD2 :** 
        ```js
        var d = new Date("2015-03-25T12:00:00-06:30");
        ```
        => Kết quả : `d = Thu Mar 26 2015 01:00:00 GMT+0700 (Indochina Time)`
### **3.2) Short Date**
- Cấu trúc **short date** sẽ được viết theo định dạng "`MM/DD/YYYY`" :
    ```js
    var d = new Date("03/25/2015");
    ```
    => Kết quả : `d = Wed Mar 25 2015 00:00:00 GMT+0700 (Indochina Time)`
### **3.3) Long Date**
- Cấu trúc **long date** thường được viết theo định dạng "`MMM DD YYYY`" :
    ```js
    var d = new Date("Mar 25 2015");
    ```
    => Kết quả : `d = Wed Mar 25 2015 00:00:00 GMT+0700 (Indochina Time)`
    hoặc cũng có thể viết :
    ```js
    var d = new Date("25 Mar 2015");
    ```
    hoặc cũng có thể viết :
    ```js
    var d = new Date("January 25 2015");
    ```
    hoặc cũng có thể viết hoa hoặc thêm dấu phẩy :
    ```js
    var d = new Date("JANUARY, 25, 2015");
    ```
## **4) Các phương thức Get**
- Các phương thức Get được sử dụng để lấy thông tin từ một **date object**
### **4.1) Phương thức `getTime()`**
- Phương thức `getTime()` trả về số giây tính từ `January 1, 1970` đến thời điểm cần xét .
- **VD :**
    ```js
    var d = new Date();
    document.getElementById("demo").innerHTML = d.getTime();
    ```
    => Kết quả : `1577723145368`
### **4.2) Phương thức `getFullYear()`**
- Phương thức `getFullYear()` trả về thông số ***year*** của **date object** đang xét với định dạng `4` chữ số .
- **VD :**
    ```js
    var d = new Date();
    document.getElementById("demo").innerHTML = d.getFullYear();
    ```
    => Kết quả : `2019`
### **4.3) Phương thức `getMonth()`**
- Phương thức `getMonth()` trả về thông số ***month*** của **date object** đang xét dưới định dạng số ( `0 - 11` )
- **VD :**
    ```js
    var d = new Date();
    document.getElementById("demo").innerHTML = d.getMonth();
    ```
    => Kết quả : `11`
- Cũng có thể sử dụng mảng để trả về ***month*** dạng chữ :
    ```js
    var d = new Date();
    var months = ["January", "February", "March", "April", "May", "June", "July", "August", "September", "October", "November", "December"];
    document.getElementById("demo").innerHTML = months[d.getMonth()];
    ```
    => Kết quả : `December`
### **4.4) Phương thức `getDate()`**
- Phương thức `getDate()` trả về thông số ***date*** của **date object** đang xét dưới dạng số ( `1 - 31` )
- **VD :**
    ```js
    var d = new Date();
    document.getElementById("demo").innerHTML = d.getDate();
    ```
    => Kết quả : `30`
### **4.5) Phương thức `getHours()`**
- Phương thức `getHours()` trả về thông số ***hour*** của **date object** đang xét dưới dạng số ( `0 - 23` )
- **VD :**
    ```js
    var d = new Date();
    document.getElementById("demo").innerHTML = d.getHours();
    ```
    => Kết quả : `23`
### **4.6) Phương thức `getMinutes()`**
- Phương thức `getMinutes()` trả về thông số ***minute*** của **date object** đang xét dưới dạng số ( `0 - 59` )
- **VD :**
    ```js
    var d = new Date();
    document.getElementById("demo").innerHTML = d.getMinutes();
    ```
    => Kết quả : `48`
### **4.7) Phương thức `getSeconds()`**
- Phương thức `getSeconds()` trả về thông số ***second*** của **date object** đang xét dưới dạng số ( `0 - 59` )
- **VD :**
    ```js
    var d = new Date();
    document.getElementById("demo").innerHTML = d.getSeconds();
    ```
    => Kết quả : `55`
### **4.8) Phương thức `getMiliseconds()`** 
- Phương thức `getMiliseconds()` trả về thông số ***milisecond*** của **date object** đang xét dưới dạng số ( `0 - 999` )
- **VD :**
    ```js
    var d = new Date();
    document.getElementById("demo").innerHTML = d.getMilliseconds();
    ```
    => Kết quả : `467`
### **4.9) Phương thức `getDay()`**
- Phương thức `getDay()` trả về ngày trong tuần của tương ứng với **date object** đang xét dưới dạng số ( `0 - 6` ) trong đó `0` là `Sunday`, `1` là `Monday` ,....
- **VD :**
    ```js
    var d = new Date();
    document.getElementById("demo").innerHTML = d.getDay();
    ```
    => Kết quả : `1`
- Có thể sử dụng mảng để trả về ***day*** dạng chữ :
    ```js
    var d = new Date();
    var days = ["Sunday", "Monday", "Tuesday", "Wednesday", "Thursday", "Friday", "Saturday"];
    document.getElementById("demo").innerHTML = days[d.getDay()];
    ```
    => Kết quả : `Monday`
### **4.10) Phương thức date UTC**
## **5) Các phương thức Set**
- Các phương thức Set được sử dụng để đặt giá trị ( ***year, month, day, hour, minute, second, milisecond*** ) cho **date object**
### **5.1) Phương thức `setFullYear()`**
- Phương thức `setFullYear()` sẽ đặt lại giá trị của ***year*** của **date object** ( cho dù nó đã có một giá trị khác )
- **VD :**
    ```js
    var d = new Date();
    d.setFullYear(2020);
    document.getElementById("demo").innerHTML = d;
    ```
    => Kết quả : `d = Thu Dec 31 2020 00:06:17 GMT+0700 (Indochina Time)`
- Phương thức `setFullYear()` có thể chứa thêm các thông số để đặt lại ngày và tháng :
    ```js
    var d = new Date();
    d.setFullYear(2020, 11, 3);
    document.getElementById("demo").innerHTML = d;
    ```
    => Kết quả : `d = Thu Dec 03 2020 00:09:07 GMT+0700 (Indochina Time)`
### **5.2) Phương thức `setMonth()`**
- Phương thức `setMonth()` sẽ đặt lại giá trị của ***month*** của **date object** ( cho dù nó đã có một giá trị khác ) ( `0 - 11` )
- **VD :**
    ```js
    var d = new Date();
    d.setMonth(11);
    document.getElementById("demo").innerHTML = d;
    ```
    => Kết quả : `d = Tue Dec 31 2019 00:08:10 GMT+0700 (Indochina Time)`
### **5.3) Phương thức `setDate()`**
- Phương thức `setDate()` sẽ đặt lại giá trị của ***date*** của **date object** ( cho dù nó đã có một giá trị khác ) ( `1 - 31` )
- **VD :**
    ```js
    var d = new Date();
    d.setDate(15);
    document.getElementById("demo").innerHTML = d;
    ```
    => Kết quả : `d = Sun Dec 15 2019 00:12:22 GMT+0700 (Indochina Time)`
- Có thể sử dụng phương thức `setDate()` để cộng thêm một số ngày cho ***date*** :
    ```js
    var d = new Date();
    d.setDate(d.getDate() + 50);
    document.getElementById("demo").innerHTML = d;
    ```
    => Kết quả : `d = Wed Feb 19 2020 00:14:17 GMT+0700 (Indochina Time)`
### **5.4) Phương thức `setHours()`**
- Phương thức `setHours()` sẽ đặt lại giá trị của ***hour*** của **date object** ( cho dù nó đã có một giá trị khác ) ( `0 - 23` )
- **VD :**
    ```js
    var d = new Date();
    d.setHours(22);
    document.getElementById("demo").innerHTML = d;
    ```
    => Kết quả : `d = Tue Dec 31 2019 22:17:12 GMT+0700 (Indochina Time)`
### **5.5) Phương thức `setMinutes()`**
- Phương thức `setMinutes()` sử dụng để đặt lại giá trị ***minute*** của **date object** ( cho dù nó đã có một giá trị khác ) ( `0 - 59` )
- **VD :**
    ```js
    var d = new Date();
    d.setMinutes(30);
    document.getElementById("demo").innerHTML = d;
    ```
    => Kết quả : `d = Tue Dec 31 2019 00:30:05 GMT+0700 (Indochina Time)`
### **5.6) Phương thức `setSeconds()`**
- Phương thức `setSeconds()` sử dụng để đặt lại giá trị ***second*** của **date object** ( cho dù nó đã có một giá trị khác ) ( `0 - 59` )
- **VD :**
    ```js
    var d = new Date();
    d.setSeconds(30);
    document.getElementById("demo").innerHTML = d;
    ```
    => Kết quả : `d = Tue Dec 31 2019 00:21:30 GMT+0700 (Indochina Time)`
### **5.7) So sánh các date object**
- **Date** có thể được so sánh dễ dàng với nhau .
- **VD :**
    ```js
    var today, someday, text;
    today = new Date();
    someday = new Date();
    someday.setFullYear(2100, 0, 14);

    if (someday > today) {
      text = "Today is before January 14, 2100.";
    } else {
      text = "Today is after January 14, 2100.";
    }
    document.getElementById("demo").innerHTML = text;
    ```
    => Kết quả : `Today is before January 14, 2100.`

    