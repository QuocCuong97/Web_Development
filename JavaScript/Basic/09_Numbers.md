# Numbers
## **1) Kiểu dữ liệu `number`**
- Trong **JavaScript**, số là một tập hợp gồm một hoặc nhiều chữ số (`0`, `1`, `2`, `3`, `4`, `5`, `6`, `7`, `8`, `9`) và có thể chứa thêm một dấu chấm động(`.`).
    - Số không chứa dấu chấm được gọi là số nguyên . ( **VD :** `5` , `-67` , .....)
    - Số có chứa dấu chấm được gọi là số thực . ( **VD :** `45.78` , `-50.2`, ....)
- Nếu một số quá lớn hoặc quá nhỏ, có thể viết chúng dưới dạng biểu thức mũ :
    - `x = 5000000000` ( <code>5*10<sup>9</sup></code> )<br><=> `x = 5e+9`
    - `x = 0.000005` ( <code>5*10<sup>-6</sup></code> )<br><=> `x = 5e-6`
## **2) Độ chính xác của số**
- Trong **JavaScript** , một số nguyên sẽ có độ chính xác lên đến `15` chữ số . Các số nguyên quá `15` chữ số sẽ bị làm tròn theo 1 qui tắc nào đó, không còn chính xác .
    ```js
    var a = 99999999999999; //14 chữ số (nằm trong độ chính xác)
    var b = 999999999999999; //15 chữ số (nằm trong độ chính xác)
    var c = 9999999999999999; //16 chữ số (không còn chính xác)
    var d = 99999999999999999; //17 chữ số (không còn chính xác)
    ```
    => Kết quả : `c` và `d` sẽ bị làm tròn :
    ```
    a = 99999999999999
    b = 999999999999999
    c = 10000000000000000
    d = 100000000000000000
    ```
- Đối với số thực thì độ chính xác sẽ lên đến `17` chữ số .
    ```js
    var a = 0.999999999999999; //16 chữ số (nằm trong độ chính xác)
    var b = 0.9999999999999999; //17 chữ số (nằm trong độ chính xác)
    var c = 0.99999999999999999; //18 chữ số (không còn chính xác)
    var d = 0.999999999999999999; //19 chữ số (không còn chính xác)
    ```
    => Kết quả : `c` và `d` sẽ bị làm tròn :
    ```
    a = 0.999999999999999
    b = 0.9999999999999999
    c = 1
    d = 1
    ```
## **3) Số dưới dạng chuỗi**
- Số trong **JavaScript** có thể tồn tại dưới dạng chuỗi , có thể thực hiện được tất cả các phép toán .
    ```js
    var z = "100" - "10"
    ```
    => Kết quả : `z = 90` (định dạng `number`)
    ```js
    var z = "100" * "10"
    ```
    => Kết quả : `z = 1000` (định dạng `number`)
    ```js
    var z = "100" / "10"
    ```
    => Kết quả : `z = 10` (định dạng `number`)

- Tuy nhiên , phép cộng sẽ bị hiểu nhầm thành việc cộng chuỗi :
    ```js
    var z = "100" + "10"
    ```
    => Kết quả : `10010` (định dạng `string`)
## **4) `NaN` - Not a Number**
- Giá trị `NaN` ( **Not a Number** ) là một giá trị thuộc kiểu **number** , nhưng nó không phải là một số .
- Giá trị `NaN` thường được sinh ra khi phép toán có chứa toán hạng không thuộc kiểu dữ liệu **number** và toán tử trong phép toán đó là phép trừ, phép nhân, hoặc phép chia .
- **VD :**
    ```js
    vax x = 100 / "Apple"
    ```
    => Kết quả : `x = NaN`
- Nếu thực hiện phép toán bất kỳ giữa một số nào đó với giá trị `NaN` thì nó sẽ cho ra giá trị `NaN` :
    ```js
    var x = 100 + NaN
    ```
    => Kết quả : `x = NaN`
- Nếu thực hiện cộng chuỗi với giá trị `NaN` , kết quả sẽ là 1 chuỗi ghép :
    ```js
    var x = "Apple" + "NaN"
    ```
    => Kết quả : `x = AppleNaN`
- Có thể kiểm tra giá trị một biến có phải `NaN` không bằng phương thức `isNaN()` :
    ```js
    var x = 100 / "Apple"
    var y = isNaN(x)
    var z = typeof(x)
    ```
    => Kết quả :
    ```
    x = NaN
    y = True
    z = number
    ```
## **5) `Infinity` - ( `-Infinity` )**
- Giá trị `Infinity` và `-Infinity` trong **JavaScript** cũng tương tự như **dương vô cùng** ( <code>&infin;</code> ) và **âm vô cùng** ( <code>-&infin;</code> ) trong đại số :
    - Giá trị `Infinity` đại diện cho **số dương lớn nhất** ( nằm ngoài khả năng đo đếm của **JavaScript** )
    - Giá trị `-Infinity` đại diện cho **số âm lớn nhất** ( nằm ngoài khả năng đo đếm của **JavaScript** )
- `Infinity` vẫn thuộc định dạng **number** .
- **VD :**
    ```js
    var myNumber = 2;
    while (myNumber != Infinity) {   // Execute until Infinity
      myNumber = myNumber * myNumber;
    }
    ```
    => Kết quả : 
    ```
    4
    16
    256
    65536
    4294967296
    18446744073709552000
    3.402823669209385e+38
    1.157920892373162e+77
    1.3407807929942597e+154
    Infinity
    ```
- Khi chia một số với mẫu số bằng `0`, giá trị trả về cũng là `Infinity` :
    ```js
    var x =  2 / 0;
    var y = -2 / 0;
    ```
    => Kết quả :
    ```
    x = Infinity
    y = -Infinity
    ```
## **6) Hexadecimal**
## **7) Number có thể trở thành object**
## **8) Các phương thức với number**
### **8.1) Phương thức `toString()`**
- Phương thức `toString()` convert định dạng **number** thành **string** .
- **VD :**
    ```js
    var x = 123;
    x.toString();            // returns 123 from variable x
    (123).toString();        // returns 123 from literal 123
    (100 + 23).toString();   // returns 123 from expression 100 + 23
    ```
### **8.2) Phương thức `toExponential()`**
- Phương thức `toExponential()` sẽ chuyển một số nhiều chữ số thành định dạng số lũy thừa .
- Phương thức `toExponential()` cần truyền vào 1 tham số là số chữ số thập phân sau khi được chuyển đổi (tham số này là tùy chọn)
- **VD :**
    ```js
    var x = 9.656;
    x.toExponential(2);     // returns 9.66e+0
    x.toExponential(4);     // returns 9.6560e+0
    x.toExponential(6);     // returns 9.656000e+0
    ```
### **8.3) Phương thức `toFixed()`**
- Phương thức `toFixed()` trả về một chuỗi , với nội dung là số sau khi đã được làm tròn .
- Phương thức `toFixed()` sẽ nhận vào một tham số là số chữ số thập phân mong muốn .
- **VD :**
    ```js
    var x = 9.656;
    var z = x.toFixed(10);
    x.toFixed(0);           // returns 10
    x.toFixed(2);           // returns 9.66
    x.toFixed(4);           // returns 9.6560
    x.toFixed(6);           // returns 9.656000
    typeof(z);              // returns string
    ```
### **8.4) Phương thức `toPrecision()`**
- Phương thức `toPrecision()` trả về một chuỗi , với nội dung là số sau khi đã được làm tròn .
- Phương thức `toPrecision()` sẽ nhận vào một tham số là số chữ số của số được làm tròn (tính cả phần nguyên và phần thập phân) .
- **VD :**
    ```js
    var x = 9.656;
    var z = x.toPrecision(10);
    x.toPrecision();        // returns 9.656
    x.toPrecision(2);       // returns 9.7
    x.toPrecision(4);       // returns 9.656
    x.toPrecision(6);       // returns 9.65600
    typeof(z);              // returns string
    ```
### **8.5) Phương thức `Number()`**
- Phương thức `Number()` dùng để phân tích một giá trị để trả về một số tương ứng với giá trị đó .
- Nếu giá trị là một đối tượng ngày tháng thì phương thức `Number()` sẽ trả về tổng số mili giây từ `1/1/1970` đến thời điểm của đối tượng ngày tháng đó .
- Nếu không thể chuyển đổi về dạng số, phương thức sẽ trả về giá trị `NaN` .
- **VD :**
    ```js
    Number(true);          // returns 1
    Number(false);         // returns 0
    Number("10");          // returns 10
    Number("  10");        // returns 10
    Number("10  ");        // returns 10
    Number(" 10  ");       // returns 10
    Number("10.33");       // returns 10.33
    Number("10,33");       // returns NaN
    Number("10 33");       // returns NaN
    Number("John");        // returns NaN
    ```
### **8.6) Phương thức `parseInt()`**
- Phương thức `parseInt()` dùng để phân tích một chuỗi để trả về một số nguyên tương ứng .
- Nếu không thể chuyển đổi về dạng số nguyên, phương thức sẽ trả về giá trị `NaN` .
- **VD :**
    ```js
    parseInt("10");         // returns 10
    parseInt("10.33");      // returns 10
    parseInt("10 20 30");   // returns 10
    parseInt("10 years");   // returns 10
    parseInt("years 10");   // returns NaN 
    ```
### **8.7) Phương thức `parseFloat()`**
- Phương thức `parseFloat()` dùng để phân tích một chuỗi để trả về một số thực tương ứng .
- Nếu không thể chuyển đổi về dạng số thực, phương thức sẽ trả về giá trị `NaN` .
- **VD :**
    ```js
    parseFloat("10");        // returns 10
    parseFloat("10.33");     // returns 10.33
    parseFloat("10 20 30");  // returns 10
    parseFloat("10 years");  // returns 10
    parseFloat("years 10");  // returns NaN
    ```
