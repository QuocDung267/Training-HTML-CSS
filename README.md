# Training-HTML-CSS
Xử lý tác vụ bất đồng bộ trong TypeScript như thế nào?
Trong TypeScript, có thể sử dụng các cú pháp như Promise, async/await, và Observable (nếu dùng RxJS) để xử lý các tác vụ bất đồng bộ. Phương pháp async/await giúp viết mã dễ hiểu và tương tự như mã đồng bộ.
Sau khi build UI rồi có integrate với API không? Quá trình bạn làm việc với API (xử lý data từ BE) như thế nào?
Sau khi xây dựng UI, tôi tích hợp với API bằng cách sử dụng fetch, Axios hoặc các thư viện khác để gửi và nhận dữ liệu từ backend. Thông thường, tôi sẽ viết các hàm gọi API trong một tầng service và sử dụng async/await để xử lý phản hồi. Kết quả sau đó sẽ được hiển thị trên UI hoặc xử lý thêm trước khi hiển thị.
Có làm về RxJS không? Trình bày sự hiểu biết về Observables, subscribe, unsubscribe?
RxJS là thư viện hỗ trợ làm việc với các luồng dữ liệu bất đồng bộ. Observable là đối tượng đại diện cho các dữ liệu có thể phát sinh theo thời gian. Ta có thể sử dụng subscribe để lắng nghe giá trị mới từ Observable và unsubscribe để dừng lắng nghe khi không còn cần thiết. RxJS cung cấp nhiều toán tử giúp xử lý dữ liệu dễ dàng hơn.
Làm thế nào để bạn xử lý lỗi khi code với TypeScript? Bạn có sử dụng các công cụ nào để phát hiện và xử lý các lỗi này không? (ESLint, câu hỏi liên quan về ESLint)
Khi code với TypeScript, tôi thường dựa vào hệ thống kiểm tra kiểu tĩnh của TypeScript để phát hiện lỗi trong quá trình compile. Ngoài ra, tôi sử dụng ESLint với các rules cho TypeScript để tự động phát hiện và sửa các lỗi về cú pháp, định dạng, cũng như các vấn đề có thể dẫn đến lỗi runtime.
Có viết Unit test chưa? Tại sao nó lại quan trọng trong build app? Một số framework để viết Unit test?
Tôi đã có kinh nghiệm viết Unit test. Việc này rất quan trọng vì nó giúp đảm bảo mã hoạt động đúng như dự định, phát hiện lỗi sớm và giảm thiểu rủi ro khi refactor mã. Một số framework phổ biến để viết Unit test là Jest, Mocha, Jasmine.
Trong quá trình build feature code, làm thế nào để tối ưu code dễ maintain, scale, làm việc chung với nhiều team?
Để tối ưu code dễ bảo trì và mở rộng, tôi tuân theo các nguyên tắc như DRY (Don't Repeat Yourself), KISS (Keep It Simple, Stupid), SOLID, và viết mã module hóa. Đồng thời, tôi sử dụng các tiêu chuẩn coding và review code thường xuyên để đảm bảo tính nhất quán khi làm việc với nhiều team.
Trình bày cách mà bạn tối ưu speed, tránh leak trong quá trình build feature/project/web?
Tôi tối ưu hiệu suất bằng cách giảm thiểu số lượng yêu cầu HTTP, sử dụng lazy loading cho hình ảnh và script, nén các file tĩnh, và dùng cache hiệu quả. Tôi cũng cẩn thận trong việc quản lý bộ nhớ, tránh memory leak bằng cách hủy event listener, unsubscribe từ Observable, và quản lý các tài nguyên không còn cần thiết.
Nếu bạn xử lý một tính năng được update từ cái đã có, thêm nhiều điều kiện (khoảng 20), bạn nghĩ mình sẽ làm như thế nào?
Để xử lý một tính năng có nhiều điều kiện phức tạp, tôi sẽ chia nhỏ logic thành các hàm hoặc module riêng biệt, sau đó sử dụng các cấu trúc như switch-case hoặc strategy pattern để quản lý các điều kiện một cách rõ ràng và dễ bảo trì. Điều này giúp mã dễ đọc, dễ kiểm thử và giảm thiểu lỗi.
