# Biểu thức và toán tử
## **1) Các biểu thức toán học**
| Toán tử | Mô tả |
|---------|-------|
| `+` | Cộng |
| `-` | Trừ |
| `*` | Nhân |
| `**` | Lũy thừa |
| `/` | Chia |
| `%` | Chia (lấy phần dư) |
| `++` | Tăng dần |
| `--` | Giảm dần |
- **VD :**
    - **Cộng** :
        ```js
        var x = 5;
        var y = 2;
        var z = x + y;
        ```
        - Kết quả : `z = 7`
    - **Trừ** :
        ```js
        var x = 5;
        var y = 2;
        var z = x - y;
        ```
        - Kết quả : `z = 3`
    - **Nhân** :
        ```js
        var x = 5;
        var y = 2;
        var z = x * y;
        ```
        - Kết quả : `z = 10`
    - **Lũy thừa** :
        ```js
        var x = 5;
        var z = x ** 2;
        ```
        - Kết quả : `z = 25`
    - **Chia** :
        ```js
        var x = 5;
        var y = 2;
        var z = x / y;
        ```
        - Kết quả : `z = 2.5`
    - **Chia lấy phần dư** :
        ```js
        var x = 5;
        var y = 2;
        var z = x % y;
        ```
        - Kết quả : `z = 2`
    - **Tăng dần** :
        ```js
        var x = 5;
        x++;
        var z = x;
        ```
        - Kết quả : `z = 6`
    - **Giảm dần** :
        ```js
        var x = 5;
        x--;
        var z = x;
        ```
        - Kết quả : `z = 4`
    - **Biểu thức chứa nhiều toán tử** :
        ```js
        var x = 100 + 50 * 3;
        ```
        - Kết quả : `x = 250`

## **2) Các biểu thức gán**

| Toán tử | Ví dụ | Tương đương với |
|---------|-------|-----------------|
| `=` | x = y | x = y |
| `+=` | x += y | x = x + y |
| `-=` | x -= y | x = x - y |
| `*=` | x *= y | x = x * y |
| `/=` | x /= y | x = x / y |
| `%=` | x %= y | x = x % y |
| `**=` | x **= y | x = x ** y |

- **VD :**
    - Toán tử `=` :
        ```js
        var x = 10;
        ```
    - Toán tử `+=` :
        ```js
        var x = 10;
        x += 5;
        ```
        - Kết quả : `x = 15`
    - Toán tử `-=` :
        ```js
        var x = 10;
        x -= 5;
        ```
        - Kết quả : `x = 5`
    - Toán tử `*=` :
        ```js
        var x = 10;
        x *= 5;
        ```
        - Kết quả : `x = 50`
    - Toán tử `/=` :
        ```js
        var x = 10;
        x /= 5;
        ```
        - Kết quả : `x = 2`
    - Toán tử `%=` :
        ```js
        var x = 10;
        x %= 5;
        ```
        - Kết quả : `x = 0`

## **3) Các toán tử so sánh**

| Toán tử | Mô tả |
|---------|-------|
| `==` | bằng |
| `===` | bằng về cả giá trị và loại (type) |
| `!=` | không bằng |
| `!==` | khác giá trị hoặc khác loại (type) |
| `>` | lớn hơn |
| `<` | nhỏ hơn |
| `>=` | lớn hơn hoặc bằng |
| `<=` | nhỏ hơn hoặc bằng |
| `?` | toán tử điều kiện |

## **4) Các toán tử logic**

| Toán tử | Mô tả |
|---------|-------|
| `&&` | and |
| `||` | or |
| `!` | not |

## **5) Các toán tử phân loại**

| Toán tử | Mô tả |
|---------|-------|
| `typeof` | Trả về loại (type) của biến |
| `instanceof` | Returns true if an object is an instance of an object type |