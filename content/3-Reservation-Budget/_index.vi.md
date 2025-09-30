---
title : "Tạo RI Budget"
date : 2025-09-30 
weight : 4
chapter : false
pre : " <b> 4. </b> "
---

#### Giới thiệu

Ở phần này, bạn sẽ thực hành khởi tạo một Reservation Instance (RI) Budget trong AWS Billing and Cost Management.

{{% notice info %}}
**ℹ️ Information**: Do bạn sẽ không sử dụng Reserved Instance trong phạm vi các bài lab vì Reserved Instance yêu cầu bạn phải trả trước phí sử dụng, nên bài lab này chỉ mang tính chất minh họa. Chính vì thế, bạn có thể làm theo hoặc chỉ xem hướng dẫn cũng được.
{{% /notice %}}

#### Nội dung

- [Khởi tạo Reservation Budget](#khởi-tạo-reservation-budget)

#### Khởi tạo Reservation Budget

1. Đăng nhập vào trang quản trị **AWS Management Console** và chọn dịch vụ **AWS Billing and Cost Management** tại thanh tìm kiếm.

![Billing Service](/images/4/z0001.png?featherlight=false&width=90pc)

2. Tại trang quản trị, chọn **Budgets**. 

![Billing Service](/images/4/z00001.png?featherlight=false&width=90pc)

3. Chọn **Create budget**.

![Billing Service](/images/4/z00001.png?featherlight=false&width=90pc)

4. Thực hiện **Budget setup**:

   - Chọn **Customize**
   - Chọn **Reservation budget**
   - Chọn **Next**

![Billing Service](/images/4/z0002.png?featherlight=false&width=90pc)

![Billing Service](/images/4/z00002.png?featherlight=false&width=90pc)

5. Đặt tên budget.

![Billing Service](/images/4/x0003.png?featherlight=false&width=90pc)

6. Cấu hình **Coverage threshold**.

![Billing Service](/images/4/z0004.png?featherlight=false&width=90pc)

7. Cấu hình **Alert preferences**.

![Billing Service](/images/4/z0005.png?featherlight=false&width=90pc)

8. Chọn **Create budget**.

![Billing Service](/images/4/z0006.png?featherlight=false&width=90pc)

9. Hoàn thành tạo budget.

![Billing Service](/images/4/x0007.png?featherlight=false&width=90pc)

10. Kiểm tra budget đã tạo.

![Billing Service](/images/4/x0008.png?featherlight=false&width=90pc)

{{% notice tip %}}
**💡 Pro Tip**: Reservation Budgets giúp bạn theo dõi mức độ sử dụng Reserved Instances và tiết kiệm chi phí. Thiết lập các ngưỡng cảnh báo phù hợp sẽ giúp bạn tối ưu hóa việc sử dụng Reserved Instances.
{{% /notice %}}
