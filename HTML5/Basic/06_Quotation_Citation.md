# Trích dẫn trong HTML
## **1) Phần tử `<q>`**
- Phần tử `<q>` định nghĩa đoạn chú thích ngắn .
- Trình duyệt thường thêm dấu chú thích ( dấu `""` ) quanh nội dung chú thích .
- **VD :**
    ```html
    <p>WWF's goal is to: <q>Build a future where people live in harmony with nature.</q></p>
    ```
    - Hiển thị trên trình duyệt :
        
        <img src=https://i.imgur.com/jzmztn9.png>

## **2) Phần tử `<blockquote>`**
- Phần tử `<blockquote>` định nghĩa 1 đoạn chú thích ( của 1 nguồn khác )
- Trình duyệt sẽ tự động thụt dòng cho phần tử `<blockquote>` .
- **VD :**
    ```html
    <p>Here is a quote from WWF's website:</p>
    <blockquote cite="http://www.worldwildlife.org/who/index.html">
    For 50 years, WWF has been protecting the future of nature.
    The world's leading conservation organization,
    WWF works in 100 countries and is supported by
    1.2 million members in the United States and
    close to 5 million globally.
    </blockquote>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/xsyUWFK.png>

## **3) Phần tử `<abbr>`**
- Phần tử `<abbr>` định nghĩa một từ viết tắt .
- Sử dụng phần tử `<abbr>` có thể cung cấp thông tin hữu ích cho trình duyệt, các hệ thống dịch ngôn ngữ và các công cụ tìm kiếm .
- **VD :**
    ```html
    <p>The <abbr title="World Health Organization">WHO</abbr> was founded in 1948.</p>
    ```
    - Hiển thị trong trình duyệt :

        <img src=https://i.imgur.com/do8j7Fs.png>

## **4) Phần tử `<address>`**
- Phần tử `<address>` định nghĩa thông tin liên lạc ( tác giả/chủ sở hữu ) của văn bản hoặc 1 bài báo .
- Phần tử `<address>` luôn được hiển thị dưới dạng *in nghiêng* . Hầu hết các trình duyệt sẽ thêm 1 dòng trống trước và sau phần tử .
- **VD :**
    ```html
    <address>
    Written by John Doe.<br>
    Visit us at:<br>
    Example.com<br>
    Box 564, Disneyland<br>
    USA
    </address>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/mrZApdV.png>
## **5) Phần tử `<cite>`**
- Phần tử `<cite>` định nghĩa tiêu đề , chú thích cho 1 thực thể cụ thể nào đó ( như hình ảnh....)
- Trình duyệt sẽ hiển thị phần tử `<cite>` dưới dạng *in nghiêng* .
- **VD :**
    ```html
    <img src="img_the_scream.jpg" width="220" height="277" alt="The Scream">
    <p><cite>The Scream</cite> by Edvard Munch. Painted in 1893.</p>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/FrcLm0Y.png>

## **6) Phần tử `<bdo>`**
- Phần tử `<bdo>` định nghĩa 1 đoạn chữ viết ngược .
- **VD :**
    ```html
    <bdo dir="rtl">This text will be written from right to left</bdo>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/oCCDGoT.png>