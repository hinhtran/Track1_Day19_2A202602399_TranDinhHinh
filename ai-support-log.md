# AI Support Log

*(Ghi chép trung thực việc dùng AI trong quá trình làm bài Lab Day 18)*

- **AI đã giúp gì:**
  - Hỗ trợ xây dựng nhanh giao diện tương tác `prototype.html` bằng TailwindCSS và Vanilla JS đảm bảo 70% common context.
  - Chuẩn hóa cấu trúc bảng quan sát hành vi Fact-First và 4 tầng tư duy sư phạm cho `prototype-feedback-note.md`.
  - Hỗ trợ đối chiếu, phát hiện pattern hành vi và xây dựng tài liệu tổng hợp nhóm `group-feedback-synthesis.md`.

- **Điểm sai/hời hợt của AI (nếu có):**
  - Giao diện ban đầu của AI đặt tên nút chọn phương án mang tính định kiến (`Quyen: User Control`, `Dung: AI Co-pilot`, `Hinh: AI Diagnostic`), dễ làm lệch tâm lý người thử nghiệm.
  - Thiếu cơ chế kiểm soát / phục hồi (Control & Recovery / Fallback) ở Option C khi AI chẩn đoán sai bệnh.
  - Thông báo ở Option B lúc đầu ghi lộ cơ chế kỹ thuật ("chờ 3 giây AI quét").

- **Cách tự sửa:**
  - Tự yêu cầu và sửa đổi nhãn nút sang trung tính: *Phương án A, Phương án B, Phương án C*.
  - Bổ sung nút và hàm `overrideDiagnosis()` ở Option C để người dùng có thể tự chọn lại chủ đề khi AI đoán sai.
  - Thay đổi thông báo tạm dừng video ở Option B sang câu từ tự nhiên theo ngữ cảnh bài học.
