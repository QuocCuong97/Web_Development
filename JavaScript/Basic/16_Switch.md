# Switch...case
- Mệnh đề `switch` được sử dụng để lựa chọn các khối code thực hiện khác nhau dựa vào các điều kiện khác nhau .
- Mệnh đề `switch` cũng được tính là mệnh đề điều kiện, ý nghĩa tương tự cấu trúc `if...else if...else`
- Cú pháp :
    ```js
    switch(expression) {
      case x:
        // code block
        break;
      case y:
        // code block
        break;
      default:
        // code block
    }
    ```
- Nếu các `case` đều thỏa mãn , `case` đầu tiên sẽ được chọn .
- Nếu không có `case` nào thỏa mãn , chương trình sẽ thực hiện khối code có nhãn `default` .
- Nếu không khai báo nhãn `default`, chương trình sẽ tiếp tục các câu lệnh phía sau cụm `switch...case` .
- Từ khóa `switch` được sử dụng để thoát ra khỏi toàn bộ khối lệnh `switch` . Không cần thiết phải khai báo `break` trong case cuối cùng .
- **VD :**
    ```js
    switch (new Date().getDay()) {
      case 0:
        day = "Sunday";
        break;
      case 1:
        day = "Monday";
        break;
      case 2:
        day = "Tuesday";
        break;
      case 3:
        day = "Wednesday";
        break;
      case 4:
        day = "Thursday";
        break;
      case 5:
        day = "Friday";
        break;
      case 6:
        day = "Saturday";
    }
    document.getElementById("demo").innerHTML = "Today is " + day;
    ```
    => Kết quả : `Today is Tuesday`
### **Gộp chung các điều kiện có code block giống nhau**
- **VD :**
    ```js
    switch (new Date().getDay()) {
      case 4:
      case 5:
        text = "Soon it is Weekend";
        break;
      case 0:
      case 6:
        text = "It is Weekend";
        break;
      default:
        text = "Looking forward to the Weekend";
    }
    ```
## **Strict Comparison**
