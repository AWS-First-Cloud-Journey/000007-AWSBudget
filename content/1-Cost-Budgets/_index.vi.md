+++
title = "Tạo Cost Budget"
date = 2024
weight = 2
chapter = false
pre = " <b> 2. </b> "
+++

#### Tổng quan

Ở phần này, bạn sẽ thực hành tạo một Cost Budget - công cụ quan trọng giúp bạn theo dõi và kiểm soát chi phí AWS của mình.

#### Khởi tạo Cost Budget

ℹ️ **Information**: Các tài khoản AWS mới chỉ có thể tạo được Cost Budget, các loại budget khác có thể không khả dụng ngay lập tức.

1. Đăng nhập vào **AWS Management Console** và tìm dịch vụ **Billing and Cost Management** tại thanh tìm kiếm.

2. Tại trang quản trị, chọn **Budgets** từ menu bên trái.

3. Nhấn vào nút **Create budget**.

![Billing Service](/images/2/0001.png?featherlight=false&width=90pc)

#### Thiết lập cấu hình Budget

4. Trong phần **Budget setup**:
   - Chọn **Customize** (tùy chỉnh)
   - Tại **Budget types**, chọn **Cost budget**
   - Nhấn **Next**

![Billing Service](/images/2/0002.png?featherlight=false&width=90pc)
![Billing Service](/images/2/00021.png?featherlight=false&width=90pc)

5. Trong giao diện **Set your budget**:
   - Tại **Budget name**, nhập **```Monthly```**

![Billing Service](/images/2/0003.png?featherlight=false&width=90pc)

   - **Period**: Chọn khoảng thời gian cho Budget:
     - **Daily** (Hàng ngày)
     - **Monthly** (Hàng tháng)
     - **Quarterly** (Hàng quý)
     - **Annually** (Hàng năm)
   
   - **Budget effective dates**:
     - **Recurring Budget**: Nếu bạn muốn Budget được lặp lại định kỳ
     - **Expiring Budget**: Nếu bạn chỉ muốn Budget được áp dụng một lần duy nhất
     
     💡 **Pro Tip**: Tất cả các múi giờ trong AWS Budget đều sử dụng chuẩn **UTC**.
   
   - **Specify your monthly budget**:
     - **Fixed**: Nếu bạn muốn ngân sách của mỗi kỳ hạn là giống nhau
     - **Monthly Budget Planning**: Nếu bạn muốn thiết lập ngân sách khác nhau cho từng tháng
     - **Budgeted amount**: Nhập số tiền tương ứng với ngân sách của bạn

![Billing Service](/images/2/0004.png?featherlight=false&width=90pc)

6. Tại phần **Budget scope**, chọn **All AWS services** để áp dụng ngân sách cho tất cả dịch vụ AWS. Sau đó nhấn **Next**.

![Create Cost Budget](/images/2/0005.png?featherlight=false&width=90pc)

#### Thiết lập cảnh báo

7. Trong phần **Configure alerts**, chọn **Add an alert threshold** để thiết lập ngưỡng cảnh báo. Nhấn **Next**.

![Create Cost Budget](/images/2/0006.png?featherlight=false&width=90pc)

8. Thực hiện cấu hình chi tiết cho **Alert** và chọn **Next**.

![Create Cost Budget](/images/2/0007.png?featherlight=false&width=90pc)

9. Xem lại các thiết lập hành động (nếu có) và chọn **Next**.

![Create Cost Budget](/images/2/0008.png?featherlight=false&width=90pc)

10. Xem lại toàn bộ cấu hình và chọn **Create budget** để hoàn tất.

![Create Cost Budget](/images/2/0009.png?featherlight=false&width=90pc)

11. Xác nhận Budget đã được tạo thành công.

![Create Cost Budget](/images/2/00010.png?featherlight=false&width=90pc)

#### Lợi ích của Cost Budget

ℹ️ **Information**: Cost Budget giúp bạn theo dõi chi phí AWS theo thời gian thực và nhận cảnh báo khi chi phí vượt quá ngưỡng đã thiết lập.

💡 **Pro Tip**: Nên thiết lập nhiều ngưỡng cảnh báo (ví dụ: 50%, 80%, 100%) để có thể chủ động trong việc kiểm soát chi phí.

🔒 **Security Note**: Đảm bảo thông báo cảnh báo được gửi đến những người có trách nhiệm và quyền hạn để có thể kịp thời xử lý khi chi phí vượt ngưỡng.
