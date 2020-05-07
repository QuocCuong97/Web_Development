# Tổng quan về API
## **1) Giới thiệu về API**
- **API - *Application Programming Interface*** là một phần mềm cho phép truy cập dữ liệu hoặc dịch vụ giữa các ứng dụng khác nhau. Đó là một tập hợp các quy tắc mô tả cách thức một ứng dụng tương tác với một ứng dụng khác và các hướng dẫn để cho phép tương tác này xảy ra . Người sử dụng gửi yêu cầu truy cập API request đến máy chủ để yêu cầu thông tin và nhận được trả lời API response từ server cùng với thông tin được yêu cầu .

    <img src=https://i.imgur.com/1aX4M7l.png>
## **2) Phân loại API**
### **2.1) Phân loại theo nền tảng**
- **API trên nền tảng web**: API trên nền tảng web hay còn gọi là web API. Loại này hiện đang được sử dụng phổ biến trong lập trình web hiện nay. Những website lớn như ***Facebook***, ***Google*** đều cung cấp hệ thống API cho phép bạn kết nối, lấy dữ liệu hoặc cập nhật dữ liệu vào hệ thống. Đại đa số các API trên nền tảng web được thiết kế theo tiêu chuẩn **RESTful**. Dữ liệu trả về thường có định dạng dữ liệu là **JSON**, **XML** hoặc một kiểu dữ liệu bất kì .
- **API trên hệ điều hành**: Khái niệm này còn có trước cả API trên nền tảng web. Microsoft cung cấp các hệ điều hành Windows cùng các tài liệu API là đặc tả các hàm, phương thức, lời gọi hàm cũng như các giao thức kết nối cho lập trình viên. Giúp cho các lập trình viên có thể tạo ra các phần mềm ứng dụng có thể tương tác trực tiếp với hệ điều hành.
- **API của thư viện phần mềm hay framework**: Mô tả và quy định các hành động mong muốn mà các thư viện cung cấp. Một API có thể có nhiều cách triển khai khác nhau, giúp cho một chương trình viết bằng ngôn ngữ này có thể sử dụng thư viện được viết bằng ngôn ngữ khác. Chẳng hạn có thể dùng PHP để yêu cầu một thư viện tạo file PDF được viết bằng C++.
### **2.2) Phân loại theo quyền hạn**
- **API mở ( *open APIs/Public APIs* )** : các API này có sẵn công khai và có thể được sử dụng không bị hạn chế . Vì các API này công khai nên nhiều nhà cung cấp API yêu cầu người sử dụng nhận khóa hoặc mã thông báo trước khi sử dụng nhằm kiểm soát số lượng yêu cầu API mà họ nhận được và xử lý .
- **API nội bộ ( *internal APIs* )** : loại này còn được gọi là API riêng tư, chỉ các hệ thống nội bộ mới dùng loại này do chúng ít được biết đến và thường sử dụng trong phạm vi công ty. Chúng được sử dụng trong các đội ngũ phát triển nội bộ khác nhau để có thể cải thiện các sản phẩm và dịch vụ mình.
- **API cho đối tác ( *partner APIs* )** : đây là các API được sử dụng giữa một tổ chức hoặc công ty với đối tác để tạo thuận lợi cho việc kinh doanh giữa họ . Đối tác kinh doanh phải có giấy phép hoặc được sự cho phép để sử dụng API này .

