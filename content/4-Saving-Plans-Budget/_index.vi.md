+++
title = "Tạo Saving Plans Budget"
date = 2020-04-18T00:38:32+07:00
weight = 4
chapter = false
pre = "<b>4. </b>"
+++

Ở phần này, bạn sẽ thực hành khởi tạo một Savings Plans Budget

{{% notice info %}}
Do bạn sẽ không sử dụng savings plans instance trong phạm vi các bài lab vì savings plans instance yêu cầu bạn phải mua trước savings plans, nên bài lab này chỉ mang tính chất minh họa. Chính vì thế, bạn có thể làm theo hoặc chỉ xem hướng dẫn cũng được.
{{% /notice %}}

{{% notice note %}}
Nếu bạn đã làm qua phần [tạo RI Budget](../3-reservation-budgets), bạn sẽ thấy quy trình tạo Savings Plans Budget cũng rất tương đồng, với một điểm khác nhau duy nhất là Reservation Budget hoạt động liên quan tới **reserve instance**, còn Savings Plans Budget hoạt động liên quan tới **savings plans instance**.
{{% /notice %}}

**Nội dung:**
- [Khởi tạo Saving plans Budget](#khởi-tạo-saving-plans-budget)

#### Khởi tạo Saving plans Budget

1. Đăng nhập vào trang quản trị **AWS Management Console** và chọn dịch vụ **Billing** tại thanh tìm kiếm.
![Billing Service](/images/4-budget/CostBudget/1_FindBilling.png?width=90pc)
2. Tại trang quản trị, chọn **Budgets**. 
3. Chọn **Create budget**.
![Create Service](/images/4-budget/CostBudget/1_CreateBudget.png?width=90pc)
4. Tại trang **Select budget type**, chọn **Reservation budget**, và chọn **Set your budget**.
5. Ở trang **Set you budget**, bạn có thể thiết lập các mục sau:
    - Mục **Define your budget name and timeframe**:
        - **Name**: đặt tên cho Budget.
        - **Period**: chọn khoảng thời gian cho Budget theo Ngày (*Daily*), Tháng (*Monthly*), Quý (*Quaterly*), và Năm (*Annualy*)
    - Mục **Specify your Savings Plans budget**:
        - Chọn **Savings Plans Utilization** hoặc **Savings Plans Coverage** để chọn cách theo dõi mức sử dụng của bạn
            + Chọn **Savings Plans Utilization**, nếu bạn muốn theo dõi phần trăm mức sử dụng savings plans instance hiện tại so với mức sử dụng đã định trước cho saving plans instance.
{{% notice info %}}
**Savings Plans Utilization** = tổng số giờ sử dụng savaings plans instanace / tổng số giờ đã định trước cho savings plans instance. Chính vì thế, Savings Plans Utilization giúp bạn đo độ hiệu quả của việc sử dụng savings plans instance.
{{% /notice %}}
            + Chọn **Savings Plans Coverage**, nếu bạn muốn theo dõi phần trăm mức sử dụng savings plans instance hiện tại so với tổng mức sử dụng dịch vụ có cùng phân loại với savings plans instance.
{{% notice info %}}
**Savings Plans Coverage** = tổng số giờ sử dụng savings plans instanace / tổng số giờ đã sử dụng dịch vụ có cùng phân loại với savings plans instance. Chính vì thế, Savings Plans Coverage giúp bạn quyết định được lượng savings plans instance cần trả trước để có thể tận dụng tối đa độ phủ của savings plans instace vì sử dụng savings plans instance sẽ rẻ hơn là sử dụng on-demand instance.
{{% /notice %}}
        - Tại **Utilization threshold**, điền vào giá trị bạn muốn thiết lập cho Budget.
    - Mục **Set additional budget parameters - Optional**: bạn có thể lọc mức sử dụng cần theo dõi của Cost Budget bằng cách áp dụng các bộ lọc có sẵn.
![Budget Name & Amount](/images/4-budget/SavingPlansBudget/4_BudgetNAme&Amount.png?width=90pc)
6. Cuốn xuống cuối trang và chọn **Configure alerts**.
7. Tại mục **Email contacts**, nhập vào email mà bạn muốn gửi thông báo tới và chọn **Add email contact** để có thể gửi đến nhiều email cùng 1 lúc. Thông báo có thể gửi tới 10 email 1 lúc. 
    - Bạn cũng có thể sử dụng dịch vụ AWS SNS hoặc AWS Chatbot để gửi thông báo.  
8. Chọn **Confirm budget**.
![Configure Alerts](/images/4-budget/SavingPlansBudget/4_ConfigureAlerts.png?width=90pc)
9. Xem lại tất cả cấu hình và chọn **Create**.