---
title : "Tạo Saving Plans Budget"
date :  2025-09-30
weight : 5
chapter : false
pre : " <b> 5. </b> "
---

#### Giới thiệu

Ở phần này, bạn sẽ thực hành khởi tạo một Savings Plans Budget trong AWS Billing and Cost Management để theo dõi và quản lý hiệu quả các cam kết Savings Plans của bạn.

{{% notice info %}}
**ℹ️ Information**: Do bạn sẽ không sử dụng Savings Plans trong phạm vi các bài lab vì Savings Plans yêu cầu bạn phải cam kết sử dụng trước, nên bài lab này chỉ mang tính chất minh họa. Chính vì thế, bạn có thể làm theo hướng dẫn hoặc chỉ xem qua các bước thực hiện.
{{% /notice %}}

{{% notice note %}}
**ℹ️ Information**: Nếu bạn đã làm qua phần [tạo RI Budget](../3-reservation-budgets), bạn sẽ thấy quy trình tạo Savings Plans Budget cũng rất tương đồng. Điểm khác biệt chính là Reservation Budget liên quan đến **Reserved Instances**, còn Savings Plans Budget liên quan đến các cam kết **Savings Plans**.
{{% /notice %}}

#### Nội dung

- [Khởi tạo Savings Plans Budget](#khởi-tạo-savings-plans-budget)

#### Khởi tạo Savings Plans Budget

1. Đăng nhập vào trang quản trị **AWS Management Console** và tìm dịch vụ **AWS Billing and Cost Management** tại thanh tìm kiếm.

![Billing Service](/images/5/z0001.png?featherlight=false&width=90pc)

2. Tại trang quản trị, chọn **Budgets** từ menu bên trái.

![Billing Service](/images/5/x00001.png?featherlight=false&width=90pc)

3. Nhấn vào nút **Create budget**.

![Billing Service](/images/5/x00001.png?featherlight=false&width=90pc)

4. Thực hiện cấu hình **Budget setup**:

   - Chọn **Customize** (tùy chỉnh)
   - Tại **Budget types**, chọn **Savings Plans budget**
   - Nhấn **Next**

![Billing Service](/images/5/z0002.png?featherlight=false&width=90pc)

![Billing Service](/images/5/z00002.png?featherlight=false&width=90pc)

5. Tại phần **Details**, nhập tên cho budget của bạn trong trường **Budget name**.

![Billing Service](/images/5/z0003.png?featherlight=false&width=90pc)

6. Thực hiện cấu hình **Utilization threshold** - ngưỡng sử dụng cho Savings Plans.

![Billing Service](/images/5/z0004.png?featherlight=false&width=90pc)

7. Cấu hình **Alert preferences** và sau đó chọn **Next**:
   - Thiết lập ngưỡng cảnh báo
   - Thêm địa chỉ email để nhận thông báo khi đạt ngưỡng

![Billing Service](/images/5/z0005.png?featherlight=false&width=90pc)

8. Xem lại các thiết lập và nhấn **Create budget** để hoàn tất.

![Billing Service](/images/5/z0006.png?featherlight=false&width=90pc)

9. Sau khi tạo thành công, bạn sẽ thấy thông báo xác nhận.

![Billing Service](/images/5/z0007.png?featherlight=false&width=90pc)

10. Kiểm tra chi tiết budget đã tạo trong danh sách budgets.

![Billing Service](/images/5/z0008.png?featherlight=false&width=90pc)

{{% notice tip %}}
**💡 Pro Tip**: Savings Plans Budget giúp bạn theo dõi mức độ sử dụng cam kết Savings Plans và đảm bảo bạn đang tận dụng tối đa các khoản tiết kiệm. Thiết lập ngưỡng cảnh báo ở mức 80-90% sẽ giúp bạn có thời gian điều chỉnh trước khi đạt đến mức sử dụng tối đa.
{{% /notice %}}

{{% notice info %}}
**ℹ️ Information**: AWS Savings Plans cung cấp mô hình giá linh hoạt với mức giảm giá lên đến 72% so với giá On-Demand, đổi lại bạn cam kết sử dụng một lượng tính toán nhất định (tính bằng USD/giờ) trong thời hạn 1 hoặc 3 năm.
{{% /notice %}}