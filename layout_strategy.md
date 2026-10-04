# Chiến lược layout

Navbar dùng Flexbox: căn các mục theo nội dung, dùng wrap và gap để menu dài xuống dòng.

Dashboard dùng Grid: kiểm soát hàng và cột, widget A span hai hàng và hai cột, widget B span hai cột. Widget là con trực tiếp của một grid. Tablet có hai cột; mobile một cột và bỏ span.

Pricing dùng Bootstrap row, col-12 col-md-4: ba cột từ 768px, xếp dọc dưới breakpoint này. Không viết CSS riêng cho lưới Pricing.

Grid phù hợp bố cục hai chiều, Flexbox phù hợp căn chỉnh component một chiều. Chúng kết hợp được: Grid đặt widget, Flexbox căn biểu tượng và chữ bên trong. Không có công cụ nào bắt buộc cho mọi layout.
