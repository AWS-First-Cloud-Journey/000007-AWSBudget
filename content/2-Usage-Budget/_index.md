+++
title = "Tạo Usage Budget"
date = 2020-04-18T00:38:32+07:00
weight = 2
chapter = false
pre = "<b>2. </b>"
+++

Ở phần này, bạn sẽ thực hành tạo một Usage Budget.

{{% notice note %}}
Nếu bạn đã làm qua phần [tạo Cost Budget](../1-cost-budgets), bạn sẽ thấy quy trình tạo Usage Budget cũng rất tương đồng, với một điểm khác nhau duy nhất là Cost Budget hoạt động dựa trên **chi phí**, còn Usage Budget hoạt động dựa trên **mức sử dụng**.

{{% /notice %}}

**Nội dung:**
- [Khởi tạo usage budget](#khởi-tạo-usage-budget)

#### Khởi tạo usage budget

1. Đăng nhập vào trang quản trị **AWS Management Console** và chọn dịch vụ **Billing** tại thanh tìm kiếm.
![Billing Service](/images/4-budget/CostBudget/1_FindBilling.png?width=90pc)
2. Tại trang quản trị, chọn **Budgets**. 
3. Chọn **Create budget**.
![Create Service](/images/4-budget/CostBudget/1_CreateBudget.png?width=90pc)
4. Tại trang **Select budget type**, chọn **Usage budget**, và chọn **Set your budget**.
5. Ở trang **Set you budget**, bạn có thể thiết lập các mục sau:
    - Mục **Define your budget name and timeframe**:
        - **Name**: đặt tên cho Budget.
        - **Period**: chọn khoảng thời gian cho Budget theo Ngày (*Daily*), Tháng (*Monthly*), Quý (*Quaterly*), và Năm (*Annualy*)
        - **Budget effective dates**:
            - Chọn **Recurring Budget** nếu bạn muốn Budget này được lặp đi lặp lại định kỳ
            - Chọn **Expiring Budget** nếu bạn chỉ muốn Budget được đặt một lần duy nhất.   
            - Tất cả các múi giờ đều là **UTC**.
    - Mục **Specify your monthly usage budget**:
        - Chọn **Usage unit(s)** hoặc **Usage Type** để chọn cách theo dõi mức sử dụng của bạn
            + Chọn **Usage Type Group**, nếu bạn muốn chọn loại giá trị cho tất cả các dịch vụ.
            + Chọn **Usage Type**, nếu bạn muốn chọn riêng từng dịch vụ và từng giá trị cho mỗi dịch vụ đó.
        - Chọn **Fixed** nếu bạn muốn mức sử dụng của mỗi kỳ hạn là giống nhau
        - Chọn **Monthly Budget Planning** nếu bạn muốn mức sử dụng của mỗi kỳ hạn là khác nhau
        - **Budgeted amount**: nhập số giờ tương ứng với mức sức dụng mà bạn cho phép.
            - **Lưu ý**: nếu bạn chọn **Monthly Budget Planning**, bạn sẽ phải nhập budgeted amount cho từng kỳ hạn.
![Budget Name & Amount](/images/4-budget/UsageBudget/2_BudgetNAme&Amount.png?width=90pc)
    - Mục **Set additional budget parameters - Optional**: bạn có thể lọc mức sử dụng cần theo dõi của Cost Budget bằng cách áp dụng các bộ lọc có sẵn.
6. Cuốn xuống cuối trang và chọn **Configure threhold**.
7. Tại trang **Configure threshold**, bạn có thể thiết lập mức sử dụng mà bạn muốn AWS Budget bắt đầu gửi cảnh báo.
    - Mục **Define your budget threshold**: bạn sẽ nhập mức sử dụng cho phép theo phần của tổng số giờ ngân sách cho phép
        - Chọn **Actual cost** nếu bạn muốn AWS Budget gửi cảnh báo khi mức sử dụng thực tế vượt qua mức sử dụng cho phép
        - Chọn **Forcasted cost** nếu bạn muốn AWS Budget gửi cảnh báo khi mức sử dụng dự báo vượt qua mức sử dụng cho phép
    - Mục **Set up your notifications**: bạn sẽ quyết định đối tượng nhận cảnh báo từ AWS Budget:
        - **Email recipient**: cảnh báo sẽ được gửi cho đối tượng nhận theo địa chỉ email. Tối đa 10 đối tượng nhận.
        - **Amazon Simple Notification Service (Amazon SNS)**: cảnh báo sẽ được gửi cho đối tượng nhận là các tài nguyên AWS thông qua Amazon SNS
        - **AWS Chatbot Alerts**: cảnh báo sẽ được gửi cho đối tượng nhận trong Amazon Chime hoặc Slack
8.  Chọn **Confirm budget**.
![Threshold](/images/4-budget/UsageBudget/2_Threshold.png?width=90pc)
9. Xem lại tất cả cấu hình và chọn **Create**.