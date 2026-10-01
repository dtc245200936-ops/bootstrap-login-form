# Báo Cáo Phân Tích Kỹ Thuật: Tác Hại Của Absolute Positioning Và Sức Mạnh Của CSS Grid

## 1. Tác hại của `position: absolute` đối với Responsive Design
Kỹ thuật dàn trang cổ điển sử dụng `position: absolute` đưa phần tử ra khỏi luồng hiển thị thông thường của tài liệu (Document Flow). Việc gán cứng chiều cao (`height: 400px`) cho khung chứa làm mất khả năng tự động co giãn theo nội dung bên trong. 

Khi kích thước màn hình thu nhỏ (Mobile Breakpoint), các phần tử con bị nén, dàn hàng hoặc vỡ khung, dẫn đến hiện tượng các phần tử phía sau (như đoạn văn bản bài viết) chèn đè lên hình ảnh do khung chứa không còn tính toán đúng chiều cao thực tế.

## 2. CSS Grid – Giải pháp kiến trúc bền vững
CSS Grid giải quyết hoàn toàn bài toán này nhờ vào:
* **Tính toán không gian tự động (2D Layout System):** Cho phép chia cột và hàng linh hoạt bằng đơn vị `fr` (fractional unit) mà không cần tính toán phần trăm hay pixel thủ công.
* **Bảo toàn Document Flow:** Thẻ chứa tự động mở rộng theo chiều cao của Grid Items.
* **Tùy biến Responsive dễ dàng:** Thông qua Media Queries, chỉ cần đổi `grid-template-columns: 1fr` trên Mobile là toàn bộ thư viện ảnh khảm lập tức xếp chồng dọc an toàn mà không làm đè lấn lên các thành phần xung quanh.