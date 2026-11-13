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
