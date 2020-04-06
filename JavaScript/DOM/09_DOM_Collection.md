# DOM Collection
## **1) `HTMLCollection` object**
- Phương thức `getElementsbyTagName` sẽ trả về `HTMLCollection` object .
- Một `HTMLCollection` object là một list (collection) các phần tử **HTML** .
- **VD :** Lấy tất cả các phần tử `<p>` :
    ```js
    var x = document.getElementsByTagName("p");
    ```
    - Để lấy phần tử `<p>` thứ 2 ta sẽ lấy theo dạng index (bắt đầu từ `0`) :
        ```js
        y = x[1];
        ```
## **2) `HTMLCollection` length**
- Thuộc tính `length` định nghĩa số lượng phần tử trong list `HTMLCollection` .
- **VD :**
    ```js
    var myCollection = document.getElementsByTagName("p");
    document.getElementById("demo").innerHTML = myCollection.length;
    ```
- Thuộc tính `length` cũng rất hữu ích khi tạo vòng lặp qua các phần tử trong `HTMLCollection` :
    ```js
    var myCollection = document.getElementsByTagName("p");
    var i;
    for (i = 0; i < myCollection.length; i++) {
      myCollection[i].style.backgroundColor = "red";
    }
    ```