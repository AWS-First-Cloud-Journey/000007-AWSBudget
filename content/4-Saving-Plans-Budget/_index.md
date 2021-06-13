+++
title = "Tạo Saving plans Budget"
date = 2020-04-18T00:38:32+07:00
weight = 4
chapter = false
pre = "<b>4. </b>"
+++

**Nội dung:**
- [Khởi tạo Saving plans Budget](#khởi-tạo-saving-plans-budget)

#### Khởi tạo Saving plans Budget

1. Đăng nhập vào trang quản trị AWS Management Console, vào dịch vụ Billing and Cost Management tại **[Amazon Web Services](https://console.aws.amazon.com/billing/home?#/budgets)**.
2. Tại trang quản trị, chọn **Budgets**.
3. Chọn **Create budget**.
4. Tại mục **Select budget type**, Chọn **Savings Plans budget**.
5. Chọn **Set your budget**.
6. Tại mục **Name**, đặt tên cho Budget.
7. Tại mục **Period**, chọn khoảng thời gian cho Budget. Bạn có thể đặt Budget theo **Tháng, Quý, Năm**.    
   Tất cả các múi giờ đều là **UTC**.
8. Tại mục **Savings Plans budget type**, chọn loại Saving Plans mà bạn muốn đặt Budget: **Savings Plans Utilization** hoặc **Savings Plans Coverage**.  
9.  Tại mục **Utilization threshold**, điền vào giá trị bạn muốn thiết lập cho Budget. 

![Create Reservation Budget](/images/4-budget/SavingPlansBudget/savingplansbudget-1.PNG?width=90pc)

10. Tại mục **Budget parameters (optional)**, chọn **Filtering**, bạn có thể để Budget bao gồm tất cả dịch vụ hoặc [tùy chọn dịch vụ](https://docs.aws.amazon.com/awsaccountbilling/latest/aboutv2/budgets-create-filters.html).

![Create Reservation Budget](/images/4-budget/SavingPlansBudget/savingplansbudget-2.PNG?width=90pc)

11. Chọn **Configure alerts**.
12. Tại mục **Email contacts**, nhập vào email mà bạn muốn gửi thông báo tới và chọn **Add email contact** để có thể gửi đến nhiều email cùng 1 lúc. Thông báo có thể gửi tới 10 email 1 lúc. 
    Bạn cũng có thể sử dụng dịch vụ AWS SNS để gửi thông báo.  
    To receive a notification, you must specify an email address, You can also specify an Amazon SNS topic.
13. Đối với bạn sử dụng **SNS topic ARN**, nhập SNS ARN của bạn và chọn **Verify**. Để tìm hiểu cách sử dụng AWS SNS, bạn có thể tham khảo [link sau](https://docs.aws.amazon.com/sns/latest/dg/sns-tutorial-create-topic.html). 
14. Chọn **Confirm budget**.

![Create Reservation Budget](/images/4-budget/SavingPlansBudget/savingplansbudget-3.PNG?width=90pc)

15. Xem lại tất cả cấu hình và chọn **Create**.

![Create Reservation Budget](/images/4-budget/SavingPlansBudget/savingplansbudget-4.PNG?width=90pc)
