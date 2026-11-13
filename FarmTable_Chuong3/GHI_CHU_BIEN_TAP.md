# Ghi chú biên tập Chương 3

## Văn phong

Đối chiếu các phần đã có nội dung ở Chương 1, 4, 5 và 6 trong FarmTable_Outline.md. Bản trước thiên về mô tả kỹ thuật với nhiều câu ngắn, nhãn “Bài toán”, “Quy tắc” và lưu ý cho người biên soạn. Bản mới chuyển thành lời trình bày của nhóm, giải thích bối cảnh trước khi đi vào phương pháp, bổ sung quan hệ giữa các đoạn và thống nhất cách gọi người mua, nhà bán, quản trị viên. Thuật ngữ và tên trường vẫn được giữ khi cần đối chiếu thiết kế.

Các mục 3.1–3.8, 16 bảng và 24 sơ đồ được giữ. Hình 3.11b là ảnh giao diện bổ sung ngoài danh mục outline, không phải sơ đồ Draw.io; ảnh này không nằm trong bản chỉnh văn phong. Hình 3.11a (wireframe) và 3.12a (ERD hỗ trợ) vẫn được giữ cùng 22 hình trong outline.

Lưu ý về môi trường thực thi và hướng dẫn biên tập được đặt trong README/ghi chú này để không ngắt mạch nội dung báo cáo. Những giới hạn thuộc phương pháp, chẳng hạn dữ liệu nhãn gợi ý chưa phủ toàn catalog và nghiên cứu khả dụng chưa có người tham gia, vẫn được trình bày trong chương.

## Định dạng và liên kết

Bản PDF 37 trang, khổ A4. Toàn bộ chữ được soạn trong Word dùng cỡ 13; nội dung dùng Times New Roman, mã minh họa dùng Courier New. Cỡ chữ bên trong sơ đồ giữ theo bản Draw.io đã thiết kế. Chú thích hình căn giữa, in nghiêng, kèm “(link)” màu xanh và gạch chân theo mẫu. Cả Word và PDF có 24 liên kết thực.

Liên kết mở ứng dụng https://app.diagrams.net/ và nạp đúng tệp `.drawio` của từng hình. Nguồn sơ đồ được ghim theo phiên bản khớp với ảnh trong báo cáo: Hình 3.1/3.3 tại `3360c016c846168f93370341e93e597bb8c32453`; Hình 3.2 tại `4a5de44b56c87e73e7a779919a11b56253b606d2`; Hình 3.4 tại `d0225b81f29f8f7f62900127e5f587fb40eaa83b`; toàn bộ 20 hình từ 3.5 trở đi tại `36bd42a778f872a18aaae8e58403dd1c1ebd3c73`. Không yêu cầu quyền ghi repo khi mở để xem; có thể tải/lưu bản riêng để chỉnh sửa.

Đã kiểm tra cấu trúc DOCX, 24 ảnh/24 liên kết, 16 bảng; kiểm tra văn bản PDF có cỡ 13 và không tràn lề; kiểm tra 24 URL nguồn trả HTTP 200 và XML Draw.io hợp lệ. Đã rà soát bố cục bản PDF sau chuyển đổi. Kiểm tra URL nguồn không thay thế việc kiểm tra trình duyệt của từng người đọc.

## Nguồn và phạm vi xác minh

Nội dung đối chiếu FarmTable_Outline.md, FarmTable_ThongTin.md và mã nguồn `lini1907/Web_Project`, nhánh `feat/v2-fullstack`, commit `5b949f0a0b575308266e49af7b5d52604e8daf9d`. Đây là lần chỉnh tài liệu, không sửa mã nguồn ứng dụng.

Frontend đã build thành công ở lần kiểm tra trước. Bộ kiểm thử API phụ thuộc MongoDB chưa được xác minh trong phiên soạn vì môi trường chặn tải binary từ máy chủ MongoDB. Mục 3.8.1 trình bày phương pháp/kịch bản kiểm thử, không phải xác nhận các ca đã chạy đạt trong phiên này. Các mã TC và thống kê bộ kiểm thử dẫn theo tài liệu dự án. Phần SUS là đề xuất bổ sung phương pháp, chưa có dữ liệu thu thập thực tế.

## Chỉnh riêng Hình 3.2 theo phản hồi

Đổi sang bảng màu trắng/xám và be nhạt. Giãn các khối, tách nhãn khỏi đường, sửa điểm kết thúc ở package nghiệp vụ, đặt đường gọi dịch vụ ngoài dưới MongoDB và tách đường SSE quay về giao diện. Bảy quan hệ vẫn giữ nội dung và cặp nguồn–đích. Hình được mở/xuất lại bằng Draw.io; bản tổng hợp 24 trang, ảnh PNG, vector SVG, A3, ZIP và ảnh trong chương đều đã đồng bộ. Liên kết ở chú thích Hình 3.2 trong Word/PDF mở phiên bản mới.

## Chỉnh riêng Hình 3.4 theo mẫu đường nối

Giữ 14 chức năng dạng oval và bốn tác nhân ở ngoài biên hệ thống. Toàn bộ 16 association giữa tác nhân và chức năng dùng đoạn thẳng nét liền, đúng kiểu trong ảnh tham khảo; hai include dùng nét đứt và đầu mũi tên mở. Đổi màu thành pastel theo nhóm: xanh nhạt cho các chức năng dùng chung/khách, mint cho giao dịch người mua, cam kem cho nhà bán và tím nhạt cho quản trị. Sắp lại ba use case mua hộp, đặt hàng và kiểm tra giá/tồn để đường include cũng đi thẳng. Nội dung và các cặp nguồn–đích vẫn giữ nguyên. Đã đồng bộ tệp gốc, PNG/SVG, bản A3, ZIP và Word/PDF; chú thích Hình 3.4 mở bản mới.

## Phối màu tiết chế từ Hình 3.5 trở đi

Thay 20 hình từ 3.5–3.22 (có 3.11a, 3.12a) bằng bản phối màu pastel trong từng hình. Nền trắng, màu nhạt, chữ và đường nối tối. BPMN phân biệt trách nhiệm; ERD chỉ tô tiêu đề theo nhóm dữ liệu; sequence theo thành phần; lưu đồ/state machine nhấn điều kiện, chờ, thành công và lỗi. Chi tiết tại `So_do_BA/QUY_UOC_MAU_BA.md`.

Đợt này chỉ thay thuộc tính màu của các đối tượng; đã đối chiếu để giữ toàn bộ nhãn, kiểu shape, kích thước, vị trí và đường nối. Hình 3.1–3.4 giữ nguyên. Đã mở/xuất lại 20 hình và bộ 24 trang trong Draw.io; thay ảnh trong Word/PDF và cập nhật 20 liên kết tương ứng, giữ bốn liên kết còn lại. Nội dung chương và cỡ chữ 13 được giữ lại.
