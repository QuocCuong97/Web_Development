# Math Object
- **Math object** trong **JavaScript** cho phép biểu diễn kết quả các công thức toán học dưới dạng số .
### **1) Các hằng số**
- **JavaScript** cung cấp `8` hằng số toán học có thể được gọi ra bằng **math object** :
    ```js
    Math.PI;      // returns 3.141592653589793
    Math.E        // returns số e
    Math.SQRT2    // returns căn bậc 2 của 2
    Math.SQRT1_2  // returns căn bậc 2 của 1/2
    Math.LN2      // returns ln2
    Math.LN10     // returns ln10
    Math.LOG2E    // returns log2(e)
    Math.LOG10E   // returns log(e)
    ```
### **2) Hàm `Math.round()`**
- Công thức `Math.round(x)` trả về giá trị `x` được làm tròn đến số nguyên gần nhất :
    ```js
    Math.round(4.7);    // returns 5
    Math.round(4.4);    // returns 4
    ```
### **3) Hàm `Math.pow()`**
- Công thức `Math.pow(x, y)` trả về giá trị `x` sau khi được lũy thừa với số mũ `y` :
    ```js
    Math.pow(8, 2);      // returns 64
    ```
### **4) Hàm `Math.sqrt()`**
- Công thức `Math.sqrt(x)` trả về giá trị căn bậc 2 của `x` :
    ```js
    Math.sqrt(64);      // returns 8
    ```
### **5) Hàm `Math.abs()`**
- Công thức `Math.abs(x)` trả về trị tuyệt đối của `x` :
    ```js
    Math.abs(-4.7);     // returns 4.7
    ```
### **6) Hàm `Math.ceil()`**
- Công thức `Math.ceil(x)` trả về giá trị `x` sau khi được làm tròn lên đến số nguyên gần nhất :
    ```js
    Math.ceil(4.4);     // returns 5
    ```
### **7) Hàm `Math.floor()`**
- Công thức `Math.floor(x)` trả về giá trị `x` sau khi được làm tròn xuống đến số nguyên gần nhất :
    ```js
    Math.floor(4.7);    // returns 4
    ```
### **8) Hàm `Math.sin()`**
- Công thức `Math.sin(x)` trả về giá trị `sin` của góc `x` ( <code>-1 &le; sinx &le; -1</code> ) - đơn vị của `x` ra `rad` .
- Có thể quy đổi `x` sang `deg` thay vì dùng `rad` bằng công thức :
    ```
    x-rad = x-deg * PI/180
    ```
- **VD :**
    ```js
    Math.sin(90 * Math.PI / 180);     // returns 1
    ```
### **9) Hàm `Math.cos()`**
- Công thức `Math.cos(x)` trả về giá trị `cos` của góc `x` ( <code>-1 &le; sinx &le; -1</code> ) - đơn vị của `x` ra `rad` .
- Có thể quy đổi `x` sang `deg` thay vì dùng `rad` bằng công thức :
    ```
    x-rad = x-deg * PI/180
    ```
- **VD :**
    ```js
    Math.cos(0 * Math.PI / 180);     // returns 1
    ```
### **10) Hàm `Math.min()` và `Math.max()`**
- Công thức `Math.min()` và `Math.max()` có thể được sử dụng để tìm giá trị nhỏ nhất hoặc lớn nhất của 1 list các tham số :
    ```js
    Math.min(0, 150, 30, 20, -8, -200);  // returns -200
    Math.max(0, 150, 30, 20, -8, -200);  // returns 150
    ```
### **11) Hàm `Math.random()`**
- Hàm `Math.random()` trả về 1 số ngẫu nhiên trong khoảng từ `0` đến `1` :  
    ```js
    Math.random();    // returns 0.6931053313565989 (random)