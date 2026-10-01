# AI Prompt Log - Tra Cứu CSS Grid & Bootstrap Utilities

## Prompt 1: Hỏi về CSS Grid Spanning
* **User:** "Làm sao để tạo một CSS Grid gồm 2 cột, trong đó 1 ảnh bên trái chiếm toàn bộ chiều cao của 2 ảnh bên phải?"
* **AI Output Summary:** Sử dụng `grid-template-columns: 2fr 1fr;` và cho ảnh chính dùng thuộc tính `grid-row: 1 / 3` (hoặc `grid-row: span 2`). Kết hợp `object-fit: cover` để ảnh không bị méo tỷ lệ.

## Prompt 2: Tra cứu Bootstrap Alignment & Spacing
* **User:** "Thay vì viết CSS thủ công cho thanh Author Info, Bootstrap 5 có những Class Utility nào hỗ trợ Flexbox căn giữa và khoảng cách?"
* **AI Output Summary:** Có thể dùng combo class `d-flex align-items-center justify-content-between flex-wrap gap-2` để thay thế hoàn toàn CSS căn chỉnh Float thủ công.

## Prompt 3: Cấu hình Breakpoints cho Bootstrap Grid
* **User:** "Cấu hình class `col` như thế nào để 4 thẻ bài viết hiển thị 1 cột trên Mobile, 2 cột trên Tablet và 4 cột trên Desktop?"
* **AI Output Summary:** Sử dụng chuỗi class: `col-12 col-md-6 col-lg-3`.