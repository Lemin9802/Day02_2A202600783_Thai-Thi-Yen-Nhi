# Phase 1 - Individual Scan: Tìm 5+ problems

## Bảng scan

| #   | Lăng kính                        | Problem quan sát được                                                                                                                                                                                             | Ai đang đau?                 | Dấu hiệu thật                                                                                                                             |
| --- | -------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------- |
| 1   | Tốn thời gian, AI có thể tốt hơn | Lên kế hoạch di chuyển và sinh hoạt (vé xe/máy bay, chỗ ở, chỗ ăn, phòng gym) khi từ HCM ra Hà Nội học AI thực chiến. Phải tự đọc review, so sánh giá và khớp vị trí trên bản đồ từ nhiều nguồn nền tảng rời rạc. | Học viên / Người đi công tác | Mất 2-3 buổi tối mở hàng chục tab để tìm kiếm, đối chiếu và chốt lịch trình; dễ chọn sai vị trí gây bất tiện cho việc di chuyển mỗi ngày. |
| 2   | Lặp lại, Tốn thời gian           | Tinh chỉnh mô tả đồ án tốt nghiệp và kinh nghiệm thực tập để khớp với các keyword của từng Job Description khác nhau khi ứng tuyển vị trí Fresher / Trainee.                                                      | Ứng viên tìm việc            | Tốn 30-45 phút cho mỗi công ty để copy/paste, sửa từ khóa cho phù hợp và kiểm tra lại format CV.                                          |
| 3   | Lặp lại                          | Khởi tạo boilerplate code, cập nhật endpoint API và viết tài liệu đồng bộ giữa frontend React và backend .NET mỗi khi hệ thống có thêm tính năng mới.                                                             | Full-stack Developer         | Lặp lại mỗi lần đổi logic; tốn 15-20 phút gõ code lặp đi lặp lại và dễ bị miss field dẫn đến lỗi tích hợp.                                |
| 4   | AI có thể tốt hơn                | Đọc file log lỗi và làm sạch dữ liệu thô (thông số bị nhiễu) từ cảm biến môi trường truyền về hệ thống Raspberry Pi trước khi đưa vào phân tích.                                                                  | Kỹ sư phần mềm / IoT         | Mất thời gian mò mẫm trong các dòng log text dài mỗi khi phần cứng gửi dữ liệu sai lệch do môi trường vật lý.                             |
| 5   | Tốn thời gian                    | Tìm kiếm, tổng hợp và phân loại các đề thi thử, tài liệu ôn tập THPTQG từ nhiều group, diễn đàn, và xác minh lại các thông tin quy định hành chính cập nhật về một nơi để theo dõi.                               | Học sinh / Thí sinh          | Tốn 1-2 tiếng mỗi tuần chỉ để gom link, tải file và check chéo thông tin; nhiều tài liệu tải về bị thiếu hệ thống.                        |

# Phase 2 — Top 3 Problem Cards + draft workflow

## Chọn top 3

| Rank | Problem                            | Vì sao chọn                                                                                 | Điều còn chưa chắc                                                   |
| ---- | ---------------------------------- | ------------------------------------------------------------------------------------------- | -------------------------------------------------------------------- |
| 1    | Kế hoạch di chuyển HCM-HN học AI   | Trải nghiệm thật, workflow gom nhặt thông tin cực kỳ tốn thời gian, đo lường được ngay.     | Dữ liệu review, giá cả trên web có được AI thu thập chính xác không. |
| 2    | Tinh chỉnh CV theo Job Description | Phù hợp năng lực tóm tắt, đối chiếu ngữ nghĩa của ngôn ngữ (LLM). Rất sát thực tế tìm việc. | AI có thể "bịa" thêm kinh nghiệm nếu prompt không chặt.              |
| 3    | Đồng bộ API React & .NET           | Workflow tuyến tính rất rõ ràng, điểm nghẽn là việc gõ boilerplate code nhàm chán.          | Có thể chỉ cần dùng Rule/Tool gen code thay vì cần tới AI.           |

---

## Problem Card #1: Kế hoạch di chuyển HCM-HN

**Problem 1 câu:**
Mỗi học viên đi học AI xa nhà (từ HCM ra HN), học viên mất rất nhiều thời gian lên lịch trình sinh hoạt (phòng ở, chỗ ăn, phòng gym) do phải tự bơi trong làn sóng thông tin từ Google, hội nhóm Facebook, video TikTok để tìm phòng giá rẻ (tránh phí cao trên Booking/Agoda), rồi lại phải tự đối chiếu vị trí địa lý xem có gần chỗ học không.

**Actor:**
Học viên chương trình AI thực chiến/Người đi công tác ngắn ngày tối ưu chi phí.

**Thời điểm/bối cảnh:**
Vài tuần trước khi bắt đầu khóa học tại Hà Nội.

**Current workflow 3-7 bước:**
1. Xác định địa chỉ nơi học tập tại Hà Nội.
2. Lên Google Search, vào các hội nhóm Facebook tìm bài đăng cho thuê phòng trọ/căn hộ giá rẻ, hoặc lướt TikTok xem review chỗ ăn uống, phòng gym quanh khu vực đó.
3. Chat/Inbox hỏi giá, kiểm tra xem phòng còn trống không.
4. Mở Google Maps để ghim thử các địa chỉ tìm được từ FB/TikTok, đối chiếu khoảng cách xem có bị quá xa nơi học hoặc có nằm ở cung đường hay kẹt xe không.
5. So sánh giá, lọc review khen chê thực tế từ bình luận của cộng đồng để tránh dính "phốt".
6. Chốt phương án và lưu vào Note/Google Sheets.

**Bottleneck:**
Bước 2, 4 và 5 - Lướt hàng trăm bài viết, bình luận trên Facebook/TikTok và mở mười mấy tab Google Maps để tự sàng lọc thông tin thủ công, đối chiếu vị trí địa lý và kiểm tra độ uy tín (mất hơn 150 phút).

**Impact:**
Mất tổng cộng 2-3 buổi tối (khoảng 3-4 tiếng) vô cùng mệt mỏi mà vẫn có rủi ro bị lừa cọc phòng trên Facebook, hoặc dính phải phòng chất lượng tệ do bài review ảo trên TikTok.

**Success metric:**
Giảm tổng thời gian tìm kiếm và chốt lịch trình từ 180 phút xuống dưới 40 phút. Chi phí thuê chỗ ở tiết kiệm hơn 20-30% so với đặt trực tiếp trên Agoda/Booking. Khoảng cách di chuyển giữa các địa điểm không quá 2km.

**Non-AI alternative:**
Chấp nhận chi phí cao để đặt phòng qua Agoda/Booking cho an toàn và nhanh, hoặc ở ký túc xá/nhà người quen (nếu có).

**AI hypothesis:**
AI đóng vai trò bộ lọc ngôn ngữ lớn: Nhập dữ liệu đầu vào là các đoạn văn bản (text bài đăng cho thuê trên Facebook, transcript video TikTok, kết quả Google Search), AI sẽ tự động bóc tách (Extract) ra các trường dữ liệu: Địa chỉ, Giá cả, Tiện ích (có gần gym không), Ưu điểm, Nhược điểm (Phốt nếu có từ comment) và vẽ thành bảng so sánh cho người dùng.

**Quick gut:**
[ ] No AI/process fix
[ ] Rule (Rule không thể đọc hiểu các bài đăng tự do trên Facebook)
[x] Workflow (Dùng script gom text/API Search -> Dùng AI bóc tách cấu trúc dữ liệu -> Người chọn)
[ ] Agent
[ ] Chưa biết

### Draft current workflow

CURRENT STATE - 180 phút

┌──────────────┐   ┌──────────────┐   ┌──────────────┐   ┌──────────────┐
│ 1 Nhập địa   │   │ 2 Lội FB,    │   │ 3 Ghim Maps  │   │ 4 Đọc comment│
│ chỉ học      │ → │ lướt TikTok  │ → │ check khoảng │ → │ đối chiếu giá│
│ ⏱ 5'        │   │ ⏱ 60'        │   │ cách ⏱ 30'  │   │ ⏱ 60' 🔴    │
└──────────────┘   └──────────────┘   └──────────────┘   └──────────────┘
                                                                │
                                                                ▼
                                                         ┌──────────────┐
                                                         │ 5 Chốt lịch  │
                                                         │ & lưu Sheet  │
                                                         │ ⏱ 25'        │
                                                         └──────────────┘

🔴 = Bottleneck


###Draft future workflow

FUTURE STATE - 35 phút

┌──────────────┐   ┌──────────────┐   ┌──────────────┐
│ 1 Nhập địa   │   │ 2 Tool gom   │   │ 3 AI bóc     │
│ chỉ & budget │ → │ text FB/Web  │ → │ tách data,   │
│ ⏱ 2'        │   │ ⏱ 5'         │   │ review ⏱ 3' │
└──────────────┘   └──────────────┘   └──────────────┘
                                              │
                                              ▼
                   ┌──────────────┐   ┌──────────────┐
                   │ 5 Duyệt &    │   │ 4 AI xuất    │
                   │ liên hệ      │ ← │ bảng 3 combo │
                   │ ⏱ 20' 🟢    │   │ ⏱ 5'        │
                   └──────────────┘   └──────────────┘

🟢 = Human boundary
Fallback: AI bóc tách sai/thiếu → Người dùng tự click link check lại.
Bottleneck mới: Người dùng duyệt & liên hệ - chấp nhận được vì là điểm kiểm soát rủi ro.

---

## Problem Card #2: Tinh chỉnh CV theo Job Description

**Problem 1 câu:**
Ứng viên Fresher/Trainee mất nhiều thời gian viết lại mô tả đồ án tốt nghiệp và kinh nghiệm thực tập (ví dụ tại Alta) để khớp keyword của từng Job Description (JD) mỗi khi apply công ty mới.

**Actor:**
Ứng viên (như Full-stack/AI Trainee).

**Thời điểm/bối cảnh:**
Mỗi khi chuẩn bị nộp hồ sơ xin việc vào một JD mới.

**Current workflow 3-7 bước:**
1. Đọc JD để nhặt keyword (VD: cần .NET, React, IoT, AI).
2. Mở file Master CV (Word/Docs).
3. Viết lại phần mô tả kinh nghiệm/dự án cho khớp các keyword.
4. Căn chỉnh lại format cho không bị tràn trang.
5. Xuất PDF và nộp.

**Bottleneck:**
Bước 3 - Cố gắng viết lại câu chữ mô tả sao cho tự nhiên, vừa đúng sự thật vừa chứa đủ keyword của JD (tốn 25 phút).

**Impact:**
Mất khoảng 30-45 phút cho mỗi bản CV. Gây mệt mỏi, dẫn đến việc ứng viên thường nộp đại 1 CV chung chung cho mọi công ty và dễ rớt từ vòng lọc hồ sơ.

**Success metric:**
Giảm thời gian tinh chỉnh một bản CV xuống dưới 10 phút; nội dung xuất ra không chứa thông tin bịa đặt (hallucination).

**Non-AI alternative:**
Tạo sẵn 3 bản CV template theo 3 hướng (Front-end, Back-end, AI) rồi lấy ra xài dần, bớt phải sửa nhiều.

**AI hypothesis:**
AI nhận đầu vào là Master CV và văn bản JD, đối chiếu keyword và tự động draft lại các gạch đầu dòng mô tả dự án. Người dùng chỉ cần review và export.

**Quick gut:**
[ ] No AI/process fix
[ ] Rule
[x] Workflow
[ ] Agent
[ ] Chưa biết

### Draft current workflow

CURRENT STATE - 40 phút

┌──────────────┐   ┌──────────────┐   ┌──────────────┐
│ 1 Đọc phân   │   │ 2 Mở Master  │   │ 3 Viết lại   │
│ tích JD      │ → │ CV (Word)    │ → │ mô tả khớp   │
│ ⏱ 5'         │   │ ⏱ 2'        │  │ keyword ⏱ 25'🔴│
└──────────────┘   └──────────────┘   └──────────────┘
                                              │
                                              ▼
                   ┌──────────────┐   ┌──────────────┐
                   │ 5 Export PDF │   │ 4 Sửa lỗi    │
                   │ & nộp        │ ← │ typo & format│
                   │ ⏱ 3'         │   │ ⏱ 5'        │
                   └──────────────┘   └──────────────┘

🔴 = Bottleneck


###Draft future workflow

FUTURE STATE - 12 phút

┌──────────────┐   ┌──────────────┐   ┌──────────────┐
│ 1 Copy JD &  │   │ 2 AI phân    │   │ 3 AI draft   │
│ CV vào AI    │ → │ tích keyword │ → │ bullet points│
│ ⏱ 2'         │  │ JD ⏱ 1'      │   │ ⏱ 2'        │
└──────────────┘   └──────────────┘   └──────────────┘
                                              │
                                              ▼
                   ┌──────────────┐   ┌──────────────┐
                   │ 5 Update CV  │   │ 4 Ứng viên   │
                   │ & Export PDF │ ← │ review & edit│
                   │ ⏱ 2'        │   │ ⏱ 5' 🟢     │
                   └──────────────┘   └──────────────┘

🟢 = Human boundary
Fallback: AI draft ảo/bịa thông tin -> Ứng viên tự gõ lại dựa trên CV gốc.

## Problem Card #3: Đồng bộ API React và .NET

**Problem 1 câu:**
Mỗi khi cập nhật logic API ở backend .NET, Dev tốn thời gian viết lại boilerplate code (type/interface, fetch function) sang frontend React.

**Actor:**
Full-stack Developer.

**Thời điểm/bối cảnh:**
Khi có thay đổi, thêm bớt trường dữ liệu ở tính năng mới trong quá trình phát triển dự án.

**Current workflow 3-7 bước:**
1. Đổi code logic ở .NET controller.
2. Chạy lại Swagger để xem format JSON thay đổi.
3. Mở project React, tạo file/sửa interface (TypeScript).
4. Viết lại hàm fetch/axios gọi API.
5. Chạy test tích hợp UI.

**Bottleneck:**
Bước 3 và 4 - Gõ lại các trường dữ liệu bằng tay một cách nhàm chán, cực kỳ dễ gõ sai tên trường (typo) gây lỗi mismatch dữ liệu (mất khoảng 15 phút).

**Impact:**
Tốn 20-30 phút mỗi lần đổi API, dễ bị lỗi `undefined` ở UI, làm đứt gãy luồng suy nghĩ và kéo dài thời gian hoàn thiện tính năng.

**Success metric:**
Giảm thời gian đồng bộ code từ 25 phút xuống dưới 3 phút; 0 lỗi typo sai tên trường dữ liệu.

**Non-AI alternative:**
Dùng các công cụ sinh code tự động bằng Rule (như Swagger Codegen, OpenAPI Generator). 

**AI hypothesis:**
Copy file JSON từ định dạng Swagger dán vào AI, yêu cầu AI sinh ra chính xác code TypeScript interface và custom hook (ví dụ React Query hoặc Axios hook) để copy ngược lại vào project.

**Quick gut:**
[ ] No AI/process fix
[x] Rule (Công cụ gen code bằng Rule vốn đã làm rất tốt)
[x] Workflow (Dùng AI thay thế công cụ gen code cho các trường hợp custom nhanh)
[ ] Agent
[ ] Chưa biết

### Draft current workflow

CURRENT STATE - 25 phút

┌──────────────┐   ┌──────────────┐   ┌──────────────┐
│ 1 Đổi .NET   │   │ 2 Check      │   │ 3 Gõ lại TS  │
│ Controller   │ → │ Swagger JSON │ → │ Interface    │
│ ⏱ 5'        │   │ ⏱ 2'         │   │ ⏱ 10' 🔴    │
└──────────────┘   └──────────────┘   └──────────────┘
                                              │
                                              ▼
                   ┌──────────────┐   ┌──────────────┐
                   │ 5 Test UI &  │   │ 4 Viết hàm   │
                   │ Fix typo     │ ← │ gọi Axios    │
                   │ ⏱ 3'        │   │ ⏱ 5'        │
                   └──────────────┘   └──────────────┘

🔴 = Bottleneck

###Draft future workflow

FUTURE STATE - 7 phút

┌──────────────┐   ┌──────────────┐   ┌──────────────┐
│ 1 Đổi .NET   │   │ 2 Paste JSON │   │ 3 AI gen TS  │
│ Controller   │ → │ vào prompt   │ → │ Interface +  │
│ ⏱ 5'        │   │ AI ⏱ 1'      │   │ fetch ⏱ 1'  │
└──────────────┘   └──────────────┘   └──────────────┘
                                              │
                                              ▼
                                      ┌──────────────┐
                                      │ 4 Dev check &│
                                      │ paste project│
                                      │ ⏱ 0' 🟢     │
                                      └──────────────┘

🟢 = Human boundary
Fallback: AI sinh code sai format -> Dev dùng tool Rule (Swagger Codegen) hoặc tự gõ lại.

## Chọn card muốn pitch nhất

Card tôi muốn pitch nhất:
Problem Card #1: Kế hoạch di chuyển HCM-HN học AI (Tìm combo chỗ ở rẻ, phương tiện di chuyển, ăn uống, gym,... qua các trang MXH  theo định vị học tập).

Vì sao:
Bài toán này đánh trúng tâm lý tối ưu chi phí của học viên (không muốn dùng app đắt đỏ như Agoda). Điểm mấu chốt là công cụ Rule truyền thống không thể hiểu được ngôn ngữ tự do trên FB/TikTok, nhưng AI lại làm rất xuất sắc việc bóc tách dữ liệu phi cấu trúc này. Workflow rõ ràng, dấu hiệu đau cụ thể (tốn 3-4 tiếng lướt web) và metric trước/sau cực kỳ dễ so sánh.

Câu hỏi tôi muốn nhóm challenge:
Làm sao để thiết kế phần Data Collection đầu vào từ FB/TikTok một cách đơn giản nhất (ví dụ: dùng tool cào text hay copy tay) để AI xử lý mượt mà mà không làm toàn bộ workflow bị phức tạp hóa hay dính rác dữ liệu?
