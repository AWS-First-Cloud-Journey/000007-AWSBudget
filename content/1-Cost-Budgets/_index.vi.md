
---
title : "Tạo Cost Budget"
date :  "`r Sys.Date()`" 
weight : 2
chapter : false
pre : " <b> 2. </b> "
---


Ở phần này, bạn sẽ thực hành tạo một Cost Budget.

#### Khởi tạo cost budget

1. Đăng nhập vào trang quản trị **AWS Management Console** và chọn dịch vụ **Billing** tại thanh tìm kiếm.

1. Tại trang quản trị, chọn **Budgets**. 

2. Chọn **Create budget**.

![Billing Service](/images/2/0001.png?featherlight=false&width=90pc)

4. Đối với **Budget setup**

- Chọn **Customize**
- **Budget types**, chọn **Cost budget**
- Chọn **Next**

![Billing Service](/images/2/0002.png?featherlight=false&width=90pc)

5. Trong giao diện **Set your budget**

- Đối với **Budget name**, nhập **```Monthly```**

![Billing Service](/images/2/0003.png?featherlight=false&width=90pc)

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

![Billing Service](/images/2/0004.png?featherlight=false&width=90pc)

6. Đối với **Budget scope** chọn **All AWS services**. Sau đó chọn **Next**

![Create Cost Budget](/images/2/0005.png?featherlight=false&width=90pc)

7. Đối với **Configure alerts**, chọn **Add an alert threshold**. Chọn **Next**


![Create Cost Budget](/images/2/0006.png?featherlight=false&width=90pc)

8. Thực hiện cấu hình **Alert** và chọn **Next**

![Create Cost Budget](/images/2/0007.png?featherlight=false&width=90pc)

9. Chọn **Next**

![Create Cost Budget](/images/2/0008.png?featherlight=false&width=90pc)

10. Chọn **Create budget**

![Create Cost Budget](/images/2/0009.png?featherlight=false&width=90pc)

11. Tạo budget thành công.

![Create Cost Budget](/images/2/00010.png?featherlight=false&width=90pc)

