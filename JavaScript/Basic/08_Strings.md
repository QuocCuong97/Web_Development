# String
## **1) Kiểu dữ liệu `string`**
- Là một chuỗi các ký tự, được đặt trong dấu nháy đơn ( `''` ) hoặc dấu ngoặc kép ( `""` ) .
- **VD :**
    ```js
    var answer1 = "It's alright";             // Single quote inside double quotes
    var answer2 = "He is called 'Johnny'";    // Single quotes inside double quotes
    var answer3 = 'He is called "Johnny"';    // Double quotes inside single quotes
    ```
## **2) Escape Sequence**
- **VD :** 
    ```js
    var x = "We are the so-called "Vikings" from the north.";
    ```
    - Kết quả : `x = "We are the so-called "` <br>=> Nội dung của chuỗi bị nhầm lẫn
- Để tránh trường hợp này xảy ra, sử dụng **escape character** .
- Dấu "`\`" trong **escape sequence** sẽ chuyển các ký tự đặc biệt sau nó thành string :

    | Escape Sequence | Kết quả | Mô tả |
    |-----------------|---------|-------|
    | `\'` | `'` | Dấu nháy đơn |
    | `\"` | `"` | Dấu nháy kép |
    | `\\` | `\` | Dấu xuộc |
    | `\n` | | Xuống dòng |

    => VD trên nên viết thành :
    ```js
    var x = "We are the so-called \"Vikings\" from the north.";
    ```
> Có thể sử dụng dấu `\` để xuống dòng 1 chuỗi string dài :
```js
document.getElementById("demo").innerHTML = "Hello \
Dolly!";
```
hoặc an toàn nhất là :
```js
document.getElementById("demo").innerHTML = "Hello " +
"Dolly!";
```
## **3) String có thể trở thành object**
## **4) Các phương thức chuỗi**
- Các phương thức chuỗi giúp tiện lợi hơn khi làm việc với chuỗi .
### **4.1) Phương thức `length`**
- Phương thức `length` sẽ trả về độ dài của chuỗi .
- Cú pháp :
    ```js
    <var_name>.length
    ```
- **VD :**
    ```js
    var txt = "ABCDEFGHIJKLMNOPQRSTUVWXYZ";
    var sln = txt.length;
    ```
    - Kết quả : `sln = 26`
### **4.2) Phương thức `indexOf()`**
- Phương thức `indexOf()` trả về số thứ tự của ký tự đầu tiên trong phần string cần tìm so với string gốc .
- Cú pháp :
    ```js
    <var_name> = <main_string>.indexOf("find_string")
    ```
- **VD :**
    ```js
    var str = "Please locate where 'locate' occurs!";
    var pos = str.indexOf("locate");
    ```
    - Kết quả : `pos = 7` (chữ "`l`" đầu tiên trong chuỗi ban đầu )
### **4.3) Phương thức `search()`**
- Phương thức `search()` trả về số thứ tự của ký tự đầu tiên trong phần string cần tìm so với string gốc .
- Cú pháp :
    ```js
    <var_name> = <main_string>.search("find_string")
    ```
- **VD :**
    ```js
    var str = "Please locate where 'locate' occurs!";
    var pos = str.search("locate");
    ```
    - Kết quả : `pos = 7` (chữ "`l`" đầu tiên trong chuỗi ban đầu )
> Khác biệt giữa `search()` và `indexOf()` :
### **4.4) Phương thức `slice()`**
- Phương thức `slice()` sẽ tách lấy một phần chuỗi và trả về phần được tách đó .
- Phương thức `slice()` sẽ nhận vào 2 tham số : vị trí bắt đầu và vị trí kết thúc ( sẽ không tính điểm cuối )
- **JavaScript** sẽ đếm vị trí các phần tử trong chuỗi bắt đầu từ `0` .
- Cú pháp :
    ```js
    <var_name> = <main_string>.slice(start, end)
    ```
    - Kết quả : `var_name = "start....(end-1)"`
- **VD :** 
    ```js
    var str = "Apple, Banana, Kiwi";
    var res = str.slice(7, 13);
    ```
    => Kết quả : `res = "Banana"`
- Nếu tham số đưa vào là số âm , chuỗi sẽ đếm ngược từ cuối lên :
    ```js
    var res = str.slice(-12, -6);
    ```
    => Kết quả : `res = "Banana"`
- Nếu bỏ qua tham số thứ 2, phương thức `slice()` sẽ cắt chuỗi từ điểm start đến cuối chuỗi :
    ```js
    var res = str.slice(7);
    ```
    => Kết quả : `res = "Banana, Kiwi"`
### **4.5) Phương thức `substring()`**
- Phương thức `substring()` tương tự như phương thức `slice()` .
- Điểm khác biệt là phương thức `substring()` không hỗ trợ truyền tham số âm .
- Cú pháp :
    ```js
    <var_name> = <main_string>.substring(start, end)
    ```
    - Kết quả : `var_name = "start....(end-1)"`
- **VD :**
    ```js
    var str = "Apple, Banana, Kiwi";
    var res = str.substring(7, 13);
    ```
    => Kết quả : `res = "Banana"`
### **4.6) Phương thức `substr()`**
- Phương thức `substr()` tương tự như phương thức `slice()` .
- Điểm khác biệt là tham số thứ 2 phương thức `substr()` sẽ là độ dài chuỗi muốn cắt bắt đầu từ tham số thứ nhất .
- Cú pháp :
    ```js
    <var_name> = <main_string>.substr(start, length)
    ```
    - Kết quả : `var_name = "start....(start + length)"`
- **VD :**
    ```js
    var str = "Apple, Banana, Kiwi";
    var res = str.substr(7, 6);
    ```
    => Kết quả : `res = "Banana"`
- Nếu bỏ qua tham số thứ 2, phương thức `substr()` sẽ cắt chuỗi từ điểm start đến cuối chuỗi :
    ```js
    var str = "Apple, Banana, Kiwi";
    var res = str.substr(7);
    ```
    => Kết quả : `res = "Banana, Kiwi"`
- Nếu đưa vào chỉ 1 tham số âm , phương thức `substr()` sẽ cắt chuỗi tính từ cuối đến điểm cần cắt :
    ```js
    var str = "Apple, Banana, Kiwi";
    var res = str.substr(-4);
    ```
    => Kết quả : `res = "Kiwi"`
### **4.7) Phương thức `replace()`**
- Phương thức `replace()` sẽ thay thế một chuỗi trong chuỗi ban đầu bằng một chuỗi khác cho trước .
- Cú pháp :
    ```js
    <var_name> = <main_string>.replace(part_str, replace_str)
    ```
- **VD :**
    ```js
    var str = "Please visit Microsoft!";
    var n = str.replace("Microsoft", "Intel");
    ```
    => Kết quả : `str = "Please visit Intel!"`
- Mặc định, phương thức `replace()` chỉ tìm và thay thế chuỗi thỏa mãn đầu tiên nó tìm được :
    ```js
    var str = "Please visit Microsoft and Microsoft!";
    var n = str.replace("Microsoft", "Intel");
    ```
    => Kết quả : `str = "Please visit Intel and Microsoft!"`
- Để khắc phục điều này , lồng phần chuỗi cần tìm trong cờ `/g` ( `global match` ) :
    ```js
    str = "Please visit Microsoft and Microsoft!";
    var n = str.replace(/Microsoft/g, "W3Schools");
    ```
    => Kết quả : `str = "Please visit Intel and Intel!"`
- Mặc định, phương thức `replace()` chỉ tìm và thay thế chuỗi chuẩn theo từng ký tự , phân biệt chữ thường và chữ in hoa . Để khắc phục điều này , lồng phần chuỗi cần tìm trong cờ `/i` ( `insensitive` ) .
    ```js
    str = "Please visit Microsoft!";
    var n = str.replace(/MICROSOFT/i, "Intel");
    ```
    => Kết quả : `str = "Please visit Intel!"`
### **4.8) Phương thức `toUpperCase()` và `toLowerCase()`**
- Phương thức `toUpperCase()` sử dụng để convert một đoạn string bất kỳ thành đoạn chữ in hoa .
- **VD :**
    ```js
    var text1 = "Hello World!";       // String
    var text2 = text1.toUpperCase();  // text2 is text1 converted to upper
    ```
    => Kết quả : `text2 = "HELLO WORLD!"`
- Phương thức `toLowerCase()` sử dụng để convert một đoạn string bất kỳ thành đoạn chữ thường .
- **VD :**
    ```js
    var text1 = "Hello World!";       // String
    var text2 = text1.toLowerCase();  // text2 is text1 converted to lower
    ```
    => Kết quả : `text2 = "hello world!"`
### **4.9) Phương thức `concat()`**
- Phương thức `concat()` dùng để join hai hoặc nhiều chuỗi với nhau .
- Sử dụng thay cho việc cộng chuỗi .
- **VD :**
    ```js
    var text1 = "Hello";
    var text2 = "World";
    var text3 = text1.concat(" ", text2);
    ```
    => Kết quả : `text3 = "Hello World!"`
### **4.10) Phương thức `trim()`**
- Phương thức `trim()` sẽ xóa bỏ các khoảng trống (`space`) thừa ở đầu và cuối chuỗi .
- **VD :**
    ```js
    var str = "       Hello World!        ";
    var res = str.trim();
    ```
    => Kết quả : `res = "Hello World!"`
### **4.11) Phương thức `charAt()`**
- Phương thức `charAt()` trả về ký tự tại vị trí cho trước trong chuỗi cho trước .
- **VD :**
    ```js
    var str = "HELLO WORLD";
    var res = str.charAt(0);
    ```
    => Kết quả : `res = "H"`
### **4.12) Phương thức `charCodeAt()`**
- Phương thức `charCodeAt()` trả về ký tự được quy đổi ra mã Unicode tại vị trí cho trước trong chuỗi cho trước .
- Phương thức sẽ trả về 1 giá trị trong bộ mã **UTF-16** ( từ `0 - 65535` )
- **VD :**
    ```js
    var str = "HELLO WORLD";
    var res = str.charCodeAt(0);
    ```
    => Kết quả : `res = 72`
### **4.13) Phương thức `split()`**
- Phương thức `split()` sẽ convert một chuỗi thành một mảng ( **array** )
- Khi được chuyển thành mảng, ta có thể lấy từng giá trị của mảng ra bằng cách sử dụng **property access** :
    ```js
    a[0], a[1], a[2],.......
    ```
- **VD :**
    ```js
    var txt = "a,b,c,d,e";
    var arr = txt.split(',')
    ```
    => Kết quả : `arr[0] = a , arr[1] = b,.....`
