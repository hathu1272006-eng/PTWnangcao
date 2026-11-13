# FarmTable – Chương 3: Phương pháp thực hiện

Người viết: Vũ Thu Hà. Bản Word/PDF 26 trang đã thay các hình bằng bộ sơ đồ vẽ lại theo ký pháp nghiệp vụ.

## Tải tài liệu

- **[Tệp Draw.io nhiều trang, chỉnh sửa được](So_do_BA/FarmTable_Chuong3_BA.drawio?raw=true)**
- **[PDF sơ đồ khổ A3, 24 trang để đọc/in chi tiết](So_do_BA/FarmTable_So_do_BA_A3.pdf?raw=true)**
- [Word sơ đồ khổ A3](So_do_BA/FarmTable_So_do_BA_A3.docx?raw=true)
- [Tải trọn bộ Draw.io, PNG, SVG và bản A3](So_do_va_anh_Chuong3.zip?raw=true)
- [Chương 3 – Word đã thay hình](FarmTable_Chuong3.docx?raw=true)
- [Chương 3 – PDF đã thay hình](FarmTable_Chuong3.pdf?raw=true)

Để sửa: tải tệp `.drawio`, mở https://app.diagrams.net/ → **File → Open From → Device**. Đổi trang bằng thanh tab phía dưới. Mỗi khối, nhãn và đầu nối là đối tượng gốc, không phải một ảnh nền. Đọc [hướng dẫn và danh mục đầy đủ](So_do_BA/README_BA.md).

Nếu GitHub không xem trước được, chọn **Download raw file**. Bản A3 là bản chi tiết để đọc các trường ERD và nhãn dài; hình trong chương được thu nhỏ để giữ nhịp nội dung.

## Bộ hình vẽ lại

24 trang gồm 22 hình theo outline, ERD hỗ trợ (3.12a) và wireframe (3.11a). Dùng UML Use Case, Activity, Sequence, State Machine; BPMN 2.0 với pool/lane, XOR và timer boundary; DFD Yourdon–DeMarco; Logical ERD Crow’s Foot. Các hình còn lại dùng flowchart, pipeline hoặc sitemap phù hợp mục đích.

![Ví dụ BPMN duyệt nhà bán](So_do_BA/png/Hinh_3_5.png)

## Nguồn và kiểm tra

Đối chiếu mã nguồn `lini1907/Web_Project`, nhánh `feat/v2-fullstack`, commit `5b949f0a0b575308266e49af7b5d52604e8daf9d`. Bộ hình đã mở/xuất SVG bằng trình biên tập Draw.io cục bộ; kiểm tra đầu nối, pool boundary và ký pháp theo từng loại hình. Xem ảnh mở trong Draw.io ở `So_do_BA/kiem_tra_drawio/`.

Frontend đã build thành công. Bộ kiểm thử API cần MongoDB chưa được xác minh trong phiên soạn vì môi trường chặn tải binary MongoDB. Các mã TC dẫn theo outline không được hiểu là kết quả vừa chạy đạt.
