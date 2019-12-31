# Break và Continue
## **1) `break`**
- `break` thường sử dụng để thoát ra khỏi cấu trúc `switch...case`
- `break` cũng được sử dụng để thoát khỏi vòng lặp , sau đó thực hiện tiếp các đoạn code đằng sau .
- **VD :**
    ```js
    for (i = 0; i < 10; i++) {
    if (i === 3) { break; }
      text += "The number is " + i + "<br>";
    }
    ```
    => Kết quả :
    ```
    The number is 0
    The number is 1
    The number is 2
    ```
## **2) `continue`**
- `continue` sẽ bỏ qua 1 bước trong vòng lặp , và nếu condition còn `true`, chương trình sẽ chạy tiếp vòng lặp .
- **VD :**
    ```js
    for (i = 0; i < 10; i++) {
    if (i === 3) { continue; }
      text += "The number is " + i + "<br>";
    }
    ```
    => Kết quả :
    ```
    The number is 0
    The number is 1
    The number is 2
    The number is 4
    The number is 5
    The number is 6
    The number is 7
    The number is 8
    The number is 9
    ```
## **3) Labels**
- Để đánh nhãn một mệnh đề **JavaScript** , đặt label ( nhãn ) trước mệnh đề với một dấu "`:`"
    ```js
    label:
    statements
    ```
- Mệnh đề `break` và `continue` là các mệnh đề duy nhất trong **JavaScript** giúp thoát khỏi các code block .
    ```js
    break labelname;
	continue labelname;
	```
- Mệnh đề `continue` ( không đi kèm label ) chỉ có thể được sử dụng để bỏ qua 1 bước trong vòng lặp .
- Mệnh đề `break` ( không đi kèm label ) chỉ có thể được sử dụng để thoát khỏi vòng lặp hoặc `switch...case` .
- Sau khi thêm label , mệnh đề `break` có thể được sử dụng để thoát ra bất cứ khối code block nào .
- **VD :**
	```js
	var cars = ["BMW", "Volvo", "Saab", "Ford"];
	list: {
	  text += cars[0] + "<br>";
	  text += cars[1] + "<br>";
	  break list;
	  text += cars[2] + "<br>";
	  text += cars[3] + "<br>";
	}
	document.getElementById("demo").innerHTML = text;
	```
	=> Kết quả :
	```
	BMW
	Volvo
	```
	> **Code block** phải được khai báo trong cặp dấu `{}` .
	