+++
title = "Tạo RI Budget"
date = 2020-04-18T00:38:32+07:00
weight = 3
chapter = false
pre = "<b>3. </b>"
+++

Ở phần này, bạn sẽ thực hành khởi tạo một Reservation Instance (RI) Budget.

{{% notice info %}}
Do bạn sẽ không sử dụng reserve instance trong phạm vi các bài lab vì reserve instance yêu cầu bạn phải trả trước phí sử dụng, nên bài lab này chỉ mang tính chất minh họa. Chính vì thế, bạn có thể làm theo hoặc chỉ xem hướng dẫn cũng được.
{{% /notice %}}

**Nội dung:**
- [Khởi tạo reservation budget](#khởi-tạo-reservation-budget)

#### Khởi tạo reservation budget

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
    - Mục **Specify your Reservation budget**:
        - Chọn **RI Utilization** hoặc **RI Coverage** để chọn cách theo dõi mức sử dụng của bạn
            + Chọn **RI Utilization**, nếu bạn muốn theo dõi phần trăm mức sử dụng reserve instance hiện tại so với mức sử dụng đã trả trước cho reserve instance.
{{% notice info %}}
**RI Utilization** = tổng số giờ sử dụng reserve instanace / tổng số giờ đã trả trước cho reserve instance. Chính vì thế, RI Utilization giúp bạn đo độ hiệu quả của việc sử dụng reserve instance.
{{% /notice %}}
            + Chọn **RI Coverage**, nếu bạn muốn theo dõi phần trăm mức sử dụng reserve instance hiện tại so với tổng mức sử dụng dịch vụ có cùng phân loại với reserve instance.
{{% notice info %}}
**RI Coverage** = tổng số giờ sử dụng reserve instanace / tổng số giờ đã sử dụng dịch vụ có cùng phân loại với reserve instance. Chính vì thế, RI Coverage giúp bạn quyết định được lượng reserve instance cần trả trước để có thể tận dụng tối đa độ phủ của reserve instace vì sử dụng reserve instance sẽ rẻ hơn là sử dụng on-demand instance.
{{% /notice %}}

{{% notice tip %}}
Giả sử chúng ta cam kết sử dụng 100 giờ nhưng chỉ sử dụng hết 50 giờ.  
**RI Utilization** = 50%  ( do chúng ta chỉ sủ dụng 50% số giờ cam kết )
**RI Coverage** = 100%  ( do mức cam kết đã đảm bảo toàn bộ mức sử dụng thực tế )
Trong truong hợp chúng ta cam kết sử dụng 50 giờ nhưng thực tế dùng đến 100 giờ.  
**RI Utilization** = 100%  ( do chúng ta đã sử dụng toàn bộ số giờ cam kết )
**RI Coverage** = 50% ( do chúng ta chỉ cam kết được 50% mức sử dụng thực tế )  
{{% /notice %}}
        - Tại **Service**, chọn loại service mà bạn muốn đặt Budget.
        - Tại **Utilization threshold**, điền vào giá trị bạn muốn thiết lập cho Budget.
![Budget Name & Amount](/images/4-budget/ReservationBudget/3_BudgetNAme&Amount.png?width=90pc)
    - Mục **Set additional budget parameters - Optional**: bạn có thể lọc mức sử dụng cần theo dõi của Cost Budget bằng cách áp dụng các bộ lọc có sẵn.
6. Cuốn xuống cuối trang và chọn **Configure alerts**.
7. Tại mục **Email contacts**, nhập vào email mà bạn muốn gửi thông báo tới và chọn **Add email contact** để có thể gửi đến nhiều email cùng 1 lúc. Thông báo có thể gửi tới 10 email 1 lúc. 
    - Bạn cũng có thể sử dụng dịch vụ AWS SNS hoặc AWS Chatbot để gửi thông báo.  
8. Chọn **Confirm budget**.
![Configure Alerts](/images/4-budget/ReservationBudget/3_ConfigureAlerts.png?width=90pc)
9. Xem lại tất cả cấu hình và chọn **Create**.