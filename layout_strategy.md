# Layout Strategy Report - MetricsHub

**Triết lý cốt lõi:** "CSS Grid sinh ra để dựng Layout tổng thể (2D), Flexbox sinh ra để quản lý Component chi tiết (1D)."

1. **Navbar (Flexbox):** Navbar là không gian 1 chiều dọc/ngang. Dùng Flexbox giúp các item tự căn chỉnh kích thước linh hoạt theo độ dài chữ (Content-First), tránh tình trạng tràn chữ khi thay đổi ngôn ngữ.
2. **Dashboard (CSS Grid):** Bento Box là bố cục 2 chiều phức tạp. Grid cho phép kiểm soát cả hàng và cột đồng thời với `grid-column: span` và `grid-row: span`, giúp loại bỏ hoàn toàn các thẻ `div` lồng nhau vô nghĩa (đánh tan Div Soup).
3. **Pricing (Bootstrap Grid):** Thành phần chuẩn hóa 3 cột cần dựng nhanh (Rapid Prototyping). Dùng lớp `col-12 col-md-4` giúp đạt độ phản hồi (Responsive) chuẩn trên nhiều thiết bị mà không cần viết CSS thuần.