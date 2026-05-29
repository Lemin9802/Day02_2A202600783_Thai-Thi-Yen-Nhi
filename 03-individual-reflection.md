# Phase 7 — Individual Reflection

## 1. Tôi đã tham gia vào phần nào?

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng |
|---|---|---|
| Scan cá nhân | Lên danh sách 5 problems sát thực tế (bao gồm tối ưu quy trình code React/.NET và tối ưu lịch trình cá nhân). | Mang lăng kính đa dạng vào buổi thảo luận nhóm. |
| Pitch Problem Card | Trình bày bài toán "Kế hoạch di chuyển HCM-HN tìm combo chỗ ở, gym, ăn". | Ý tưởng gốc của tôi bị nhóm từ chối vì scope quá rộng, nhưng nhóm đã dùng nó làm nền tảng để tinh chỉnh thành bài toán chốt: "Agent tìm phòng trọ tối ưu". |
| Validation / research | Chia sẻ rủi ro về độ phức tạp khi thu thập dữ liệu phi cấu trúc từ Facebook/TikTok. | Giúp nhóm đánh giá đúng độ khó của đầu vào, từ đó quyết định loại bỏ phần tìm "combo ăn/gym" để thu hẹp scope. |
| Problem Statement | Hỗ trợ định hình lại workflow và xây dựng các success metrics (thời gian, số lượng tin). | Đảm bảo giữ được linh hồn của bài toán gốc là giảm thời gian từ 3-4 giờ lướt web xuống còn 30-45 phút. |
| Rule / Workflow / Agent | Phân tích sự cần thiết của Agent khi cần kết hợp Map API và Risk Checker. | Cùng nhóm thống nhất chọn Agent làm hướng đi cuối cùng thay vì Workflow tuyến tính. |

## 2. Bảng dùng AI trong reflection

| Phase | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai/hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| Scan & Problem Card | Nhờ AI đóng vai "Skeptical PM" để phản biện điểm yếu của ý tưởng cá nhân. | AI chỉ ra cực kỳ chính xác rằng việc tự động cào data từ FB/TikTok là điểm yếu chí mạng. Nhờ đó, tôi không bị bất ngờ khi nhóm từ chối bài của mình với lý do tương tự. | Đánh giá thấp giá trị của việc tiết kiệm chi phí so với thuê trên app đặt phòng. | Tôi vui vẻ đồng ý với nhóm: Cắt bỏ các yêu cầu phụ (gym, ăn) để tập trung giải quyết triệt để phần tìm phòng trọ. |
| Workflow | Dùng AI để chuyển luồng tư duy thành bản vẽ ASCII. | Căn chỉnh các bước vuông vức, thấy rõ điểm nghẽn (Bottleneck). | AI thường có xu hướng gộp bước "Review" và "Liên hệ" của người dùng. | Tách rõ Human Boundary ở khâu liên hệ chủ nhà để chốt rủi ro. |
| Decision | Đối chiếu Rule vs Workflow vs Agent. | Gợi ý được các Tool mà Agent có thể gọi (như Maps API để tính commute score). | AI (khi đóng vai Agent) hay ảo tưởng sức mạnh ôm cả việc chốt cọc thay người dùng. | Cùng nhóm thiết lập Boundary chặt chẽ: Agent chỉ chấm điểm, người dùng tự xác minh. |

## 3. Reflection câu hỏi mở

*   **Điều tôi học được từ bài toán của nhóm:** Bài toán cá nhân của tôi ban đầu định hình ở mức Workflow. Tuy nhiên, khi ghép vào nhóm và nhận feedback (cả từ AI Skeptical PM lẫn đồng đội), tôi nhận ra việc thu thập data MXH là quá sức cho Workflow thông thường. Nhóm đã tinh chỉnh thành Agent kết hợp gọi Maps API và chấm điểm rủi ro. Đây là bài học lớn về sự "thỏa hiệp" để có một Problem Statement khả thi và sắc bén hơn.
*   **Điều tôi đóng góp cốt lõi:** Dù ý tưởng gốc (tìm combo nhà + gym + ăn) phải thu hẹp lại, nhưng tôi đã cung cấp được bối cảnh (context) đau đớn thực tế và metric đo lường thời gian (từ 3-4 giờ xuống 30-45 phút) để nhóm xây dựng thành công Problem Statement cuối cùng.
*   **Nếu làm lại, tôi sẽ thay đổi điều gì:** Tôi sẽ challenge nhóm kỹ hơn ở khâu thiết kế **"Search/listing collector tool"** của Agent. Nhóm đang kỳ vọng Agent tự đi gom tin đăng từ FB/TikTok, nhưng rủi ro rác dữ liệu vẫn rất cao. Đáng lẽ nên chốt scope nhỏ hơn: *"Người dùng copy link/text paste vào để Agent phân tích"* thì sẽ an toàn và dễ validate hơn trong MVP.

## 4. Tự kiểm cuối bài

- [x] [12đ cá nhân] Cá nhân có 5+ problems và top 3 Problem Cards.
- [x] [12đ cá nhân] Tôi đã pitch rõ và challenge nhóm đúng trọng tâm.
- [x] [10đ cá nhân] Reflection cá nhân có nói rõ vai trò trong nhóm, cách dùng AI, điều học được và nếu làm lại sẽ đổi gì.
- [x] [6đ cá nhân] Tôi tự giải thích được mạch problem → workflow → metric → boundary → độ phù hợp với AI.