# Modal
## **1) Cơ bản về Modal**
- **Modal** là một hộp thoại - hay nói đúng hơn là 1 của sổ popup mà khi hiển thị sẽ nổi hẳn lên trên trang web đang hiển thị .
- **Modal** có thể chứa đựng được nhiều content theo cấu trúc header - body - footer .
- **VD :**
    ```html
    <!-- Button to Open the Modal -->
    <button type="button" class="btn btn-primary" data-toggle="modal" data-target="#myModal">
    Open modal
    </button>

    <!-- The Modal -->
    <div class="modal" id="myModal">
      <div class="modal-dialog">
        <div class="modal-content">

        <!-- Modal Header -->
          <div class="modal-header">
            <h4 class="modal-title">Modal Heading</h4>
            <button type="button" class="close" data-dismiss="modal">&times;</button>
          </div>

        <!-- Modal body -->
          <div class="modal-body">
            Modal body..
          </div>

        <!-- Modal footer -->
          <div class="modal-footer">
            <button type="button" class="btn btn-danger" data-dismiss="modal">Close</button>
          </div>

        </div>
      </div>
    </div>
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/v2IqS1M.png>

## **2) Thêm hiệu ứng cho Modal**
- Sử dụng class "`.fade`" để thêm hiệu ứng fading khi đóng/mở **modal** .
    ```html
    <!-- Fading modal -->
    <div class="modal fade"></div>

    <!-- Modal without animation -->
    <div class="modal"></div>
    ```
## **3) Kích cỡ của Modal**
- Mặc định, **modal** ở kích cỡ medium .
- Thay đổi kích cỡ của **modal** bằng cách sử dụng các class :
    - "`.modal-sm`" : modal nhỏ 
    - "`.modal-lg`" : modal lớn hơn
    - "`.modal-xl`" : modal cực lớn
- Thêm các class này vào phần tử `<div>` chứa class "`.modal-dialog`"
    - **VD1 :**
        ```html
        <div class="modal-dialog modal-sm">
        ```
        - Hiển thị trên trình duyệt :

            <img src=https://i.imgur.com/iNSu3UB.png>

    - **VD2 :**
        ```html
        <div class="modal-dialog modal-lg">
        ```
        - Hiển thị trên trình duyệt :

            <img src=https://i.imgur.com/9xd8kRA.png>

    - **VD3 :**
        ```html
        <div class="modal-dialog modal-xl">
        ```
        - Hiển thị trên trình duyệt :

            <img src=https://i.imgur.com/nT1Fd8U.png>

## **4) Căn chỉnh giữa cho Modal**
- Sử dụng class "`.modal-dialog-centered`" để căn chỉnh giữa cả theo hướng dọc và hướng ngang .
    ```html
    <div class="modal-dialog modal-dialog-centered">
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/uDDbDdY.png>

## **5) Scrolling Modal**
- Khi trong modal có quá nhiều nội dung và cần cuộn xuống để đọc, thanh scrollbar của page sẽ được sử dụng để cuộn nội dung xuống .
    
    <img src=https://i.imgur.com/wgEAlKY.png>

- Tuy nhiên để có thể sử dụng thanh cuộn bên trong modal mà không cần cuộn cả trang web, sử dụng class "`.modal-dialog-scrollable`" :
    ```html
    <div class="modal-dialog modal-dialog-scrollable">
    ```
    - Hiển thị trên trình duyệt :

        <img src=https://i.imgur.com/IY8qFwG.png>

