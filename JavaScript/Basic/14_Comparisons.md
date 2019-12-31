# Comparisons
## **1) Các toán tử so sánh**
- Các toán tử so sánh được sử dụng trong các mệnh đề logic để quyết định xem các biến hoặc các giá trị bằng nhau hay khác nhau .
- Bảng các toán tử so sánh :

    | Toán tử | Mô tả | So sánh<br>(`với x = 5`) | Returns |
    |---------|-------|----------------------|---------|
    | `==` | bằng | `x == 8`<br>`x == 5`<br>`x == "5"` | `false`<br>`true`<br>`true` |
    | `===` | bằng cả về giá trị và type | `x === 5`<br>`x === "5"` | `true`<br>`false` |
    | `!=` | không bằng | `x != 8` | `true` |
    | `!==` | khác giá trị hoặc khác type | `x !== 5`<br>`x !== "5"`<br>`x !== 8` | `false`<br>`true`<br>`true` |
    | `>` | lớn hơn | `x > 8` | `false` |
    | `<` | nhỏ hơn | `x < 8` | `true` |
    | `>=` | lớn hơn hoặc bằng | `x >= 8` | `false` |
    | `<=` | nhỏ hơn hoặc bằng | `x <= 8` | `true` |
- Các toán tử so sánh có thể được sử dụng trong các biểu thức điều kiện để xét các điều kiện :
    ```js
    if (age < 18) text = "Too young";
    ```
## **2) Các toán tử logic**
- Các toán tử logic được sử dụng để xét sự logic giữa 2 biến hoặc 2 giá trị .
- Bảng các toán tử logic :
    
    | Toán tử | Mô tả | VD (`với x = 6, y = 3`) |
    |---------|-------|-------------------------|
    | `&&` | and | `(x < 10 && y > 1) is true` |
    | `||` | or | `(x == 5 || y == 5) is false` |
    | `!` | not | `!(x == y) is true` |
## **3) Toán tử điều kiện**
- **JavaScript** cũng có 1 toán tử điều kiện sẽ gán giá trị vào biến phụ thuộc vào condition .
    ```js
    variablename = (condition) ? value1:value2 
    ```
- **VD :**
    ```js
    function myFunction() {
      var age, voteable;
      age = document.getElementById("age").value;
      voteable = (age < 18) ? "Too young":"Old enough";
      document.getElementById("demo").innerHTML = voteable + " to vote.";
    }
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/uQ9WbkL.png>

## **4) So sánh các giá trị khác loại**
- So sán các giá trị khác loại sẽ trả về kết quả không như ý muốn .
- Khi so sánh một chuỗi với một số , **JavaScript** sẽ chuyển đổi chuỗi thành số trong quá trình so sánh . Chuỗi rỗng sẽ bị chuyển về `0` . Một chuỗi không có nội dung là số sẽ chuyển thành `NaN` -> khiến cho kết quả so sánh luôn là `false` .
- **VD :**

    | Trường hợp | Giá trị trả về |
    |------------|----------------|
    | `2 < 12` | `true` |
    | `2 < "12"` | `true` | 
    | `2 < "John"` | `false` | 
    | `2 > "John"` | `false` |
    | `2 == "John"` | `false` |
    | `"2" < "12"` | `false` |
    | `"2" > "12"` | `true` |
    | `"2" == "12"` | `false` |
    > Khi so sánh 2 chuỗi , `"2"` sẽ lớn hơn `"12"` , vì trong bảng chữ cái `1` nhỏ hơn `2`
- Để đảm bảo kết quả so sánh chính xác, các biến cần được convert về đúng loại trước khi thực hiện phép so sánh :
    ```js
    age = Number(age);
    if (isNaN(age)) {
      voteable = "Input is not a number";
    } else {
      voteable = (age < 18) ? "Too young" : "Old enough";
    }
    ```
    
