# DOM Nodess
## **1) DOM Nodes**
- Theo chuẩn **HTML DOM** của **W3C**, tất cả mọi thứ trong HTML document là 1 **node** :
    - Toàn bộ document là một **document node** .
    - Tất cả các phần tử HTML là một **element node** .
    - Phần text bên trong các phần tử HTML là các **text node** .
    - Tất cả các thuộc tính HTML là một **attribute node** .
    - Tất cả các comment là các **comment node** .
- Với **HTML DOM**, tất cả các **node** trên cây **node** có thể được truy cập bằng **JavaScript** .
- Các **node** mới có thể được tạo ra, tất cả các **node** đều có thể bị chỉnh sửa hoặc bị xóa .

    <img src=https://i.imgur.com/JocbV80.png>

## **2) Mối quan hệ giữa các node**
- Các **node** trong cây **node** có mối quan hệ phân cấp với các **node** khác .
- Các khái niệm ***parent***, ***child*** và ***sibling*** được sử dụng để mô tả các mối quan hệ này :
    - Trong 1 cây **node**, **node** cao nhất được gọi là **root** (hay **root node**)
    - Tất cả các **node** nều có 1 và chỉ 1 ***parent***, ngoại trừ **root** ( không có ***parent*** )
    - Một **node** có thể có nhiều ***children***
    - ***Siblings*** là các **node** có chung ***parent*** .
- Mô tả cây **node** :

    <img src=https://i.imgur.com/iNUw8bj.png>

    - Từ sơ đồ này có thể thấy :
        - `<html>` là **root node** .
        - `<html>` không có ***parent*** .
        - `<html>` là ***parent*** của `<head>` và `<body>` .
        - `<head>` là ***first child*** của `<html>`
        - `<body>` là ***last child*** của `<html>`
    - Và :
        - `<head>` có 1 ***child*** : `<title>`
        - `<title>` có 1 ***child*** (**text node**) : "`DOM Tutorial`"
        - `<body>` có 2 ***child*** : `<h1>` và `<p>`
        - `<h1>` có 1 ***child*** : "`DOM Lesson one`"
        - `<p>` có 1 ***child*** : "`Hello World`"
        - `<h1>` và `<p>` là ***sibling***
## **3) Điều hướng giữa các node**
- Có thể sử dụng các thuộc tính **node** để điều hướng giữa các **node** bằng **JavaScript**  :
    - `parentNode`
    - `childNodes[`*`nodenumber`*`]`
    - `firstChild`
    - `lastChild`
    - `nextSibling`
    - `previousSibling`
## **4) Một số thuộc tính của node**
### **4.1) Child Nodes và Node Values**
- **VD :**
    ```html
    <title id="demo">DOM Tutorial</title>
    ```
    - **Element node** `<title>` này không chứa text .
    - Nó chứa một **text node** với giá trị là "`DOM Tutorial`"
    - Giá trị này có thể được truy xuất bằng thuộc tính `innerHTML` của **node** :
        ```js
        var myTitle = document.getElementById("demo").innerHTML;
        ```
    - Việc này cũng tương đương với việc lấy ra **nodeValue** của **textnode** ( chính là ***first child*** của `<title>` ) :
        ```js
        var myTitle = document.getElementById("demo").firstChild.nodeValue;
        ```
        hoặc sử dụng **node number** :
        ```js
        var myTitle = document.getElementById("demo").childNodes[0].nodeValue;
        ```
        => Kết quả của cả 3 cách trên đều là : `myTitle='DOM Tutorial'`
### **4.2) DOM Root Node**
- Có 2 thuộc tính đặc biệt cho phép truy cập toàn bộ HTML document :
    - `document.body` - Phần body của document ( nằm trong thẻ `<body>` )
    - `document.documentElement` - Toàn bộ document ( nằm trong thẻ `<html>` )
### **4.3) Thuộc tính `nodeName`**
- Thuộc tính `nodeName` chỉ ra tên của **node** :
    - `nodeName` là read-only
    - `nodeName` của **element node** chính là tên tag (UPPERCASE)
    - `nodeName` của **attribute node** chính là tên attribute
    - `nodeName` của **text node** sẽ luôn là `#text`
    - `nodeName` của **document node** sẽ luôn là `#document`
### **4.4) Thuộc tính `nodeValue`**
- Thuộc tính `nodeValue` chỉ ra giá trị của **node** :
    - `nodeValue` của **element node** luôn là `null`
    - `nodeValue` của **text node** chính là phần text đó
    - `nodeValue` của **attribute node** chính là giá trị của attribute
### **4.5) Thuộc tính `nodeType`**
- Thuộc tính `nodeType` là read-only . Nó trả về loại của **node**

| Node | Loại | VD | 
|------|------|----|
| ELEMENT_NODE | `1` | `<h1 class="heading">Hello World</h1>` |
| ATTRIBUTE_NODE | `2` | `class = "heading"` |
| TEXT_NODE | `3` | `Hello World` |
| COMMENT_NODE | `8` | `<!-- This is a comment -->` |
| DOCUMENT_NODE | `9` | Toàn bộ document( bao gồm cả thẻ `<html>` ) |
| DOCUMENT_TYPE_NODE | `10` | `<!DOCTYPE html>` |

- **VD :**
    ```html
    <h1 id="id01">My First Page</h1>
    <p id="id02"></p>

    <script>
    var type = document.getElementById("id01").nodeType;
    </script>
    ```
    => Kết quả : `type = 1`