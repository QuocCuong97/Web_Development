# DOM Node Lists
## **1) `NodeList` object**
- Một `NodeList` object là một list (collection) các **node** lấy được từ document .
- `NodeList` object gần giống với `HTMLCollection` object .
- Một số trình duyệt cũ trả về `NodeList` object thay vì `HTMLCollection` cho phương thức như `getElementsByClassName()` .
- Tất cả các trình duyệt sẽ trả về `NodeList` object cho phương thức `childNodes` .
- Hầu hết các trình duyệt trả về `NodeList` object cho phương thức `querySelectorAll()`
- **VD :** Lấy tất cả các phần tử `<p>` :
    ```js
    var myNodeList = document.querySelectorAll("p");
    ```
    - Để lấy phần tử `<p>` thứ 2 ta sẽ lấy theo dạng index (bắt đầu từ `0`) :
        ```js
        y = myNodeList[1];
        ```
## **2) `NodeList` length**
- Thuộc tính `length` định nghĩa số lượng **node** trong list `NodeList` .
- **VD :**
    ```js
    var myNodelist = document.querySelectorAll("p");
    document.getElementById("demo").innerHTML = myNodelist.length;
    ```
- Thuộc tính `length` cũng rất hữu ích khi tạo vòng lặp qua các **node** trong `NodeList` :
    ```js
    var myNodelist = document.querySelectorAll("p");
    var i;
      for (i = 0; i < myNodelist.length; i++) {
      myNodelist[i].style.backgroundColor = "red";
    }
    ```
## **3) Sự khác nhau giữa một `HTMLCollection` và một `NodeList`**
- Một `HTMLCollection` là tập hợp của các phần tử HTML .
- Một `NodeList` là tập hợp các **document node** .
- Cả 2 đều có thể sử dụng chỉ số index để access các item .
- `HTMLCollection` còn có thể sử dụng `name`, `id` để access các item .
