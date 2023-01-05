---
title : "Tạo RI Budget"
date :  "`r Sys.Date()`" 
weight : 4
chapter : false
pre : " <b> 4. </b> "
---
Ở phần này, bạn sẽ thực hành khởi tạo một Reservation Instance (RI) Budget.

{{% notice info %}}
Do bạn sẽ không sử dụng reserve instance trong phạm vi các bài lab vì reserve instance yêu cầu bạn phải trả trước phí sử dụng, nên bài lab này chỉ mang tính chất minh họa. Chính vì thế, bạn có thể làm theo hoặc chỉ xem hướng dẫn cũng được.
{{% /notice %}}

**Nội dung:**
- [Khởi tạo reservation budget](#khởi-tạo-reservation-budget)

#### Khởi tạo reservation budget

1. Đăng nhập vào trang quản trị **AWS Management Console** và chọn dịch vụ **Billing** tại thanh tìm kiếm.

![Billing Service](/images/4/0001.png?featherlight=false&width=90pc)

1. Tại trang quản trị, chọn **Budgets**. 

![Billing Service](/images/4/0001.png?featherlight=false&width=90pc)

2. Chọn **Create budget**.

![Billing Service](/images/4/0001.png?featherlight=false&width=90pc)

3. Thực hiện **Budget setup**

- Chọn **Customize**
- Chọn **Reservation budget**
- Chọn **Next**

![Billing Service](/images/4/0002.png?featherlight=false&width=90pc)

4. Cấu hình **Coverage threshold**

![Billing Service](/images/4/0008.png?featherlight=false&width=90pc)

5. Cấu hình **Alert**

![Billing Service](/images/4/0006.png?featherlight=false&width=90pc)

6. Chọn **Create budget**

![Billing Service](/images/4/0007.png?featherlight=false&width=90pc)

7. Hoàn thành tạo budget

![Billing Service](/images/4/0009.png?featherlight=false&width=90pc)

8. Kiểm tra budget.


![Billing Service](/images/4/00010.png?featherlight=false&width=90pc)
