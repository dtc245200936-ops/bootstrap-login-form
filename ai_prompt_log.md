# AI Prompt Log

1. **Brainstorming Tool Selection:**
   * *Prompt:* "Khi tôi cần một bố cục mà một phần tử con (Child) phải chiếm chính xác 2 hàng và 2 cột (span 2 rows, 2 columns) đan xen với các phần tử nhỏ khác, tôi nên chọn CSS Grid hay Flexbox? Tại sao Flexbox lại chật vật với yêu cầu này?"
   * *Kết quả:* Nhận diện rõ giới hạn 1D của Flexbox và lợi thế 2D của Grid.

2. **Bootstrap Query:**
   * *Prompt:* "Trong Bootstrap 5, sự khác biệt giữa lớp col-sm-4 và col-md-4 là gì? Tại sao tôi nên dùng Bootstrap thay vì tự viết CSS Grid cho một phần tử đơn giản như 3 cột Bảng giá?"
   * *Kết quả:* Nắm được các breakpoint (`sm: >=576px`, `md: >=768px`) và tính tiện lợi của thuộc tính `gap` / system grid.

3. **CSS Tuning:**
   * *Prompt:* "Hãy cho tôi xem một cú pháp CSS Grid đơn giản sử dụng span để tạo layout Bento Box có 1 hình lớn 2x2 và các hình nhỏ xung quanh."
   * *Kết quả:* Áp dụng thành công `grid-template-columns: repeat(3, 1fr)` kết hợp `span 2`.