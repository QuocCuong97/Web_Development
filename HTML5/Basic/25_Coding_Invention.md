# HTML5 Style Guide and Coding Conventions
### **1) Sử dụng đúng `DOCTYPE!`**
- Luôn khai báo `DOCTYPE!` ở dòng đầu tiên trong đoạn code .
    ```html
    <!DOCTYPE html>
    ```
### **2) Sử dụng chữ thường cho tên phần tử HTML**
- **HTML5** không phân biệt chữ hoa – chữ thường cho tên các phần tử. 
- Khuyến nghị sử dụng chữ thường cho tên các phần tử, vì:
    - Kết hợp cả chữ hoa và chữ thường sẽ không đẹp mắt, nhiều khi dẫn tới rối mắt trong lúc code .
    - Sử dụng chữ viết thường gần giống chuẩn XHTML hơn.
    - Viết thường nhìn đoạn code mạch lạc, rõ ràng hơn.
    - Viết chữ thường nhanh hơn.
- **VD :**
    - Không nên :
        ```html
        <SECTION>
          <p>This is a paragraph.</p>
        </SECTION>
        ```
    - Cực kỳ không nên :
        ```html
        <Section>
          <p>This is a paragraph.</p>
        </SECTION>
        ```
    - Nên :
        ```html
        <section>
          <p>This is a paragraph.</p>
        </section>
        ```
### **3) Luôn nhớ đóng thẻ cho tất cả các phần tử HTML**
- Trong **HTML5** , không nhất thiết sử dụng thẻ đóng cho tất cả các phần tử ( **VD :** thẻ `<p>` )
- Nhưng để code chuẩn, nên sử dụng thẻ đóng cho các phần tử .
- **VD :**
    - Không nên :
        ```html
        <section>
          <p>This is a paragraph.
          <p>This is a paragraph.
        </section>
        ```
    - Nên :
        ```html
        <section>
          <p>This is a paragraph.</p>
          <p>This is a paragraph.</p>
        </section>
        ```

