# Phần tử Block và Inline
- Tất cả các phần tử HTML đều có giá trị hiển thị mặc định tuy vào loại phần tử .
- 2 giá trị hiển thị là : **block** và **inline** .
## **1) Block**
- 1 **khối block** luôn bắt đầu bằng 1 dòng mới và sẽ chiếm toàn bộ chiều rộng có thể hiển thị ( co dãn từ trái sang phải tùy vào trình duyệt )
- Các thẻ hiển thị **khối block** :
    ```html
    <address>    <article>   <aside>   <blockquote>   <canvas>
    <dd>         <div>       <dl>      <dt>           <fieldset>
    <figcaption> <figure>    <footer>  <form>         <h1>  <h6>
    <header>     <hr>        <li>      <main>         <nav>
    <noscript>   <ol>        <p>       <pre>          <section>
    <table>      <tfoot>     <ul>      <video>
    ```
## **Thẻ `<div>`**
- Phần tử `<div>` là một trong các thẻ biểu thị một **khối block** .
- **VD1 :**
    ```html
    <div>Hello World!</div>
    <div>Hello World!</div>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/9HWpjtv.png>
- Phần tử `<div>` thường được sử dụng như 1 container chứa các phần tử khác .
- Phần tử `<div>` không bắt buộc các thuộc tính đi kèm , tuy nhiên có các thuộc tính thường được sử dụng kèm là `style`, `class`, `id` .
- Khi được sử dụng cùng với **CSS** , phần tử `<div>` có thể được sử dụng như một khối nội dung có style riêng biệt .
- **VD2 :**
    ```html
    <div style="background-color:black;color:white;padding:20px;">
    <h2>London</h2>
    <p>London is the capital city of England. It is the most populous city in the United Kingdom, with a metropolitan area of over 13 million inhabitants.</p>
    </div>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/6tKyH4v.png>
## **2) Inline**
- Phần tử **inline** sẽ không bắt đầu 1 dòng mới mà chỉ chiếm phần chiều rộng cần thiết của nó trên dòng .
- Các thẻ hiển thị **inline** :
    ```html
    <a>       <abbr>    <acronym>   <b>      <bdo>    <big>
    <br>      <button>  <cite>      <code>   <dfn>    <em>
    <i>       <img>     <input>     <kbd>    <label>  <map>
    <object>  <output>  <q>         <samp>   <script> <select>
    <small>   <span>    <strong>    <sub>    <sup>    <textarea>
    <time>    <tt>      <var>
    ```
## **Thẻ `<span>`**
- Thẻ `<span>` là một ví dụ điển hình của phần tử **inline** .
- **VD1 :**
    ```html
    <span>Hello World</span>
    <span>Hello World</span>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/GhZDUnY.png>
- Phân tử `<span>` thường được sử dụng như một container chứa các đoạn text .
- Phần tử `<span>` không bắt buộc các thuộc tính đi kèm , tuy nhiên có các thuộc tính thường được sử dụng kèm là `style`, `class`, `id` .
- Khi được sử dụng cùng với **CSS** , phần tử `<div>` có thể được sử dụng như một khối text có style riêng biệt .
- **VD2 :** 
    ```html
    <h1>My <span style="color:red">Important</span> Heading</h1>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/U4aLpUo.png>