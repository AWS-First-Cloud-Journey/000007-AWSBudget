+++
title = "Bắt đầu với AWS Budget"
date = 2021
weight = 1
chapter = false
+++

# Quản lý chi phí với AWS Budget

#### Tổng quan

Ở bài lab này, bạn sẽ được tìm hiểu thêm về dịch vụ AWS Budget để giúp bạn quản lý chi phí trên tài khoản AWS của bạn. Quản lý chi phí là một việc quan trọng hàng đầu trong việc vận hành hệ thống của bạn trên Cloud. 

#### AWS Budget
**AWS Budget** là một dịch vụ cung cấp khả năng thiết lập ngân sách để gửi cảnh báo cho bạn khi chi phí vượt quá chi phí mà ngân sách cho phép (hoặc được dự báo sẽ vượt quá ngân sách). 

AWS Budget bao gồm 4 loại budget: 
+ Cost Budget.
+ Usage Budget.
+ RI Budget.
+ Savings Plans Budget.

#### Cost Budget
**Cost Budget** cho phép bạn gửi cảnh báo khi tổng chi phí vượt qua ngưỡng chi phí trong ngân sách. 

#### Usage Budget
**Usage Budget** cho phép bạn gửi cảnh báo khi tổng mức sử dụng **theo từng dịch vụ** bạn lựa chọn vượt qua ngưỡng mức sử dụng trong ngân sách.

Ví dụ: Mức sử dụng theo số giờ chạy của dịch vụ EC2.

#### Reservation Instance (RI) Budget
**RI Budget** cho phép bạn gửi cảnh báo dựa trên mức sử dụng các dịch vụ trả trước (*reserve instance*) của bạn.

{{% notice info %}}
**Reserve instance** là một phương pháp giảm chi phí sử dụng instance bằng cách cho phép bạn trả trước hoặc cam kết mức sử dụng  của instance theo thời hạn 1 - 3 năm.
{{% /notice %}}

#### Savings Plans Budget
**Savings Plans Budget** cho phép bạn gửi cảnh báo dựa trên mức sử dụng các dịch vụ đã được quy định ở trong savings plans.

{{% notice info %}}
**Savings plans instance** cũng là một phương pháp giảm chi phí sử dụng instance bằng cách cho phép bạn trả trước hoặc cam kết dài hạn (từ 01 đến 03 năm) mức sử dụng của instance đó. 
**Savings plans** là mô hình gia ra đời sau và linh hoạt hơn Reserve Instance với mức giảm giá tương đương. Với EC2 Instance, bạn được khuyến khích sử dụng Savings plans.
{{% /notice %}}

#### Nội dung
1. [Tạo Cost Budget](1-cost-budgets)
2. [Tạo Usage Budget](2-usage-budget)
3. [Tạo RI Budget](3-reservation-budget)
4. [Tạo Savings Plans Budget](4-saving-plans-budget)
5. [Dọn Dẹp Tài Nguyên](5-clean-up)