# Training-HTML-CSS

Dưới đây là câu trả lời cho các câu hỏi trong ảnh:

Level 1:
Sự khác biệt giữa var, let, và const là gì?
var: Có phạm vi function scope, có thể khai báo lại, bị hoisting, có thể thay đổi giá trị.
let: Có phạm vi block scope, không thể khai báo lại trong cùng một phạm vi, có thể thay đổi giá trị.
const: Cũng có phạm vi block scope, không thể thay đổi giá trị sau khi đã gán.
undefined khác gì null?
undefined là khi biến chưa được gán giá trị, còn null là giá trị được lập trình viên cố ý gán để biểu thị "rỗng" hoặc "không có gì".
this là gì?
this là từ khóa đại diện cho đối tượng mà phương thức đang được gọi, hoặc ngữ cảnh hiện tại của đoạn mã.
Hoisting trong JavaScript là gì?
Hoisting là hành vi của JavaScript tự động "nâng" các khai báo biến và hàm lên đầu phạm vi của chúng, nhưng không nâng giá trị gán.
Cách bắt sự kiện khi nhấn nút trên trang web là gì?
Sử dụng addEventListener để gắn sự kiện lắng nghe vào nút, ví dụ: button.addEventListener('click', function() {...});.
Promise là gì? Các state khác nhau trong Promise?
Promise là một đối tượng đại diện cho một tác vụ bất đồng bộ. Nó có 3 trạng thái:
pending: Đang chờ xử lý.
fulfilled: Đã hoàn thành.
rejected: Bị từ chối.
Closure trong JavaScript là gì?
Closure là hàm có thể nhớ được biến từ phạm vi bên ngoài ngay cả khi hàm đó đã thực thi xong.
Callback function là gì?
Callback function là một hàm được truyền vào hàm khác như một đối số và được gọi sau khi hàm bên ngoài hoàn thành.
Để lấy 1 thẻ bằng ID có mấy cách, nếu có thì trả về gì, không tìm ra thì trả về gì?
Có thể sử dụng document.getElementById('id'). Nếu tìm thấy, trả về phần tử DOM, nếu không tìm thấy, trả về null.
Event bubbling và event capturing là gì? xử lý như thế nào?
Event bubbling là khi sự kiện truyền từ phần tử con lên phần tử cha. Event capturing là khi sự kiện truyền từ cha xuống con. Để xử lý, có thể dùng addEventListener với tham số thứ ba để chỉ định "capturing" hoặc "bubbling".
Level 2:
Sự khác biệt giữa cookies, session storage, và local storage?
cookies: Dùng để lưu dữ liệu nhỏ, thường được gửi kèm mỗi khi trình duyệt yêu cầu từ server, có thời hạn.
sessionStorage: Lưu trữ dữ liệu trong phiên làm việc, khi đóng tab sẽ mất.
localStorage: Lưu trữ dữ liệu lâu dài, không bị mất khi đóng trình duyệt.
Arrow function khác gì so với function thường?
Arrow function không có this và arguments riêng, nó kế thừa this từ ngữ cảnh bên ngoài, và cú pháp ngắn gọn hơn.
Các giá trị falsy trong JavaScript là gì? Có cần lưu ý gì khi làm việc với giá trị falsy không?
Các giá trị falsy bao gồm: false, 0, '' (chuỗi rỗng), null, undefined, và NaN. Khi làm việc với giá trị falsy, cần cẩn thận vì các giá trị này đều được coi là "sai" khi kiểm tra trong điều kiện.
Spread operator dùng khi nào?
Spread operator (...) được dùng để mở rộng một mảng, đối tượng hoặc chuỗi thành các phần tử hoặc thuộc tính riêng lẻ. Ví dụ: sao chép mảng, gộp đối tượng.
Clone 1 object/array thì dùng những cách gì?
Có thể dùng Object.assign(), spread operator (...) hoặc JSON.parse(JSON.stringify()) để clone object/array.
Kể tên các sự kiện tương ứng với onmousedown, onmouseup, onmousemove trên touch screen?
Các sự kiện tương ứng trên màn hình cảm ứng là touchstart, touchend, và touchmove.
Khi bạn cần chờ đợi nhiều tác vụ bất đồng bộ bạn sẽ làm như thế nào?
Có thể sử dụng Promise.all() hoặc async/await kết hợp với Promise.all() để chờ đợi nhiều tác vụ bất đồng bộ cùng hoàn thành
