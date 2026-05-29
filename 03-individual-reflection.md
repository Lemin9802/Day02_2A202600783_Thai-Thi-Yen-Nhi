# Phase 7 — Individual Reflection

## 1. Tôi đã tham gia vào phần nào?

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng |
|---|---|---|
| Scan cá nhân | Lên danh sách 5 problems sát thực tế (bao gồm cả tối ưu quy trình code React/.NET và tối ưu lịch trình cá nhân). | Mang lăng kính đa dạng (từ kỹ thuật đến đời sống) vào nhóm. |
| Pitch Problem Card | Trình bày bài toán "Kế hoạch di chuyển HCM-HN tìm combo chỗ ở, gym, ăn". | Bài toán có tính thực tế và pain point cao nên đã được nhóm đồng thuận chọn làm Candidate chính để phát triển. |
| Validation / research | Chỉ ra khó khăn trong việc thu thập dữ liệu phi cấu trúc từ bài đăng Facebook, video TikTok. | Giúp nhóm xác định rõ AI Intervention Point nằm ở khâu "bóc tách thông tin". |
| Problem Statement | Đề xuất việc thiết lập ranh giới (Boundary) rõ ràng: Agent chỉ xếp hạng và cảnh báo rủi ro, không tự quyết định thuê. | Giới hạn được rủi ro lừa đảo (scam) vốn rất phổ biến trên MXH. |
| Rule / Workflow / Agent | Cùng nhóm phân tích và quyết định nâng lên mức Agent. | Xác định được các Tools cụ thể Agent cần gọi (Map/Route tool, Parser, Risk checker). |

## 2. Bảng dùng AI trong reflection

| Phase | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai/hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| Scan & Problem Card | Nhờ AI đóng vai "Skeptical PM" để phản biện điểm yếu của ý tưởng tìm trọ. | Chỉ ra rằng bước "cào" data từ FB/TikTok tự động là rất khó và lý tưởng hóa. | Đánh giá thấp giá trị của việc tiết kiệm chi phí so với thuê trên app. | Chỉnh lại luồng: Đưa phần gom text về Rule/Script hoặc user tự paste thay vì bắt AI tự động 100%. |
| Workflow | Dùng AI để chuyển luồng tư duy thành bản vẽ sơ đồ dạng Text/ASCII. | Căn chỉnh các bước vuông vức, thấy rõ điểm nghẽn (Bottleneck). | Có xu hướng gộp bước "Review" và "Liên hệ" làm một. | Tách rõ Human Boundary ở khâu liên hệ chủ nhà để chốt rủi ro. |
| Decision | Đối chiếu Rule vs Workflow vs Agent. | Gợi ý được các Tool mà Agent có thể gọi (Maps API). | Đề xuất Agent ôm đồm cả việc lên lịch hẹn tự động. | Cắt bỏ tính năng tự hẹn lịch, chỉ giữ Agent ở mức tạo Shortlist và cảnh báo rủi ro. |

## 3. Reflection câu hỏi mở

*   **Điều tôi học được từ bài toán của nhóm:** Ban đầu, tôi định hình bài toán của mình ở mức Workflow. Tuy nhiên, khi vào nhóm và mổ xẻ kỹ khâu tính toán di chuyển (phải dùng Google Routes API) kết hợp với đánh giá rủi ro (Risk checker), tôi nhận ra đây chính là đất diễn tuyệt vời cho Agent. Dữ liệu phi cấu trúc (teencode, viết tắt) trên MXH là nơi Rule thông thường hoàn toàn "bó tay", khẳng định rõ ràng AI Value.
*   **Điều tôi đóng góp cốt lõi:** Đưa ra bài toán gốc có impact đo lường được bằng thời gian cụ thể (từ 3-4 giờ lướt web xuống còn 30-45 phút).
*   **Nếu làm lại, tôi sẽ thay đổi điều gì:** Tôi sẽ challenge nhóm mạnh hơn ở phần "Agent Tools" — cụ thể là thu hẹp nguồn dữ liệu đầu vào. Việc bắt Agent tự động thu thập từ quá nhiều nguồn (cả web, FB, TikTok) có thể khiến MVP thất bại vì rác dữ liệu. Đáng lẽ nên chốt scope nhỏ hơn: "Người dùng copy paste link/text bài đăng vào để Agent phân tích" sẽ khả thi hơn trong thực tế vận hành.

## 4. Tự kiểm cuối bài

- [x] [12đ cá nhân] Cá nhân có 5+ problems và top 3 Problem Cards.
- [x] [12đ cá nhân] Tôi đã pitch rõ và challenge nhóm đúng trọng tâm.
- [x] [10đ cá nhân] Reflection cá nhân có nói rõ vai trò trong nhóm, cách dùng AI, điều học được và nếu làm lại sẽ đổi gì.
- [x] [6đ cá nhân] Tôi tự giải thích được mạch problem → workflow → metric → boundary → độ phù hợp với AI.