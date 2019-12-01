# Các phần tử Form
## **1) Phần tử `<input>`**
- Phần tử form quan trọng nhất là phần tử `<input>` .
- Phần tử `<input>` có thể hiển thị theo nhiều cách , phụ thuộc vào các thuộc tính của nó .
- **VD :**
    ```html
    <input name="firstname" type="text">
    ```
- Nếu thuộc tính `type` bị bỏ sót , mặc định sẽ là `text` input .
## **2) Phần tử `<select>`**
- Phần tử `<select>` định nghĩa một list drop-down .
- **VD :**
    ```html
    <select name="cars">
      <option value="volvo">Volvo</option>
      <option value="saab">Saab</option>
      <option value="fiat">Fiat</option>
      <option value="audi">Audi</option>
    </select>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/cMcVjoY.png>

- Phần tử `<option>` định nghĩa mỗi option được chọn trong list .
- Mặc định , phần tử đầu tiên trong list sẽ được chọn ( được bôi xanh lúc đầu )
- Để định nghĩa option được chọn trước , thêm thuộc tính `selected` vào phần tử `<option>` .
    ```html
    <option value="fiat" selected>Fiat</option>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/2H09rWb.png>

- Sử dụng thuộc tính `size` để định nghĩa số dòng option có thể thấy được , list sẽ trở thành dạng cuộn :
    ```html
    <select name="cars" size="3">
      <option value="volvo">Volvo</option>
      <option value="saab">Saab</option>
      <option value="fiat">Fiat</option>
      <option value="audi">Audi</option>
    </select>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/FPU406m.png>

- Sử dụng thuộc tính `multiple` để định nghĩa số dòng option user có thể chọn được ( mặc định là `1` ) :
    ```html
    <select name="cars" size="4" multiple>
      <option value="volvo">Volvo</option>
      <option value="saab">Saab</option>
      <option value="fiat">Fiat</option>
      <option value="audi">Audi</option>
    </select>
    ```
    - Hiển thị trên trình duyệt :
        
        <img src=https://i.imgur.com/G1axwBR.png>

## **3) Phần tử `<textarea>`**
- Phần tử `<textarea>` định nghĩa trường input nhiều dòng (mặc định là 1 dòng) .
- **VD :**
    ```html
    <textarea name="message" rows="10" cols="30">
    The cat was playing in the garden.
    </textarea>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/Gvlmh8r.png>

- Thuộc tính `rows` chỉ ra số dòng có thể nhìn thấy ở trường input(số dòng có thể nhìn thấy tối đa mà không cần dùng thanh scrollbar)
- Thuộc tính `cols` chỉ ra chiều ngang (số ký tự chiều ngang) có thể nhìn thấy của trường input .
- Cũng có thể định nghĩa kích cỡ của trường input bằng cách sử dụng **CSS** :
    ```html
    <textarea name="message" style="width:200px; height:600px;">
    The cat was playing in the garden.
    </textarea>
    ```
## **4) Phần tử `<button>`**
- Phần tử `<button>` định nghĩa một nút có thể click được .
- **VD :**
    ```html
    <button type="button" onclick="alert('Hello World!')">Click Me!</button>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/UgvPasU.png>

## **5) Các phần tử form mới trong HTML5**
- Phiên bản **HTML5** bổ sung các phần tử form sau :
    - `<datalist>`
    - `<output>`
### **5.1) Phần tử `<datalist>`**
- Phần tử `<datalist>` định nghĩa 1 danh sách các option cho phần tử `<input>` .
- Người dùng sẽ thấy 1 dạng list drop-down các option bên trên và sau khi chọn option nào thì đó sẽ là input text .
- Thuộc tính `list` của phần tử `<input>` liên quan đến thuộc tính `<id>` của phần tử `<datalist>` .
- **VD :**
    ```html
    <form action="/action_page.php">
      <input list="browsers">
      <datalist id="browsers">
        <option value="Internet Explorer">
        <option value="Firefox">
        <option value="Chrome">
        <option value="Opera">
        <option value="Safari">
      </datalist>
    </form>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/sQWXarV.png>

### **5.2) Phần tử `<output>`**
- Phần tử `<output>` đại diện cho 1 kết quả sau một quá trình xử lý (ví dụ như kết quả sau khi thực hiện một script) .<br>
[Tham khảo thêm](https://www.w3schools.com/html/html_form_elements.asp)