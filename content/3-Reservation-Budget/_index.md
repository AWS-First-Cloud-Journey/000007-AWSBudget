+++
title = "Tạo Reservation Budget"
date = 2020-04-18T00:38:32+07:00
weight = 3
chapter = false
pre = "<b>3. </b>"
+++

**Nội dung:**
- [Khởi tạo reservation budget](#khởi-tạo-reservation-budget)

#### Khởi tạo reservation budget

1. Đăng nhập vào trang quản trị AWS Management Console, vào dịch vụ Billing and Cost Management tại **[Amazon Web Services](https://console.aws.amazon.com/billing/home?#/budgets)**.
2. Tại trang quản trị, chọn **Budgets**.
3. Chọn **Create budget**.
4. Tại mục **Select budget type**, Chọn **Reservation budget**.
5. Chọn **Set your budget**.
6. Tại mục **Name**, đặt tên cho Budget.
7. Tại mục **Period**, chọn khoảng thời gian cho Budget. Bạn có thể đặt Budget theo **Tháng, Quý, Năm**.    
   Tất cả các múi giờ đều là **UTC**.
8. Tại mục **Reservation budget type**, bạn có thể tùy chọn giữa 2 loại **RI Utilization** hoặc **RI Coverage**.  
9.  Tại mục **Service**, chọn loại service mà bạn muốn đặt Budget.
10. Tại mục **Utilization threshold**, điền vào giá trị bạn muốn thiết lập cho Budget.  

![Create Reservation Budget](/images/4-budget/ReservationBudget/reservation-budget-1.PNG?width=90pc)

{{%notice tip%}}

**RI Utilization** : Là tỉ lệ sử dụng các RI chúng ta đã mua, giúp xác định xem chúng ta có lãng phí RI hay không.\
**RI Coverage** : Là tỉ lệ những RI chúng ta đã mua so với tổng các instance mà chúng ta có thể mua thêm RI, giúp xác định chúng ta có thể tối ưu hóa chi phí bằng cách mua thêm RI hay không.
{{%/notice%}}

11. Tại mục **Budget parameters (optional)**, chọn **Filtering**, bạn có thể để Budget bao gồm tất cả dịch vụ hoặc [tùy chọn dịch vụ](https://docs.aws.amazon.com/awsaccountbilling/latest/aboutv2/budgets-create-filters.html).  

![Create Reservation Budget](/images/4-budget/ReservationBudget/reservation-budget-2.PNG?width=90pc)

12. Chọn **Configure alert**.
13. Tại mục **Email contacts**, nhập vào email mà bạn muốn gửi thông báo tới và chọn **Add email contact** để có thể gửi đến nhiều email cùng 1 lúc. Thông báo có thể gửi tới 10 email 1 lúc. 
    Bạn cũng có thể sử dụng dịch vụ AWS SNS để gửi thông báo.
14. Đối với bạn sử dụng **SNS topic ARN**, nhập SNS ARN của bạn và chọn **Verify**. Để tìm hiểu cách sử dụng AWS SNS, bạn có thể tham khảo [link sau](https://docs.aws.amazon.com/sns/latest/dg/sns-tutorial-create-topic.html). 
15. Chọn **Confirm budget**.

![Create Reservation Budget](/images/4-budget/ReservationBudget/reservation-budget-3.PNG?width=90pc)

16. Xem lại tất cả cấu hình và chọn **Create**.

![Create Reservation Budget](/images/4-budget/ReservationBudget/reservation-budget-4.PNG?width=90pc)
