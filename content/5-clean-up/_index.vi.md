+++
title = "Dọn Dẹp Tài nguyên"
date = 2024
weight = 6
chapter = false
pre = " <b> 6. </b> "
+++

#### Tổng quan

⚠️ **Warning**: Việc cài đặt budget là một hoạt động quan trọng khi quản lý tài nguyên và vận hành trên môi trường điện toán đám mây AWS. Tuy nhiên, nếu bạn chỉ đang thực hành trên môi trường lab để hiểu tính năng, bạn nên thực hiện các thao tác dọn dẹp tài nguyên dưới đây để xóa các mức cảnh báo đã thiết lập, tránh nhận thông báo không cần thiết.

#### Xóa AWS Budgets

1. Đăng nhập vào **AWS Management Console** và tìm dịch vụ **AWS Billing and Cost Management** tại thanh tìm kiếm.

2. Tại trang quản trị, chọn **Budgets** từ menu bên trái.

3. Thực hiện xóa budget:
   - Chọn **Budget** cần xóa
   - Nhấn vào nút **Delete**

![Xóa Budget](/images/5/z0009.png?featherlight=false&width=90pc)

4. Trong hộp thoại xác nhận, nhấn **Delete** để hoàn tất việc xóa budget.

![Xác nhận xóa Budget](/images/5/z00010.png?featherlight=false&width=90pc)

5. Lặp lại các bước trên với tất cả các Budget còn lại mà bạn đã tạo trong quá trình thực hành.

ℹ️ **Information**: Việc xóa AWS Budgets không ảnh hưởng đến tài nguyên đang chạy trong tài khoản AWS của bạn. Các budget chỉ là công cụ giám sát và cảnh báo, không kiểm soát trực tiếp việc sử dụng tài nguyên.

💡 **Pro Tip**: Nếu bạn dự định sử dụng AWS trong môi trường thực tế, hãy cân nhắc việc thiết lập lại các budget phù hợp với nhu cầu thực tế của bạn sau khi hoàn thành bài lab này.