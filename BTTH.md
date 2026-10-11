### Lý do chọn Agile thay vì Waterfall

* Waterfall thất bại vì: Yêu cầu bị chốt cứng từ đầu, khách hàng chỉ thấy sản phẩm cuối cùng. Khi nhu cầu của 30 siêu thị thay đổi, chi phí và thời gian sửa đổi là quá lớn
* Agile giải quyết bằng cách: Chia nhỏ dự án thành từng chu kỳ ngắn (Sprint), bàn giao sản phẩm dùng được liên tục để nhận phản hồi và điều chỉnh kịp thời

### Nguyên tắc làm việc (Đổi mới theo 4 giá trị Agile)

* Thay vì chỉ nhắn tin/bình luận: Họp trao đổi trực tiếp ngắn gọn hằng ngày (Daily Scrum)
* Thay vì viết tài liệu quá chi tiết: Tập trung làm sản phẩm chạy được và demo cho khách hàng sau mỗi Sprint
* Thay vì chờ 2 tuần duyệt hợp đồng khi đổi yêu cầu: Lắng nghe và điều chỉnh linh hoạt Backlog cùng đại diện GreenMart
* Thay vì cố bám kế hoạch cũ: Sẵn sàng thay đổi ưu tiên công việc dựa trên phản hồi thực tế

### Khung Scrum & 3 Trụ cột

Độ dài Sprint: 2 tuần (Tổng 3 Sprints trong 6 tuần).

#### Ứng dụng 3 trụ cột:

| Tru cột    | Nội dung                                                                |
| ----------- | ------------------------------------------------------------------------ |
| Minh bạch  | Bảng công việc và tiến độ rõ ràng cho cả team và GreenMart    |
| Thanh tra   | Đánh giá sản phẩm chạy được sau mỗi 2 tuần (Sprint Review)    |
| Thích nghi | Điều chỉnh kế hoạch Sprint tiếp theo ngay khi có phản hồi mới  |

#### Phân vai Scrum Team

| Trụ cột     | Người phụ trách                  | Được quyền                                                                 | Không được                                                                 |
| ------------- | ------------------------------------ | ------------------------------------------------------------------------------ | ------------------------------------------------------------------------------ |
| Product Owner | Long                                 | Thứ tự ưu tiên tính năng, nghiệm thu sản phẩm                         | Ép khối lượng công việc lên Dev Team hoặc can thiệp kỹ thuật        |
| Scrum Master  | Hoa                                  | Quy trình vận hành Scrum, tháo gỡ rào cản cho đội                     | Phân công việc cá nhân hoặc quyết định thứ tự ưu tiên tính năng |
| Developers    | An, Bình, Chi - Dev; Dung - Tester  | Giải pháp kỹ thuật, ước lượng thời gian, tự phân công công việc  | Tự ý đổi ưu tiên nghiệp vụ hoặc hạ thấp tiêu chuẩn chất lượng  |

### Artifacts & Lịch sự kiện (6 tuần đầu)

#### Product Backlog (Sắp xếp ưu tiên):

* Đăng nhập / Đăng ký tài khoản
* Tìm kiếm và lọc sản phẩm
* Xem thông tin tồn kho thời gian thực tại các chi nhánh
* Quản lý giỏ hàng trực tuyến
* Thanh toán trực tuyến (Ví/Thẻ)
* Quản lý trạng thái đơn hàng

#### Sprint 1 (Tuần 1 - Tuần 2):

* Mục tiêu: Tìm kiếm được sản phẩm và thêm vào giỏ hàng thành công
* Sprint Backlog: Hạng mục 1, 2 và 4

* Increment: Bản Web/App chạy được cho phép đăng nhập, tìm kiếm và tạo giỏ hàng

#### 5 Sự kiện trong Sprint (2 tuần):

* Sprint Planning (Đầu Sprint - 2h): Chốt mục tiêu và kế hoạch Sprint
* Daily Scrum (15 phút mỗi sáng): Cập nhật tiến độ, phát hiện vướng mắc

* Sprint Review (Cuối Sprint - 1h): Demo tính năng cho GreenMart xem
* Sprint Retrospective (Ngay sau Review - 1h): Đánh giá và cải tiến cách làm việc

* Backlog Refinement (Giữa Sprint - 1h): Làm rõ tính năng cho Sprint sau

### Xử lý Tình huống Thay đổi

#### Tình huống 1: Khách muốn đổi ưu tiên giữa Sprint (làm Đặt hàng online trước)

* PO ghi nhận yêu cầu và đưa tính năng này lên đầu Product Backlog để làm ở Sprint 2
* Giữ nguyên kế hoạch Sprint 1 đang chạy để tránh đứt gãy tiến độ của đội

#### Tình huống 2: Đến buổi Sprint Review vẫn còn tính năng chưa xong:

* Minh bạch thông báo với khách hàng, không demo tính năng chưa đạt chuẩn
* Cập nhật lại công việc dở dang vào Product Backlog để PO sắp xếp lại vào Sprint sau
