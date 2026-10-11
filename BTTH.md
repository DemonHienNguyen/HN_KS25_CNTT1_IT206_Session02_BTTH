## Phần 1: Kiến trúc Mô hình Vận hành

### 1.1. Phạm vi Áp dụng & Định hướng Đội Đối soát

Đội Đối soát không áp dụng mô hình Scrum thuần túy như hai đội Đặt xe và Thanh toán, mà vận hành theo mô hình Scrumban/Kanban tích hợp trong cùng một khung quản trị Agile chung của RikkeiGo. Lý do là công việc đối soát mang tính chất luồng vận hành liên tục (Continuous Flow), ưu tiên tính ổn định tuyệt đối và phải tuân thủ nghiêm ngặt lịch cố định của cơ quan thuế và ngân hàng, không phù hợp với việc đóng gói tính năng theo chu kỳ Sprint ngắn hạn.

### 1.2. Các Module Quy trình & Phân tách Trách nhiệm

| **Module**                   | **Đội Đặt xe & Thanh toán (Scrum)**                                                                                                                                                                                   | **Đội Đối soát (Scrumban / Kanban)**                                                                                                                                                                                                | **Nguyên tắc Tách bạch Trách nhiệm**                                                                                                                              |
| ---------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **3 Vai trò (Roles)**       | Product Owner:Quản lý Product Backlog, tối ưu giá trị sản phẩm<br />Scrum Master :Bảo vệ quy trình, tháo gỡ rào cản<br />Developers:Quyết định giải pháp kỹ thuật, cam kết Sprint                         | Operations PO / Lead:Quản lý hàng đợi công việc đối soát<br />Agile Coach / SM:Tối ưu luồng công việc (Flow) & WIP Limits<br />Operations Team:Thực thi kiểm tra, đối soát và xử lý sai lệch                           | PO quyết định**CÁI** GÌ làm trước; Team quyết định LÀM NHƯ THẾ NÀO ; SM/Coach duy trì QUY TRÌNH & KỶ LUẬT TIMEBOX Không chồng chéo chỉ đạo. |
| **3 Sản phẩm (Artifacts)** | Product Backlog: Hàng đợi tính năng ưu tiên theo ROI<br />Sprint Backlog:Hạng mục cam kết trong 2 tuần<br />Increment:Phần mềm đạt Definition of Done (DoD)                                                      | Service Backlog:Yêu cầu đối soát & báo cáo thuế<br />Kanban Board:Bảng luồng công việc kèm giới hạn WIP<br />Reconciliation Output:Báo cáo khớp 100% dữ liệu                                                               | Đảm bảo tính Minh bạch. Mọi kết quả đầu ra phải qua kiểm định Definition of Done (DoD) hoặc Checklist tuân thủ trước khi phát hành.                     |
| **5 Sự kiện (Events)**     | Sprint:Nhịp 2 tuần cố định.<br />Sprint Planning:Lập kế hoạch Sprint<br />Daily Scrum:15 phút đồng bộ mỗi ngày<br />Sprint Review: Demo và thu thập phản hồi<br />Sprint Retrospective: Cải tiến quy trình | Cadence Planning: Lập kế hoạch luồng tuần/tháng.<br />Daily Standup: 15 phút rà soát điểm nghẽn (Bottlenecks).<br />Service Review: Đánh giá SLA và tuân thủ thuế.<br />Retrospective: Cải tiến quy trình đối soát. | Thực thi Thanh tra (Inspection)& Thích nghi (Adaptation) . Các sự kiện có khung thời gian cố định (Timebox), không bị kéo dài tự do.                          |

### 1.3. Luồng Giá trị Khép kín (End-to-End Value Stream)

được vẽ trong gigido.drawio

## Phần 2: Xử lý Tình huống Ngoại lệ



### Tình huống 1: Đến buổi Sprint Review nhưng KHÔNG CÓ hạng mục nào đạt Definition of Done

* Nơi phát hiện: Tại sự kiện Sprint Review (cuối Sprint).
* Người xử lý:
  * Product Owner: Chủ trì quyết định nghiệm thu.
  * Scrum Master: Giám sát tính tuân thủ nguyên tắc Agile/Scrum.
  * Developers: Báo cáo thực trạng và các rào cản kỹ thuật.
* Cách xử lý chuẩn Agile:
  1. Nghiệm thu thực chất (PO): PO kiên quyết từ chối nghiệm thu tất cả các hạng mục chưa đạt 100% DoD
  2. Chuyển đổi mục tiêu buổi Review (SM & PO): Không hủy buổi Review.
  3. Trả hạng mục về Backlog (PO): Mọi công việc dở dang được đưa ngược lại Product Backlog.
  4. Phân tích nguyên nhân tại Retrospective (SM & Team): Ngay tại phiên Sprint Retrospective, team áp dụng kỹ thuật *5 Whys* để tìm nguyên nhân gốc rễ

### Tình huống 2: Đội Thanh toán muốn kéo dài riêng Sprint đang chạy thêm 1 tuần để "làm cho xong"

* Nơi phát hiện: Tại sự kiện Daily Scrum hoặc giữa Sprint khi Đội Thanh toán phát hiện nguy cơ trễ cam kết.
* Người xử lý:
  * Scrum Master (SM): Người bảo vệ nguyên tắc và kỷ luật khung thời gian (Timebox).
  * Product Owner (PO): Quản lý và điều chỉnh phạm vi sản phẩm.
* Cách xử lý chuẩn Agile:
  1. Từ chối kéo dài Sprint (SM): Scrum Master từ chối tuyệt đối đề xuất kéo dài Sprint
  2. Cắt giảm phạm vi trong Sprint: PO làm việc với Developers để cắt giảm phạm vi (Descope) các hạng mục chưa chạm đến hoặc không tối quan trọng
  3. Đóng Sprint đúng hạn: Sprint kết thúc đúng lịch 2 tuần. Những hạng mục chưa xong được đưa trả về Product Backlog để PO xem xét cho Sprint sau
  4. Rút kinh nghiệm tại Retrospective: Đội Thanh toán phân tích lý do ước lượng sai hoặc phạm vi phình to
