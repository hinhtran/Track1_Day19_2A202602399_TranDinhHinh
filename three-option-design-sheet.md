# Three Option Design Sheet

## 1. Solution Mechanism (Dựa trên Prerequisite Map)
- **Option A:** User chủ động bấm nút "Tạo Sơ đồ". AI vẽ sơ đồ. User tự nhìn, phán đoán và click vào chỗ hổng.
- **Option B:** Sơ đồ luôn hiện. AI theo dõi thời gian dừng video, tự động highlight nhấp nháy vị trí nghi ngờ hổng và hỏi "Có phải bạn kẹt ở đây?". User xác nhận.
- **Option C:** User bấm "Không hiểu bài". AI cho làm 2 câu trắc nghiệm. Dựa vào kết quả, AI tự động chỉ thẳng vị trí hổng trên sơ đồ và hiện giải thích.

## 2. Human-AI Decision Table

| Human–AI decision | Option A (User phán đoán) | Option B (AI gợi ý) | Option C (AI chẩn đoán) |
| --- | --- | --- | --- |
| **User làm gì? AI làm gì?** | User tự xác định vị trí. AI chỉ vẽ sơ đồ. | AI gợi ý vị trí. User xác nhận Yes/No. | AI test và chẩn đoán bệnh. User học lại. |
| **AI Act / Ask / Don't Act? Vì sao?** | Don't Act. (AI không đưa ra kết luận để User toàn quyền). | Ask. (Hỏi để User xác nhận). | Act. (Hành động luôn dựa trên kết quả test). |
| **User hiểu capability/limit bằng gì?** | Bằng việc thấy toàn bộ sơ đồ và tự biết đây chỉ là bản đồ. | Bằng câu hỏi xác nhận của AI (AI không chắc chắn 100%). | Bằng việc thấy bài test 2 câu của AI. |
| **Evidence/uncertainty được thể hiện thế nào?** | Không có (Vì AI không đoán). | Hiệu ứng nhấp nháy + Dấu chấm hỏi (?). | Cột điểm/Kết quả test hiện ra. |
| **User kiểm soát và recovery thế nào?** | Chọn sai thì tự bấm sang node khác. | Bấm "Bỏ qua gợi ý, để tôi tự tìm". | Bấm "Bài test sai rồi, cho tôi bỏ qua". |
