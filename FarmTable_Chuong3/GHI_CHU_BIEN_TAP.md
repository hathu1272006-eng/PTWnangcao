# Ghi chú biên tập Chương 3

## Văn phong

Đối chiếu các phần đã có nội dung ở Chương 1, 4, 5 và 6 trong FarmTable_Outline.md. Bản trước thiên về mô tả kỹ thuật với nhiều câu ngắn, nhãn “Bài toán”, “Quy tắc” và lưu ý cho người biên soạn. Bản mới chuyển thành lời trình bày của nhóm, giải thích bối cảnh trước khi đi vào phương pháp, bổ sung quan hệ giữa các đoạn và thống nhất cách gọi người mua, nhà bán, quản trị viên. Thuật ngữ và tên trường vẫn được giữ khi cần đối chiếu thiết kế.

Các mục 3.1–3.8, 16 bảng và 24 sơ đồ được giữ. Hình 3.11b là ảnh giao diện bổ sung ngoài danh mục outline, không phải sơ đồ Draw.io; ảnh này không nằm trong bản chỉnh văn phong. Hình 3.11a (wireframe) và 3.12a (ERD hỗ trợ) vẫn được giữ cùng 22 hình trong outline.

Lưu ý về môi trường thực thi và hướng dẫn biên tập được đặt trong README/ghi chú này để không ngắt mạch nội dung báo cáo. Những giới hạn thuộc phương pháp, chẳng hạn dữ liệu nhãn gợi ý chưa phủ toàn catalog và nghiên cứu khả dụng chưa có người tham gia, vẫn được trình bày trong chương.

## Định dạng và liên kết

Bản PDF 37 trang, khổ A4. Toàn bộ chữ được soạn trong Word dùng cỡ 13; nội dung dùng Times New Roman, mã minh họa dùng Courier New. Cỡ chữ bên trong sơ đồ giữ theo bản Draw.io đã thiết kế. Chú thích hình căn giữa, in nghiêng, kèm “(link)” màu xanh và gạch chân theo mẫu. Cả Word và PDF có 24 liên kết thực.

Liên kết mở ứng dụng https://app.diagrams.net/ và nạp đúng tệp `.drawio` của từng hình. Nguồn sơ đồ được ghim tại commit `3360c016c846168f93370341e93e597bb8c32453` của repo PTWnangcao để khớp với ảnh trong báo cáo. Không yêu cầu quyền ghi repo khi mở để xem; có thể tải/lưu bản riêng để chỉnh sửa.

Đã kiểm tra cấu trúc DOCX, 24 ảnh/24 liên kết, 16 bảng; kiểm tra văn bản PDF có cỡ 13 và không tràn lề; kiểm tra 24 URL nguồn trả HTTP 200 và XML Draw.io hợp lệ. Đã rà soát bố cục bản PDF sau chuyển đổi. Kiểm tra URL nguồn không thay thế việc kiểm tra trình duyệt của từng người đọc.

## Nguồn và phạm vi xác minh

Nội dung đối chiếu FarmTable_Outline.md, FarmTable_ThongTin.md và mã nguồn `lini1907/Web_Project`, nhánh `feat/v2-fullstack`, commit `5b949f0a0b575308266e49af7b5d52604e8daf9d`. Đây là lần chỉnh tài liệu, không sửa mã nguồn ứng dụng.

Frontend đã build thành công ở lần kiểm tra trước. Bộ kiểm thử API phụ thuộc MongoDB chưa được xác minh trong phiên soạn vì môi trường chặn tải binary từ máy chủ MongoDB. Mục 3.8.1 trình bày phương pháp/kịch bản kiểm thử, không phải xác nhận các ca đã chạy đạt trong phiên này. Các mã TC và thống kê bộ kiểm thử dẫn theo tài liệu dự án. Phần SUS là đề xuất bổ sung phương pháp, chưa có dữ liệu thu thập thực tế.
