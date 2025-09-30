---
title : "Tạo Usage Budget"
date : 2025-09-30
weight : 3
chapter : false
pre : " <b> 3. </b> "
---

#### Tổng quan

Ở phần này, bạn sẽ thực hành tạo một Usage Budget - công cụ giúp bạn theo dõi và kiểm soát mức sử dụng tài nguyên AWS của mình.

ℹ️ **Information**: Nếu bạn đã làm qua phần [tạo Cost Budget](../1-cost-budgets), bạn sẽ thấy quy trình tạo Usage Budget cũng rất tương đồng, với một điểm khác biệt chính là Cost Budget hoạt động dựa trên **chi phí**, còn Usage Budget hoạt động dựa trên **mức sử dụng** tài nguyên.

#### Khởi tạo Usage Budget

1. Đăng nhập vào **AWS Management Console** và tìm dịch vụ **Billing and Cost Management** tại thanh tìm kiếm.


![Billing Service](/images/3/abc.png?featherlight=false&width=90pc)


2. Tại trang quản trị, chọn **Budgets** từ menu bên trái.

![Budgets Menu](/images/3/00001.png?featherlight=false&width=90pc)

3. Nhấn vào nút **Create budget**.

![Create Budget](/images/3/00001.png?featherlight=false&width=90pc)

#### Thiết lập cấu hình Budget

4. Trong phần **Budget setup**:
   - Chọn **Customize** (tùy chỉnh)
   - Tại **Budget types**, chọn **Usage budget**
   - Nhấn **Next**

![Budget Type](/images/3/00002.png?featherlight=false&width=90pc)

5. Trong giao diện **Set your budget**:
   - Tại **Budget name**, nhập tên cho budget của bạn

![Budget Name](/images/3/00003.png?featherlight=false&width=90pc)

6. Tại phần **Usage type**:
   - Chọn **Usage type groups**
   - Chọn **EC2:Running Hours** để theo dõi số giờ chạy của EC2 instances

![Usage Type](/images/3/00004.png?featherlight=false&width=90pc)

7. Thực hiện cấu hình **Set budget amount**:
   - **Period**: Chọn khoảng thời gian cho Budget (Hàng ngày/Hàng tháng/Hàng quý/Hàng năm)
   - **Budget renewal type**: Chọn loại gia hạn ngân sách (Recurring/Expiring)
   - **Budgeting method**: Chọn phương pháp lập ngân sách (Fixed/Planned)
   - Nhập số giờ sử dụng tối đa mà bạn muốn giới hạn

![Budget Amount](/images/3/00005.png?featherlight=false&width=90pc)

8. Tại phần **Budget scope**, giữ mặc định và chọn **Next**.

![Budget Scope](/images/3/00006.png?featherlight=false&width=90pc)

#### Thiết lập cảnh báo

9. Trong phần **Configure alerts**, chọn **Add an alert threshold** để thiết lập ngưỡng cảnh báo.

![Configure Alerts](/images/3/00007.png?featherlight=false&width=90pc)

10. Hoàn thành thông tin **Alert**:
    - Thiết lập ngưỡng cảnh báo (% của ngân sách)
    - Thêm địa chỉ email để nhận thông báo khi vượt ngưỡng

![Alert Details](/images/3/00008.png?featherlight=false&width=90pc)

11. Nhấn **Next** để tiếp tục.

![Next Step](/images/3/00009.png?featherlight=false&width=90pc)

12. Xem lại các thiết lập và chọn **Create budget** để hoàn tất.

![Create Budget](/images/3/000010.png?featherlight=false&width=90pc)

#### Xem và quản lý Budget

13. Sau khi tạo thành công, bạn sẽ thấy budget mới trong danh sách.

![Budget Created](/images/3/000011.png?featherlight=false&width=90pc)

14. Kiểm tra **Budget health** (Tình trạng ngân sách) để theo dõi mức sử dụng hiện tại so với ngân sách đã thiết lập.

![Budget Health](/images/3/000012.png?featherlight=false&width=90pc)

15. Xem **Budget history** (Lịch sử ngân sách) để theo dõi xu hướng sử dụng qua thời gian.

![Budget History](/images/3/000013.png?featherlight=false&width=90pc)

💡 **Pro Tip**: Sử dụng Usage Budget để theo dõi và kiểm soát việc sử dụng tài nguyên AWS, đặc biệt là các dịch vụ tính phí theo giờ như EC2. Điều này giúp bạn tránh việc sử dụng quá mức dự kiến và kiểm soát chi phí hiệu quả hơn.

🔒 **Security Note**: Đảm bảo chỉ những người có trách nhiệm quản lý chi phí mới nhận được thông báo cảnh báo từ budget để tránh rò rỉ thông tin nhạy cảm về tài chính của tổ chức.