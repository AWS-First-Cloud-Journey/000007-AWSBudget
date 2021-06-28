+++
title = "Tạo Cost Budget"
date = 2020-04-18T00:38:32+07:00
weight = 1
chapter = false
pre = "<b>1. </b>"
+++

Ở phần này, bạn sẽ thực hành tạo một Cost Budget.

**Nội dung:**
- [Khởi tạo cost budget](#khởi-tạo-cost-budget)

#### Khởi tạo cost budget

1. Đăng nhập vào trang quản trị **AWS Management Console** và chọn dịch vụ **Billing** tại thanh tìm kiếm.
![Billing Service](/images/4-budget/CostBudget/1_FindBilling.png?width=90pc)
2. Tại trang quản trị, chọn **Budgets**. 
3. Chọn **Create budget**.
![Create Service](/images/4-budget/CostBudget/1_CreateBudget.png?width=90pc)
4. Tại trang **Select budget type**, chọn **Cost budget**, và chọn **Set your budget**.
![Cost Service](/images/4-budget/CostBudget/1_CostBudget.png?width=90pc)
5. Ở trang **Set you budget**, bạn có thể thiết lập các mục sau:
    - Mục **Define your budget name and timeframe**:
        - **Name**: đặt tên cho Budget.
        - **Period**: chọn khoảng thời gian cho Budget theo Ngày (*Daily*), Tháng (*Monthly*), Quý (*Quaterly*), và Năm (*Annualy*)
        - **Budget effective dates**:
            - Chọn **Recurring Budget** nếu bạn muốn Budget này được lặp đi lặp lại định kỳ
            - Chọn **Expiring Budget** nếu bạn chỉ muốn Budget được đặt một lần duy nhất.   
            - Tất cả các múi giờ đều là **UTC**.
    - Mục **Specify your monthly budget**:
        - Chọn **Fixed** nếu bạn muốn ngân sách của mỗi kỳ hạn là giống nhau
        - Chọn **Monthly Budget Planning** nếu bạn muốn ngân sách của mỗi kỳ hạn là khác nhau
        - **Budgeted amount**: nhập số tiền tương ứng với ngân sách của bạn.
            - **Lưu ý**: nếu bạn chọn **Monthly Budget Planning**, bạn sẽ phải nhập budgeted amount cho từng kỳ hạn.
![Budget Name & Amount](/images/4-budget/CostBudget/1_BudgetName&Amount.png?width=90pc)
    - Mục **Set additional budget parameters - Optional**: bạn có thể lọc chi phí cần theo dõi của Cost Budget bằng cách áp dụng các bộ lọc có sẵn.
6. Cuốn xuống cuối trang và chọn **Configure threhold**.
![Create Cost Budget](/images/4-budget/CostBudget/1_BudgetPara.png?width=90pc)
7. Tại trang **Configure threshold**, bạn có thể thiết lập ngưỡng chi phí mà bạn muốn AWS Budget bắt đầu gửi cảnh báo.
    - Mục **Define your budget threshold**: bạn sẽ nhập ngưỡng chi phí theo phần trăm của ngân sách
        - Chọn **Actual cost** nếu bạn muốn AWS Budget gửi cảnh báo khi chi phí thực tế vượt qua ngưỡng chi phí
        - Chọn **Forcasted cost** nếu bạn muốn AWS Budget gửi cảnh báo khi chi phí dự báo vượt qua ngưỡng chi phí.
    - Mục **Set up your notifications**: bạn sẽ quyết định đối tượng nhận cảnh báo từ AWS Budget:
        - **Email recipient**: cảnh báo sẽ được gửi cho đối tượng nhận theo địa chỉ email. Tối đa 10 đối tượng nhận.
        - **Amazon Simple Notification Service (Amazon SNS)**: cảnh báo sẽ được gửi cho đối tượng nhận là các tài nguyên AWS thông qua Amazon SNS
        - **AWS Chatbot Alerts**: cảnh báo sẽ được gửi cho đối tượng nhận trong Amazon Chime hoặc Slack
8.  Chọn **Confirm budget**.
![Threshold](/images/4-budget/CostBudget/1_Threshold.png?width=90pc)
9. Xem lại tất cả cấu hình và chọn **Create**.

