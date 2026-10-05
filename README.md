# Track 1 - Day 18

## 1. Thông tin cá nhân và nhóm
- MHV: 2A202602399
- Họ tên: Trần Đình Hinh
- Tên nhóm: Prompt Kiếm Tông
- Thành viên: Hoàng Quốc Dũng, Trần Đình Hinh, Đinh Xuân Quyền
- Case đã chọn: Case A — AI Tutor: Diagnostic Refresher

## 2. Hypothesis Problem
Khi gặp một khái niệm/bài tập khó, người học gặp khó khăn trong việc hoàn thành bài học vì không tự xác định được lỗ hổng kiến thức nền tảng của mình (không biết những gì mình không biết), dẫn đến việc tra cứu mông lung, mất nhiều thời gian (mất 5-10 phút mò slide) và dễ nản chí bỏ cuộc.

## 3. Three Solution Options
* **Option A (User-led):** Sơ đồ do AI tạo theo yêu cầu (User tự nhìn sơ đồ và phán đoán bệnh).
* **Option B (AI Co-pilot):** Sơ đồ tự động + AI Highlight gợi ý nhấp nháy trên bản đồ để user xác nhận.
* **Option C (AI Diagnostic):** AI chẩn đoán thông qua 2 câu trắc nghiệm nhanh, tự động chỉ định luôn chỗ hổng kiến thức.

📄 Chi tiết thiết kế và bảng phân tích Human-AI: [three-option-design-sheet.md](three-option-design-sheet.md)  
🌐 Link prototype: File `prototype.html` (chạy trực tiếp trên trình duyệt) — xem chi tiết tại [prototype-link.md](prototype-link.md).

## 4. Đóng góp của tôi trong nhóm
- Chịu trách nhiệm thiết kế và đặc tả tương tác chính cho **Option C (AI Diagnostic - AI chẩn đoán qua 2 câu hỏi trắc nghiệm nhanh)**.
- Tham gia xây dựng giao diện chung trên `prototype.html` đảm bảo 70% common context (khung bài giảng video) và cơ chế chuyển đổi trung tính giữa các phương án.
- Trực tiếp điều phối và phỏng vấn thực tế với người học ngoài nhóm (Tester: Dương Hải Minh - MHV: 2A202602680), hoàn thành bảng [prototype-feedback-note.md](prototype-feedback-note.md) cá nhân.
- Cùng nhóm tổng hợp, đối chiếu 3 bản feedback của các thành viên để rút ra các pattern hành vi và xây dựng tài liệu [group-feedback-synthesis.md](group-feedback-synthesis.md).

## 5. Prototype Feedback
- **Tóm tắt điểm chung từ 3 feedback:** 
  + Cả 3 tester đều từ chối hoặc khó chịu với cơ chế tự động can thiệp khi dừng video của Option B (bị xem là phiền toái hoặc lầm tưởng giao diện bị lag).
  + Xuất hiện sự phân hóa rõ nét: 2/3 tester (của Quyền và Dũng) chọn **Option C** vì giải quyết đúng nỗi đau gốc "không biết mình hổng chỗ nào" và thích được thử thách; trong khi 1/3 tester (của Hinh) chọn **Option A** vì ưu tiên tốc độ, quyền tự chủ cao và không muốn bị trắc nghiệm làm ngắt mạch học.
- **Group Next Change (Nhóm sẽ làm gì tiếp theo):** 
  + Chốt phát triển mô hình **Hybrid (User-led kết hợp On-demand AI Diagnostic)**: Lấy sơ đồ kiến thức của Option A làm khung mặc định (tôn trọng quyền tự chủ của người học), đồng thời tích hợp thêm nút *"AI Chẩn đoán nhanh"* (Option C) dưới dạng tùy chọn khi người học bối rối không biết mình hổng ở đâu.
  + Loại bỏ hoàn toàn cơ chế tự động nhảy gợi ý khi dừng video của Option B.
- **Điều chưa được chứng minh (Still Unproven):** 
  + Vẫn chưa thể kết luận khi sơ đồ kiến thức có 15–20 khái niệm phức tạp thì người học có còn tự tìm được ở Option A hay sẽ bị quá tải nhận thức.
  + Chưa kiểm chứng được độ tin cậy thực tế của 2 câu hỏi trắc nghiệm ngắn trong việc chẩn đoán chính xác nhiều loại lỗ hổng kiến thức khác nhau.
- 📄 Xem chi tiết tổng hợp 3 feedback của nhóm tại: [group-feedback-synthesis.md](group-feedback-synthesis.md)

## 6. AI Support Log
- **AI đã giúp gì:** Hỗ trợ tạo khung code giao diện web `prototype.html` với TailwindCSS, chuẩn hóa cấu trúc bảng quan sát Fact-First và hỗ trợ tổng hợp, đối chiếu 3 bộ dữ liệu phỏng vấn.
- **Điểm sai/hời hợt của AI:** Ban đầu AI đặt tên các nút chọn phương án mang tính định kiến cá nhân (`Quyen: User Control...`), đồng thời thiếu cơ chế kiểm soát / phục hồi (Control & Recovery) khi AI chẩn đoán sai ở Option C.
- **Cách tự sửa:** Đổi toàn bộ nhãn nút sang trung tính (Phương án A, B, C); bổ sung nút và hàm fallback cho phép người dùng tự chọn lại kiến thức khi AI chẩn đoán không chính xác.
- 📄 Xem nhật ký đầy đủ tại: [ai-support-log.md](ai-support-log.md)
