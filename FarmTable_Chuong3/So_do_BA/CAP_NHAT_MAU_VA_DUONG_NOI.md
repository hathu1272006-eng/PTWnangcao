# Cập nhật màu và đường nối

- 24 hình dùng 24 tông chủ đạo riêng; hình dạng, nhãn và vai trò của connector được giữ nguyên.
- Giữ nền sáng, chữ tối; màu pastel là hỗ trợ thị giác, không tạo quy tắc nghiệp vụ mới.

| Hình | Điều chỉnh đường nối / nhãn |
|---|---|
| 3.1 | Đường phản hồi từ kiểm thử đi vòng ngoài, tránh xuyên qua khối Angular. |
| 3.3 | Bốn đường lỗi có kênh riêng; bỏ đoạn tự đi ngược và đè nhau. |
| 3.5 | Nhánh từ chối đi vòng tới kết quả, tránh sự kiện kết thúc. |
| 3.6 | Hai nhánh XOR dùng hai cổng ra khác nhau; nhãn IPN và sự kiện cuối không nằm trên đường vào. |
| 3.7 | Nhãn quyết định hủy đặt cạnh gateway; mũi tên vào sự kiện cuối đi từ cạnh bên. |
| 3.8 | Nhãn gateway và timer tách khỏi đường fallback / timeout. |
| 3.12a | Quan hệ sản phẩm–sự kiện đi vòng dưới, tránh cắt quan hệ người dùng–lịch sử gợi ý. |
| 3.17 | Vòng lặp worker trở lại từ phía trên, tách khỏi nhánh kết thúc. |
| 3.21 | Nhánh dùng kết quả mô hình đi vòng dưới ghi chú. |
| 3.22 | Vòng lặp chatbot đi ở mép ngoài, tránh hình bắt đầu, ghi chú và phụ đề. |

Đã đối chiếu ID đầu–cuối, nhãn và loại đầu nối với bản trước, mở/xuất trong Draw.io, kiểm tra các ràng buộc BPMN/UML/DFD và số trang bộ hình. Các thay đổi thuộc trình bày; không thay nội dung nghiệp vụ trong chương.


## Hình 3.2 – giản lược màu và sửa đường nối

- Đổi nền xanh ngọc sang trắng/xám, chỉ nhấn be nhạt ở API và lớp nghiệp vụ; chữ và đường nối dùng xám đậm.
- Tăng khoảng cách giữa giao diện, API, lớp nghiệp vụ, cơ sở dữ liệu và các dịch vụ ngoài.
- Nhãn HTTPS/JSON, SSE và đọc/ghi được đặt lệch khỏi đường nối để không che đầu mũi tên.
- Đường gọi Google/Gemini/SMTP đi dưới khối MongoDB, không xuyên qua dữ liệu; đường SSE quay về giao diện theo hành lang riêng.
- Đầu mũi tên gọi nghiệp vụ bám vào cạnh trên phần thân package.
- Giữ nguyên nội dung của bảy quan hệ và cặp phần tử nguồn–đích. Đã mở/xuất lại bằng Draw.io và kiểm tra ảnh kết quả.


## Hình 3.4 – use case pastel và đường nối thẳng

- Dùng oval cho use case, actor ở ngoài biên hệ thống; nền trắng, chữ và đường nối màu tối.
- Màu pastel phân biệt nhóm chức năng: xanh nhạt cho chức năng dùng chung/khách; mint cho giao dịch người mua; cam kem cho nhà bán; tím nhạt cho quản trị.
- Cả 16 association từ actor đến chức năng là một đoạn thẳng, nét liền; không dùng đường gấp vuông. Association giữ ký pháp UML không đầu mũi tên.
- Hai quan hệ include dùng nét đứt, đầu mũi tên mở hướng đến use case được bao gồm. Đặt Mystery Box, Đặt hàng và Kiểm tra giá/tồn gần nhau để hai đường này cũng đi thẳng.
- Giữ nguyên tên, số lượng và cặp nguồn–đích của các quan hệ; đã mở/xuất lại bằng Draw.io và kiểm tra hình.


## Từ Hình 3.5 – phối nhiều màu pastel trong từng hình

Đã thay cách tô một tông cho toàn hình bằng phối màu theo vai trò, dữ liệu, bước xử lý và trạng thái. Gồm 20 hình từ 3.5 đến 3.22, có 3.11a/3.12a. Các điểm nối, geometry và ký pháp được giữ nguyên. Xem `QUY_UOC_MAU_BA.md` và bảng phối màu mới.


## Bản cơ bản từ Hình 3.5

Đã giản lược 20 hình sang trắng/xám nhạt, chỉ nhấn nhẹ một số khối bằng xanh xám. Cấu trúc, ký pháp và đường nối giữ nguyên. Bản này thay thế cách phối nhiều màu trong từng hình ở lần trước.
