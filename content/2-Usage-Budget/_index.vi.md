+++
title = "Tạo Usage Budget"
date = 2020-04-18T00:38:32+07:00
weight = 2
chapter = false
pre = "<b>2. </b>"
+++

**Nội dung:**
- [Khởi tạo usage budget](#khởi-tạo-usage-budget)

#### Khởi tạo usage budget

1. Đăng nhập vào trang quản trị AWS Management Console, vào dịch vụ Billing and Cost Management tại **[Amazon Web Services](https://console.aws.amazon.com/billing/home?#/budgets)**.
2. Tại trang quản trị, chọn **Budgets**. 
3. Chọn **Create budget**.
4. Tại mục **Select budget type**, Chọn **Usage budget**.
5. Chọn **Set your budget**.
6. Tại mục **Name**, đặt tên cho Budget.
7. Tại mục **Period**, chọn khoảng thời gian cho Budget. Bạn có thể đặt Budget theo **Tháng, Quý, Năm**.  
8. Tại mục **Usage unit(s)**, chọn **Usage Type Group** hoặc **Usage Type**.
    + Chọn **Usage Type Group**, nếu bạn muốn chọn loại giá trị cho tất cả các dịch vụ.
    + Chọn **Usage Type**, nếu bạn muốn chọn riêng từng dịch vụ và từng giá trị cho mỗi dịch vụ đó.
9. Tại mục **Budgeted Amount**, điền vào số tiền mà bạn muốn đặt cho Budget.
10. Tại mục **Budget parameters (optional)**, chọn **Filtering**, bạn có thể để Budget bao gồm tất cả dịch vụ hoặc [tùy chọn dịch vụ](https://docs.aws.amazon.com/awsaccountbilling/latest/aboutv2/budgets-create-filters.html).  
    Tất cả các múi giờ đều là UTC.

![Create Usage Budget](/images/4-budget/UsageBudget/usage-budget-1.PNG?width=90pc)

11.   Phía dưới **Budget parameters (optional)**, chọn **Filtering**, bạn có thể để Budget bao gồm tất cả dịch vụ hoặc [tùy chọn dịch vụ](https://docs.aws.amazon.com/awsaccountbilling/latest/aboutv2/budgets-create-filters.html).     

![Create Usage Budget](/images/4-budget/UsageBudget/usage-budget-2.PNG?width=90pc)

12.  Chọn **Configure alerts**.
13.  Tại mục **Configure alerts**, **Alert 1**, chọn **Actual** để gửi thông báo đối với số tiền Budget thực tế và **Forecast** để gửi thông báo đối với số tiền Budget được dự đoán trong tương lai.
14.  Tại mục **Alert threshold**, nhập số lượng phần trăm để khi số tiền Budget đạt tới mức đó, thông báo sẽ được gửi đến bạn. Ví dụ, bạn cấu hình Budget là 200$, bạn muốn khi số tiền đạt tới mức 80% của Budget thì thông báo sẽ được gửi đến bạn. Bạn cần điền vào đó mức là 80%. 
15.  Tại mục **Email contacts**, nhập vào email mà bạn muốn gửi thông báo tới và chọn **Add email contact** để có thể gửi đến nhiều email cùng 1 lúc. Thông báo có thể gửi tới 10 email 1 lúc. 
    Bạn cũng có thể sử dụng dịch vụ AWS SNS để gửi thông báo.
16.  Đối với bạn sử dụng **SNS topic ARN**, nhập SNS ARN của bạn và chọn **Verify**. Để tìm hiểu cách sử dụng AWS SNS, bạn có thể tham khảo [link sau](https://docs.aws.amazon.com/sns/latest/dg/sns-tutorial-create-topic.html).  
17.  Chọn **Confirm budget**.

![Configure Alert](/images/4-budget/UsageBudget/usage-budget-3.PNG?width=90pc)

18. Xem lại tất cả cấu hình và chọn **Create**.

![Review](/images/4-budget/UsageBudget/usage-budget-4.PNG?width=90pc)