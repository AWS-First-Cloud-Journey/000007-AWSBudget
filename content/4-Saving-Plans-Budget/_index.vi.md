---
title : "Tạo Saving Plans Budget"
date :  "`r Sys.Date()`" 
weight : 5
chapter : false
pre : " <b> 5. </b> "
---

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

![Billing Service](/images/5/0001.png?featherlight=false&width=90pc)

1. Tại trang quản trị, chọn **Budgets**. 

![Billing Service](/images/5/0001.png?featherlight=false&width=90pc)

2. Chọn **Create budget**.

![Billing Service](/images/5/0001.png?featherlight=false&width=90pc)

3. Thực hiện **Budget setup**

- Chọn **Customize**
- Chọn **Budget types** là  **Saving Plan budget**
- Chọn **Next**

![Billing Service](/images/5/0002.png?featherlight=false&width=90pc)

4. Đặt tên cho **Budget name**

![Billing Service](/images/5/0003.png?featherlight=false&width=90pc)

5. Thực hiện cấu hình threshold.

![Billing Service](/images/5/0004.png?featherlight=false&width=90pc)

6. Cấu hình **Alert** và sau đó chọn **Next**

![Billing Service](/images/5/0005.png?featherlight=false&width=90pc)

7. Chọn **Create budget**

![Billing Service](/images/5/0006.png?featherlight=false&width=90pc)

8. Tạp budget thành công.

![Billing Service](/images/5/0007.png?featherlight=false&width=90pc)

9. Xem chi tiết budget đã tạo.

![Billing Service](/images/5/0008.png?featherlight=false&width=90pc)