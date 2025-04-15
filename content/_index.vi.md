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
+ Cost Budget
+ Usage Budget
+ RI Budget
+ Savings Plans Budget

#### Cost Budget

**Cost Budget** cho phép bạn gửi cảnh báo khi tổng chi phí vượt qua ngưỡng chi phí trong ngân sách.

#### Usage Budget

**Usage Budget** cho phép bạn gửi cảnh báo khi tổng mức sử dụng **theo từng dịch vụ** bạn lựa chọn vượt qua ngưỡng mức sử dụng trong ngân sách.

ℹ️ **Information**: Ví dụ: Mức sử dụng theo số giờ chạy của dịch vụ EC2.

#### Reservation Instance (RI) Budget

**RI Budget** cho phép bạn gửi cảnh báo dựa trên mức sử dụng các dịch vụ trả trước (*reserve instance*) của bạn.

ℹ️ **Information**: **Reserve instance** là một phương pháp giảm chi phí sử dụng instance bằng cách cho phép bạn trả trước hoặc cam kết mức sử dụng của instance theo thời hạn 1 - 3 năm.

#### Savings Plans Budget

**Savings Plans Budget** cho phép bạn gửi cảnh báo dựa trên mức sử dụng các dịch vụ đã được quy định ở trong savings plans.

ℹ️ **Information**: **Savings plans** cũng là một phương pháp giảm chi phí sử dụng instance bằng cách cho phép bạn trả trước hoặc cam kết dài hạn (từ 01 đến 03 năm) mức sử dụng của instance đó. 
**Savings plans** là mô hình gia ra đời sau và linh hoạt hơn Reserve Instance với mức giảm giá tương đương. Với EC2 Instance, bạn được khuyến khích sử dụng Savings plans.

💡 **Pro Tip**: Sử dụng Savings Plans thay vì Reserved Instances cho EC2 sẽ mang lại sự linh hoạt cao hơn với cùng mức giảm giá.

#### Nội dung
1. [Tạo Cost Budget](1-cost-budgets)
2. [Tạo Usage Budget](2-usage-budget)
3. [Tạo RI Budget](3-reservation-budget)
4. [Tạo Savings Plans Budget](4-saving-plans-budget)
5. [Dọn Dẹp Tài Nguyên](5-clean-up)

#### Lợi ích của việc sử dụng AWS Budget

Việc sử dụng AWS Budget mang lại nhiều lợi ích cho doanh nghiệp:

1. **Kiểm soát chi phí**: Giúp bạn theo dõi và kiểm soát chi phí AWS một cách chủ động.
2. **Cảnh báo kịp thời**: Nhận thông báo ngay khi chi phí vượt quá ngưỡng đã thiết lập.
3. **Lập kế hoạch tài chính**: Hỗ trợ việc lập kế hoạch tài chính và dự báo chi phí trong tương lai.
4. **Tối ưu hóa tài nguyên**: Xác định các dịch vụ có chi phí cao để có thể tối ưu hóa việc sử dụng.
5. **Phân bổ chi phí**: Dễ dàng phân bổ chi phí cho các dự án, phòng ban hoặc khách hàng khác nhau.

#### Các bước thiết lập AWS Budget hiệu quả

1. **Xác định mục tiêu ngân sách**: Hiểu rõ nhu cầu và giới hạn chi tiêu của bạn.
2. **Phân tích chi phí hiện tại**: Xem xét chi phí hiện tại để thiết lập ngân sách hợp lý.
3. **Thiết lập ngưỡng cảnh báo**: Đặt ngưỡng cảnh báo ở mức phù hợp (thường là 80% và 100% ngân sách).
4. **Cấu hình thông báo**: Đảm bảo thông báo được gửi đến đúng người có thẩm quyền.
5. **Theo dõi và điều chỉnh**: Thường xuyên xem xét và điều chỉnh ngân sách khi cần thiết.
