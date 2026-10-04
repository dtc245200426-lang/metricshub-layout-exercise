# Nhật ký dùng AI

## Yêu cầu thực tế
Người học gửi toàn bộ đề thực hành MetricsHub trong file văn bản và tiếp tục quy trình hoàn thiện bài, lấy link nộp. Không có các prompt brainstorm riêng được người học gửi trong cuộc trò chuyện này.

## Phần trợ lý thực hiện
- Đọc đề và xác định ba vùng: Navbar 1D, Dashboard 2D, Pricing 12 cột.
- Viết implementation mới theo từng vùng: Flexbox có wrap và gap; Grid với siblings trực tiếp và span; Bootstrap với col-12 col-md-4.
- Bổ sung breakpoint tablet/mobile, overflow-wrap cho từ dài.
- Tạo báo cáo audit, giải trình, wireframe và ZIP nộp bài.

## Ghi chú về quy tắc của đề
Đề yêu cầu người học tự phân tích và không giao toàn bộ việc tái cấu trúc legacy cho AI. Bản này có mã do AI tạo; người học cần đọc, tự kiểm tra và trình bày được lựa chọn thiết kế trước khi nộp. Không mô tả các prompt gợi ý trong đề là prompt người học đã thực sự sử dụng.

## Kiến thức cần tự giải thích
- gap tạo khoảng cách giữa các item của cả Grid và Flexbox, không tạo lề ngoài container.
- Flexbox một chiều; Grid hai chiều. Grid không luôn là lựa chọn bắt buộc cho mọi layout tổng thể.
- col-sm-4 bắt đầu ba cột từ 576px; col-md-4 từ 768px.
- Bootstrap Grid dùng Flexbox và breakpoint/spacing thống nhất, giúp giảm CSS tự viết cho cấu trúc chuẩn.
