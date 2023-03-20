1. DOM - Document Oject Model

- Element
- Atribute
- Text

2. JSON - JavaScript Object Notation

JSON là một định dạng dữ liệu tuân theo một quy luật nhất định mà hầu hết các ngôn ngữ lập trình hiện nay đều có thể đọc được. JSON là một tiêu chuẩn mở để trao đổi dữ liệu trên web.

- Stringtify: Từ JavaScript types -> JSON
- Parse: Từ JSON -> JavaScript
  JSON.stringtify(1) -> 1 (string)
  JSON.parse(x) -> x (string, number, null, array, object, boolean)

3. Promise

# Sync (đồng bộ)

- vd khi code chạy tuần tự theo thứ tự thì nó được gọi là đồng bộ

# Async (bất đồng bộ)

- Viết trước in ra sau (setTimeout, setInterval, fetch, XMLHttpRequest, file reading, request animation frame)

# Callback

- Dùng callback để xử lý các thao tác bất đồng bộ

# Promise

Promise là một khái niệm sinh ra để giúp chúng ta xử lý những thao tác bất đồng bộ và trước khi có promise chúng ta thường sử dụng callback và callback nó sẽ xảy ra vấn đề được gọi là callback hell. Nó sẽ bị sâu vào và khó nhìn (rối). Cho nên thằng promise nó được sinh ra từ phiên bản JS mới hơn ES6 và chúng ta có thể sử dụng nó để khắc phục tình trạng callback hell để giúp chúng ta viết code nó bị sâu vào và đọc dễ hiểu hơn.

Để sử dụng promise chúng ta sử dụng từ khóa new với Promise và trong constructor của nó chúng ta truyển vào một excutor function, trong excutor function chúng ta nhận được hai tham số dạng hàm, một là resolve, hai là reject, resolve nó sẽ được gọi khi thao tác thành công, reject khi thao tác thất bại.

Sử dụng phương thức .then và .catch (đều được nhận callback function) Khi promise resolved thì then được thực thi, và catch khi promise rejected.

Promise có 3 trạng thái:

- Pending
- Fulfilled
- Rejected

4. API (URL) - Application programming interface

Cổng giao tiếp giữa các phần mềm.
Backend -> API (URL) -> Fetch (để gọi lên API lấy dữ liệu) -> JSON/XML -> JSON.parse -> JavaScript types -> Render ra giao diện với HTML
