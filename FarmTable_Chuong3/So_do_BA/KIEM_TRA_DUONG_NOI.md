# Rà soát đường nối từ Hình 3.5 đến Hình 3.22

Đã mở/xuất từng tệp bằng trình biên tập Draw.io, rà ảnh ở kích thước lớn và kiểm tra hình học trên SVG thực xuất. Kiểm tra gồm: đường cắt qua khối không liên quan, đường đi qua chữ, nhãn nằm trên đường của chính nó, nhãn đè lên khối/nhãn khác. Cả 20 hình hiện không còn va chạm thuộc các nhóm kiểm tra này.

Đã đặt lại 130 nhãn connector và căn thẳng các đoạn nối đủ điều kiện. Màu cơ bản, nội dung nghiệp vụ, ký pháp và các quan hệ được giữ. Hình 3.10 có tác nhân/kho được vẽ lặp và ghi rõ để giảm đường giao nhau; đối chiếu theo định danh logic cho thấy 22 luồng không đổi.

| Hình | Rà soát / chỉnh sửa | Kết quả |
|---|---|---|
| 3.5 | Tách nhãn Có/Không khỏi đường, kiểm tra các nhánh duyệt và từ chối. | Không phát hiện va chạm khối/nhãn trên ảnh xuất. |
| 3.6 | Rà sequence flow, message flow, nhánh COD/online và callback; tách nhãn khỏi đầu nối. | Không phát hiện va chạm khối/nhãn trên ảnh xuất. |
| 3.7 | Giãn nhánh failed, làm thẳng hai gateway; tách hai nhãn Không theo đúng nhánh. | Không phát hiện va chạm khối/nhãn trên ảnh xuất. |
| 3.8 | Rà boundary timer, nhánh fallback, kết quả mô hình và hai message flow ML. | Không phát hiện va chạm khối/nhãn trên ảnh xuất. |
| 3.9 | Tách nhãn các cặp luồng hai chiều, giữ vùng quanh tiến trình trung tâm thoáng. | Không phát hiện va chạm khối/nhãn trên ảnh xuất. |
| 3.10 | Bố trí lại 5 tiến trình theo hàng; dùng ký hiệu lặp có ghi rõ; giữ nguyên 22 luồng logic, loại các tuyến dài chồng chéo. | Không phát hiện va chạm khối/nhãn trên ảnh xuất. |
| 3.11 | Kiểm tra các nhánh sitemap: các đoạn nối đã vuông góc, không cần đổi cấu trúc. | Không phát hiện va chạm khối/nhãn trên ảnh xuất. |
| 3.11a | Wireframe không có connector nghiệp vụ; đã kiểm tra bố cục và nhãn. | Không phát hiện va chạm khối/nhãn trên ảnh xuất. |
| 3.12 | Tách 14 nhãn quan hệ khỏi trường dữ liệu và các đường khác; giữ Crow’s Foot. | Không phát hiện va chạm khối/nhãn trên ảnh xuất. |
| 3.12a | Rà đường vòng product–event và user–audit log; đưa nhãn ra khỏi vùng thuộc tính. | Không phát hiện va chạm khối/nhãn trên ảnh xuất. |
| 3.13 | Rà 14 lời gọi/phản hồi, nhãn không che activation/lifeline. | Không phát hiện va chạm khối/nhãn trên ảnh xuất. |
| 3.14 | Làm thẳng các đoạn nối, tách nhãn điều kiện Có/Không. | Không phát hiện va chạm khối/nhãn trên ảnh xuất. |
| 3.15 | Sửa nhánh xung đột đi vòng bên trái khối Abort, tránh khối Trả lỗi; căn thẳng các bước chính. | Không phát hiện va chạm khối/nhãn trên ảnh xuất. |
| 3.16 | Đưa điều kiện chuyển trạng thái ra ngoài khối; căn thẳng các hướng chuyển. | Không phát hiện va chạm khối/nhãn trên ảnh xuất. |
| 3.17 | Rà nhánh worker, đường lặp membership và đường kết thúc; nhãn đi kèm đúng nhánh. | Không phát hiện va chạm khối/nhãn trên ảnh xuất. |
| 3.18 | Rà idempotency, giá/tồn, abort và commit; căn các đoạn nối ngắn. | Không phát hiện va chạm khối/nhãn trên ảnh xuất. |
| 3.19 | Tách nhãn tạo giao dịch, callback, thanh toán lại và hủy; giữ final state. | Không phát hiện va chạm khối/nhãn trên ảnh xuất. |
| 3.20 | Kiểm tra pipeline, đường nạp artifact và nhãn giữa hai vùng. | Không phát hiện va chạm khối/nhãn trên ảnh xuất. |
| 3.21 | Kiểm tra hai nhánh model/fallback, đường gom và đầu ra. | Không phát hiện va chạm khối/nhãn trên ảnh xuất. |
| 3.22 | Kiểm tra nhánh an toàn, gọi hàm, giới hạn lượt và đường lặp ngoài các khối. | Không phát hiện va chạm khối/nhãn trên ảnh xuất. |

Bản Word/PDF thay bằng ảnh vừa xuất; link cạnh chú thích trỏ đến đúng phiên bản nguồn mới. Riêng Hình 3.10 được tăng kích thước trong Word. Các bản master Draw.io, A3, PNG, SVG và ZIP cũng được đồng bộ.

Kết quả hình học chi tiết nằm trong `kiem_tra_drawio/ket_qua_kiem_tra_duong_noi.json`. Kiểm tra này đánh giá bố cục/đường nối của sơ đồ, không thay thế kiểm thử phần mềm.
