# Audit và wireframe MetricsHub

| Vùng | Lỗi legacy | Giải pháp |
|---|---|---|
| Navbar | Grid 200/600/200px tổng 1000px trước padding, không theo độ dài nội dung; chuỗi menu gộp vào một div | Flexbox, các link riêng, wrap, gap và overflow-wrap |
| Dashboard | Flex lồng qua .column khóa widget vào hai cột; chiều cao 200px không biểu đạt span | Một Grid duy nhất, các widget siblings, span hàng/cột |
| Pricing | Float, clear và width tự viết dù có Bootstrap | row g-4, col-12 col-md-4, card h-100; không CSS riêng cho Pricing |

Ghi chú: code legacy được cung cấp không thực sự dùng float trong Dashboard; float nằm ở Pricing. Grid có thể tạo Navbar linh hoạt nếu dùng đúng track sizing, nhưng Flexbox phù hợp hơn trường hợp menu theo nội dung này.

## Wireframe desktop

Navbar [Flexbox]: Logo | các link tự giãn / xuống dòng | Profile

Dashboard [Grid]:

| A (span 2 cột, 2 hàng) | A | C |
| A | A | D |
| B (span 2 cột) | B | Trạng thái |

Pricing [Bootstrap]: Basic (4/12) | Pro (4/12) | Enterprise (4/12)

## Vấn đáp

Flexbox và Grid kết hợp được: Grid đặt widget, Flexbox căn biểu tượng và chữ bên trong. Bootstrap dùng Flexbox dưới lưới row/column và cung cấp gutter, breakpoint, utility thống nhất. Với layout zig-zag cần liên kết vị trí theo cả hai trục, ưu tiên Grid với areas hoặc span.

## Kiểm tra

Desktop: Grid 3 cột. Tablet dưới 992px: 2 cột. Mobile dưới 576px: 1 cột, bỏ span. Pricing chuyển sang 3 cột từ 768px theo Bootstrap. Navbar dùng wrap; từ dài có thể ngắt bên trong.
