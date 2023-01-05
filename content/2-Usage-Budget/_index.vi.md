---
title : "Tạo Usage Budget"
date :  "`r Sys.Date()`" 
weight : 3
chapter : false
pre : " <b> 3. </b> "
---

Ở phần này, bạn sẽ thực hành tạo một Usage Budget.

{{% notice note %}}
Nếu bạn đã làm qua phần [tạo Cost Budget](../1-cost-budgets), bạn sẽ thấy quy trình tạo Usage Budget cũng rất tương đồng, với một điểm khác nhau duy nhất là Cost Budget hoạt động dựa trên **chi phí**, còn Usage Budget hoạt động dựa trên **mức sử dụng**.

{{% /notice %}}

**Nội dung:**
- [Khởi tạo usage budget](#khởi-tạo-usage-budget)

#### Khởi tạo usage budget

1. Đăng nhập vào trang quản trị **AWS Management Console** và chọn dịch vụ **Billing** tại thanh tìm kiếm.

![Budget Name & Amount](/images/3/0001.png?featherlight=false&width=90pc)

2. Tại trang quản trị, chọn **Budgets**. 

![Budget Name & Amount](/images/3/0001.png?featherlight=false&width=90pc)

3. Chọn **Create budget**.

![Budget Name & Amount](/images/3/0001.png?featherlight=false&width=90pc)

4. Chọn **Budget type**

- Chọn **Customize**
- Chọn **Usage budget**

![Budget Name & Amount](/images/3/0002.png?featherlight=false&width=90pc)

5. Đặt tên budget.

![Budget Name & Amount](/images/3/0003.png?featherlight=false&width=90pc)

6. Chọn **Usage type groups**

- Chọn **EC2:Running Hours**

![Budget Name & Amount](/images/3/0004.png?featherlight=false&width=90pc)

7. Thực hiện **Set budget amount**

- Chọn **Period**
- Chọn **Budget renewal type**
- Chọn **Budgeting method**
- Nhập số giờ.

![Budget Name & Amount](/images/3/0005.png?featherlight=false&width=90pc)

8. Để mặc định và chọn **Next**

![Budget Name & Amount](/images/3/0006.png?featherlight=false&width=90pc)

9. Thực hiện cấu hình **Alert**

![Budget Name & Amount](/images/3/0007.png?featherlight=false&width=90pc)

10. Hoàn thành thông tin **Alert**

![Budget Name & Amount](/images/3/0008.png?featherlight=false&width=90pc)

11. Chọn **Next**

![Budget Name & Amount](/images/3/0009.png?featherlight=false&width=90pc)

12. Chọn **Create budget**

![Budget Name & Amount](/images/3/00010.png?featherlight=false&width=90pc)

13. Tao budget thành công.

![Budget Name & Amount](/images/3/00011.png?featherlight=false&width=90pc)

14. Kiểm tra **Budget health**

![Budget Name & Amount](/images/3/00012.png?featherlight=false&width=90pc)

15. Xem lại **Budget history**

![Budget Name & Amount](/images/3/00013.png?featherlight=false&width=90pc)