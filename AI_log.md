# AI LOG – BUỔI 7, TIẾT 3

> Điền vào `[ ... ]`, tích `[x]` vào lựa chọn phù hợp. Ghi đúng việc đã làm; chưa kiểm tra thì ghi “Chưa kiểm tra”. Không cần chép toàn bộ cuộc trò chuyện AI.

## Thông tin sinh viên

- Họ và tên: Lê ngọc Hưng
- Mã sinh viên – Lớp: 1671020151 
- Ngày thực hiện:  30/10/2026
- Link repository:  https://github.com/Wipper0000/CV.git 
- URL website:  https://github.com/Wipper0000/CV 
- Tình huống: [x] Website của tôi  [ ] Repo luyện của giảng viên

## 1. Nhận định của tôi trước khi hỏi AI

- Trang/thao tác gặp lỗi: Toàn bộ website (các trang `index.html` và `ket-qua.html`).
- Mong muốn và hiện tượng thực tế:
  - Mong muốn: Giao diện CV/Portfolio cá nhân hiện đại, chuyên nghiệp, chuẩn responsive và sẵn sàng để demo.
  - Hiện tượng thực tế: Giao diện còn thô và mang tính bài tập cơ bản (danh sách kỹ năng thuần chữ, bảng học tập cổ điển, thẻ dự án đơn điệu, thiếu micro-interactions); tồn tại lỗi đường dẫn tệp.
- Dữ kiện đã kiểm tra (cấu trúc tệp, Request URL, Status…):
  - `ket-qua.html`: Dòng 8 chứa đường dẫn tuyệt đối cục bộ `D:\CNTT20-04\portfolio\css\style.css` (gây lỗi hiển thị khi deploy).
  - `index.html`: Dòng 10 dùng gạch chéo ngược `css\style.css` (chưa đúng chuẩn web).
  - `style.css`: Chưa dùng CSS Variables (`:root`), khó quản lý theme màu và responsive.
- Tôi nghi nguyên nhân là: Thiếu quy chuẩn Design System (CSS Variables) và cấu trúc giao diện chưa được tối ưu hóa thành các UI components hiện đại (Badges, Cards, Timeline).
- Vì sao tôi nhận định như vậy: Trực quan trang còn đơn điệu, các phần tử quan trọng (Kỹ năng, Dự án, Học tập) chỉ sử dụng các thẻ HTML cơ bản (`ul`, `table`) chưa được trau chuốt về UX/UI.

## 2. Tôi hỏi AI và nhận được gợi ý

- Nguồn: [x] Công cụ AI: [ Antigravity / Gemini ]  [ ] Phản hồi mẫu của giảng viên
- Câu hỏi/prompt tôi đã gửi (hoặc tình huống của phản hồi mẫu):

  `lên cho tôi kế hoạch demo cải thiện giao diện web trên project này.`

- Gợi ý chính của AI:

  1. Định hướng phong cách Modern Tech Portfolio, thiết lập bảng màu chuẩn qua CSS Variables (`:root`).
  2. Nâng cấp 7 khu vực: Header Sticky Glassmorphism; Hero nổi bật (Avatar shadow, Status badge, 2 nút CTA); Skills dạng thẻ Badge phân loại; Projects có Tech Tags & nút Demo/Code; Education chuyển từ `table` sang Timeline dọc; Contact chia layout 2 cột; Footer có nút Back-to-top.
  3. Đưa ra lộ trình triển khai 5 bước rõ ràng trước khi can thiệp vào code.

## 3. Quyết định của tôi

- [x] Chấp nhận gợi ý
- [ ] Chỉnh sửa gợi ý rồi áp dụng
- [ ] Bác bỏ gợi ý

- Tôi quyết định làm gì: Tiếp nhận toàn bộ kế hoạch cải thiện giao diện theo lộ trình 5 bước; thống nhất sẽ sửa các lỗi đường dẫn trước rồi mới nâng cấp giao diện từng khu vực.

- Lý do, dựa trên dữ kiện nào: giải quyết đúng các lỗi path CSS.

## 4. Thực hiện và kiểm chứng

- Tệp/vị trí đã sửa (không sửa thì ghi rõ): Chưa sửa trực tiếp trên mã nguồn
- Nội dung thay đổi hoặc cách xử lý khác: 
- Commit của bản sửa, nếu có: Chưa commit code (mới ghi nhận kế hoạch vào AI Log).
- Bản sửa đã deploy: [ ] Có  [x] Chưa  [ ] Không phát sinh bản sửa

| Nội dung kiểm tra | Trước xử lý | Sau xử lý/thử lại |
| --- | --- | --- |
| Request URL và Status của tài nguyên liên quan | `ket-qua.html` liên kết đường dẫn tuyệt đối máy cá nhân (dễ lỗi 404 khi deploy) | Đã xác định cần chuyển thành đường dẫn tương đối `css/style.css` trong bước tới |
| Giao diện/chức năng trên URL website | Bố cục dạng bài tập cơ bản, bảng biểu và danh sách thô | Đã có kế hoạch chi tiết nâng cấp thành giao diện Portfolio hiện đại |

- Cách thử lại và kết quả thực tế: Rà soát lại từng thành phần trong `index.html` và `style.css` đối chiếu với kế hoạch 5 bước; kế hoạch hoàn toàn khả thi và bám sát dự án.
- Căn cứ để đối chiếu (URL tệp, commit, đường dẫn ảnh chụp hoặc dữ kiện quan sát): Nội dung kế hoạch cải tiến UI chi tiết được lưu trong phiên làm việc với AI và tệp `AI_log.md`.

## 5. Kết luận

- [x] Đã xử lý được  [ ] Xử lý được một phần  [ ] Chưa xử lý được
- Điều tôi rút ra hoặc việc cần làm tiếp: Cần có kế hoạch thiết kế và rà soát lỗi kỹ thuật (đường dẫn tệp) trước khi can thiệp vào code; bước tiếp theo sẽ bắt tay vào thực hiện Bước 1 (sửa đường dẫn, tạo CSS Variables) và Bước 2 (Header, Hero).

---

*Tệp là minh chứng MC2 để nhận định mức đạt của tiết học; không tính điểm MC2 riêng. Nếu có tình huống khác, sao chép mục 1–5 để ghi thêm.*
