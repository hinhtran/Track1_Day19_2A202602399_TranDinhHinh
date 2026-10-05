# 3. Mẫu Phiếu Ghi Nhận Phản Hồi Cá Nhân (Prototype Feedback Note)

*Mỗi thành viên trong nhóm bắt buộc phải tự tay hoàn thành một bản này cho phiên kiểm thử do chính mình điều phối:*

**Họ tên cá nhân:** Trần Đình Hinh - MHV: 2A202602399  
**Họ tên tester:** Dương Hải Minh - MHV: 2A202602680
**Tester / Bối cảnh:** Sinh viên IT đang tự học video bài giảng lập trình trực tuyến, gặp đoạn khó hiểu cần gỡ rối kiến thức nền.

---

### Bảng quan sát hành vi (Fact-First)

| Tiêu điểm quan sát hành vi | Ghi chép chi tiết hành vi thực tế (Fact-First) |
| :--- | :--- |
| **First Action (Hành động đầu tiên):** Tester bấm vào đâu, nhìn vào đâu đầu tiên? | Tester bấm ngay vào nút đỏ **"🤯 Tôi không hiểu đoạn này!"** ở Phương án A, mắt nhìn lướt nhanh sơ đồ các node kiến thức xuất hiện trong popup để tìm chủ đề liên quan. |
| **Hesitation (Điểm do dự, dừng lại hoặc hiểu sai):** Chỗ nào khiến tester lúng túng hoặc hiểu lầm? | - **Ở Phương án B:** Tester bấm dừng video nhưng không nhận thấy sidebar bên phải thay đổi; sau 3 giây gợi ý mới hiện ra khiến tester tưởng giao diện bị lag/đơ.<br>- **Ở Phương án C:** Khi popup hiện câu hỏi trắc nghiệm, tester khựng lại đọc đề, hơi ngập ngừng và cảm thấy bị "ngắt mạch học". |
| **Evidence Checking (Minh chứng được đọc hay bỏ qua):** Tester có kiểm tra nguồn trích dẫn / cảnh báo không? | Bỏ qua phần giải thích chi tiết trong popup Option C; chỉ đọc lướt định nghĩa ngắn gọn xuất hiện khi click trực tiếp vào node "Kiểu dữ liệu" ở Option A. |
| **Control & Recovery (Cách sửa sai hoặc lấy lại quyền kiểm soát):** Tester dùng nút nào để khắc phục khi thấy kết quả chưa ưng ý? | Ở Option A, sau khi đọc xong định nghĩa, tester lập tức bấm nút **"Quay lại video"** để tiếp tục học. Ở Option C, tester nhận thấy có nút fallback *"AI chẩn đoán chưa đúng? Tự chọn phần cần xem lại"* nhưng chia sẻ rằng thích tự chọn ngay từ đầu hơn là phải đợi AI chẩn đoán rồi mới sửa sai. |
| **Selected Option (Phương án được tester lựa chọn):** | **Option A (User-led / User Control)** |
| **Trade-offs (Lý do chọn và sự đánh đổi chấp nhận):** Tester sẵn sàng hy sinh điều gì để chọn phương án này? | - **Lý do:** Tester cảm thấy hoàn toàn chủ động trong việc tìm kiếm kiến thức, tự quyết định mình cần ôn lại phần nào mà không bị AI can thiệp ép buộc.<br>- **Đánh đổi chấp nhận:** Chấp nhận phải tự tư duy, tự phán đoán xem mình đang hổng ở khái niệm nào (tốn chút nỗ lực tự nhận thức) thay vì có AI tự động chỉ điểm sẵn. |
| **Counter-evidence (Dữ kiện đi ngược lại kỳ vọng ban đầu của nhóm):** Có phát hiện nào bất ngờ làm nhóm 'vỡ mộng'? | Nhóm từng kỳ vọng Option C (AI Diagnostic Quiz) sẽ gây ấn tượng mạnh nhất vì "thông minh và tự động hóa cao", nhưng tester thực tế lại thấy cơ chế quiz trắc nghiệm là rườm rà, "sáng tạo nhưng hơi dài dòng", vô tình tạo thêm bài tập khi đang muốn giải quyết nhanh khúc mắc. |

---

### Bóc tách 4 Tầng Tư Duy Sư Phạm (The 4 Cognitive Layers)

*Sau khi phiên test kết thúc, hãy phân loại ghi chép thành 4 tầng rõ rệt:*

- **1. OBSERVED (Quan sát khách quan thuần túy):** 
  - Tester thử Phương án A và nhận xét: *"Mình thích cách này vì mình được chủ động tìm kiếm kiến thức đúng chỗ mình chưa rõ, không bị phụ thuộc"*.
  - Tester thử Phương án B và nhận xét: *"Cái này chưa nổi bật lắm, nếu không để ý thì mình không biết là AI đang gợi ý cho mình"*.
  - Tester thử Phương án C, hoàn thành 2 câu quiz rồi nhận xét: *"Cách này thấy sáng tạo nhưng mà hơi dài dòng một chút, đang học mà phải làm thêm trắc nghiệm thì hơi ngại"*.
  - Thời gian từ lúc mở trợ giúp đến khi quay lại video ở Phương án A là nhanh nhất (~10 giây).

- **2. INTERPRETED (Diễn giải nhận định của người làm sản phẩm):** 
  - **Tâm lý cần quyền tự chủ (Sense of Agency):** Người học ưu tiên cao cảm giác tự kiểm soát quá trình học hơn là để AI quyết định thay.
  - **Gánh nặng nhận thức phụ (Secondary Cognitive Load):** Cơ chế 2 câu hỏi trắc nghiệm của Option C vô tình tạo cảm giác "bị kiểm tra/thi cử", làm đứt gãy sự tập trung vào bài học chính.
  - **Tín hiệu tương tác của Option B quá yếu (Weak Affordance):** Cơ chế tự động kích hoạt khi dừng video chưa đủ rõ ràng để người dùng nhận biết được giá trị hỗ trợ của AI.

- **3. DECIDED — NEXT CHANGE (Quyết định hành động cụ thể cho vòng sau):** 
  - **Lấy Option A làm nền tảng chính:** Giữ nguyên sơ đồ kiến thức để người học tự do khám phá và làm chủ.
  - **Tích hợp ưu điểm gợi ý của Option B vào sơ đồ A:** Khi người học bấm mở sơ đồ ở Option A, AI chỉ đánh dấu viền sáng nhẹ (subtle highlight) kèm nhãn gợi ý *"Khả năng cao bạn cần xem lại phần này"* để định hướng, nhưng không ép buộc và không che khuất các phần khác.
  - **Đơn giản hóa Option C thành tính năng phụ:** Chuyển bài quiz chẩn đoán thành tùy chọn phụ ("Bạn không chắc mình hổng ở đâu? Nhờ AI hỏi nhanh") thay vì ép người dùng làm trắc nghiệm bắt buộc.

- **4. STILL UNPROVEN (Điều vẫn chưa thể chứng minh):** 
  - Chưa chứng minh được liệu khi bài giảng trở nên cực kỳ phức tạp (sơ đồ có trên 10-15 khái niệm liên quan), người học có còn tự tin tự xác định đúng lỗ hổng ở Option A hay không, hay lúc đó sẽ bị quá tải thông tin và cần đến sự chẩn đoán tự động của Option C.
  - Cần thêm dữ liệu thử nghiệm trên đối tượng người học mới bắt đầu (novice/mất gốc hoàn toàn) để xem mức độ hiệu quả của từng phương án.
