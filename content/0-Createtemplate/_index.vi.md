+++
title = "Tạo Budget"
date = 2024
weight = 1
chapter = false
pre = " <b> 1. </b> "
+++

#### Tổng quan

Trong phần này, bạn sẽ học cách tạo AWS Budget sử dụng template có sẵn của AWS. AWS Budget là công cụ quan trọng giúp bạn theo dõi và kiểm soát chi phí AWS một cách hiệu quả.

#### Tạo Budget theo template

1. Truy cập vào AWS Management Console:
   - Mở [AWS Management Console](https://ap-southeast-1.console.aws.amazon.com/console/home?region=ap-southeast-1)
   - Tìm và chọn dịch vụ **AWS Billing and Cost Management**

![AWS Budget](/images/1/0001.png?featherlight=false&featherlight=false&width=90pc)

2. Trong giao diện **AWS Billing and Cost Management**:
   - Chọn **Budgets** từ menu bên trái
   - Nhấn vào **Create a budget**

![AWS Budget](/images/1/0002.png?featherlight=false&featherlight=false&width=90pc)

3. Thiết lập cấu hình Budget:
   - Chọn **Use a template (simplified)** để sử dụng mẫu có sẵn
   - Trong phần **Templates**, chọn **Monthly cost budget**

![AWS Budget](/images/1/0003.png?featherlight=false&featherlight=false&width=90pc)

4. Nhập thông tin chi tiết cho Budget:
   - Đặt tên cho Budget
   - Xác định số tiền ngân sách hàng tháng
   - Thiết lập ngưỡng cảnh báo
   - Nhấn **Create budget** để hoàn tất

![AWS Budget](/images/1/0004.png?featherlight=false&featherlight=false&width=90pc)

![AWS Budget](/images/1/00041.png?featherlight=false&featherlight=false&width=90pc)

5. Xác nhận Budget đã được tạo thành công:

![AWS Budget](/images/1/0005.png?featherlight=false&featherlight=false&width=90pc)

6. Xem danh sách các Budget đã tạo:

![AWS Budget](/images/1/00060.png?featherlight=false&featherlight=false&width=90pc)

![AWS Budget](/images/1/0006.png?featherlight=false&featherlight=false&width=90pc)

7. Xem chi tiết Budget trong tab **Overview**:

![AWS Budget](/images/1/0008.png?featherlight=false&featherlight=false&width=90pc)

8. Kiểm tra tình trạng Budget và các cảnh báo:

![AWS Budget](/images/1/0005.png?featherlight=false&featherlight=false&width=90pc)

9. Xem lịch sử Budget:

![AWS Budget](/images/1/00060.png?featherlight=false&featherlight=false&width=90pc)

![AWS Budget](/images/1/0006.png?featherlight=false&featherlight=false&width=90pc)

10. Kiểm tra các loại cảnh báo có sẵn trong template:

![AWS Budget](/images/1/00011.png?featherlight=false&featherlight=false&width=90pc)

#### Lợi ích của việc sử dụng AWS Budget Templates

ℹ️ **Information**: AWS Budget Templates giúp đơn giản hóa quá trình tạo ngân sách bằng cách cung cấp các cấu hình được định nghĩa trước cho các trường hợp sử dụng phổ biến.

💡 **Pro Tip**: Sử dụng Monthly cost budget là lựa chọn tốt để bắt đầu, nhưng hãy cân nhắc tạo thêm các budget theo dịch vụ cụ thể khi hệ thống của bạn phát triển.

🔒 **Security Note**: Đảm bảo thiết lập quyền truy cập phù hợp cho AWS Budget để chỉ những người có thẩm quyền mới có thể chỉnh sửa hoặc xóa các budget đã tạo.

⚠️ **Warning**: Các cảnh báo budget không tự động dừng tài nguyên hoặc ngăn chặn việc sử dụng dịch vụ khi vượt quá ngân sách. Hãy cân nhắc kết hợp với AWS Service Quotas hoặc IAM policies để kiểm soát việc sử dụng tài nguyên.