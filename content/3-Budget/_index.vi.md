---
title: "Tạo Budget"
date: "2024-07-30"
weight: 3
chapter: false
pre: " <b> 3. </b> "
---

## Tổng quan

Trong phần này, bạn sẽ học cách tạo AWS Budget sử dụng template có sẵn của AWS. AWS Budget là công cụ quan trọng giúp bạn theo dõi và kiểm soát chi phí AWS một cách hiệu quả.
Tạo Budget theo template

## Tạo Budget theo template

1. Truy cập vào **AWS Management Console**:

   - Mở **AWS Management Console**

   - Tìm và chọn dịch vụ **AWS Billing and Cost Management**

   ![Budget](/images/3.budget/budget01.png)
   ![Budget](/images/3.budget/budget02.png)

2. Trong giao diện **AWS Billing and Cost Management**:

   - Chọn **Budgets** từ menu bên trái

   - Nhấn vào **Create a budget**
     ![Budget](/images/3.budget/budget03.png)

3. Thiết lập cấu hình Budget:

   - Chọn **Use a template (simplified)** để sử dụng mẫu có sẵn

   - Trong phần **Templates**, chọn **Monthly cost budget**
     ![Budget](/images/3.budget/budget04.png)

4. Nhập thông tin chi tiết cho Budget:

   - Đặt tên cho **Budget**

   - **Xác định số tiền** ngân sách hàng tháng

   - Thiết lập **ngưỡng cảnh báo**

   - Nhấn **Create budget** để hoàn tất
     ![Budget](/images/3.budget/budget05.png)

5. **Xác nhận Budget** đã được tạo thành công:

## Lợi ích của việc sử dụng AWS Budget Templates

{{% notice info %}}
AWS Budget Templates giúp đơn giản hóa quá trình tạo ngân sách bằng cách cung cấp các cấu hình được định nghĩa trước cho các trường hợp sử dụng phổ biến.
{{% /notice %}}

{{% notice tip %}}
Sử dụng Monthly cost budget là lựa chọn tốt để bắt đầu, nhưng hãy cân nhắc tạo thêm các budget theo dịch vụ cụ thể khi hệ thống của bạn phát triển.
{{% /notice %}}

{{% notice note %}}
Đảm bảo thiết lập quyền truy cập phù hợp cho AWS Budget để chỉ những người có thẩm quyền mới có thể chỉnh sửa hoặc xóa các budget đã tạo.
{{% /notice %}}

{{% notice warning %}}
Các cảnh báo budget không tự động dừng tài nguyên hoặc ngăn chặn việc sử dụng dịch vụ khi vượt quá ngân sách. Hãy cân nhắc kết hợp với AWS Service Quotas hoặc IAM policies để kiểm soát việc sử dụng tài nguyên.
{{% /notice %}}
