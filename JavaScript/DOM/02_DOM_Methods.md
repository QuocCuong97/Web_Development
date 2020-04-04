# DOM Methods
### **DOM Programming Interface**
- **HTML DOM** có thể được truy cập bởi **JavaScript** hoặc bất cứ ngôn ngữ lập trình nào khác .
- Trong **DOM**, tất cả các phần tử **HTML** được định nghĩa như các **object** .
- **Programming Interface** chính là các thuộc tính và các phương thức của mỗi **object** .
- **HTML DOM methods** ( phương thức ) là các hành động có thể thực hiện đối với phần tử .
- **HTML DOM properties** ( thuộc tính ) là các giá trị ( của các phần tử HTML ) mà người lập trình có thể gán hoặc thay đổi .
- **VD :** Thay đổi nội dung của phần tử `<p>` có `id="demo"` :
    ```html
    <html>
    <body>

    <p id="demo"></p>

    <script>
    document.getElementById("demo").innerHTML = "Hello World!";
    </script>

    </body>
    </html>
    ```
### **Phương thức `getElementById`**
- Cách phổ biến nhất để truy cập phần tử **HTML** là sử dụng `id` của phần tử .
### **Thuộc tính `innerHTML`**
- Cách dễ nhất để lấy nội dung của phần tử là bằng cách sử dụng thuộc tính `innerHTML` .
- Thuộc tính `innerHTML` rất hữu dụng khi lấy và thay thế nội dung của các phần tử **HTML** .