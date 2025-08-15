---
title: "Subnet"
date: "2025-07-30"
weight: 2
chapter: false
pre: " <b> 4.2 </b> "
---

## Tổng quan

- **Subnet** là một phân đoạn mạng nhỏ hơn bên trong VPC
- Cho phép phân bổ tài nguyên trên các **Availability Zones (AZ)**

---

## Hướng dẫn

1. Truy cập dịch vụ **VPC**

   - Chọn **Subnets** từ menu bên trái
   - Nhấn **Create subnet**  
     ![Subnet](/images/4.networking/subnet01.png)

2. Chọn VPC

   - Trong màn hình **Create subnet**
   - Chọn VPC **CloudTalkr-VPC** đã tạo trước đó

3. Cấu hình subnet đầu tiên

   - **Subnet name**: Nhập `Public Subnet 1`
   - **Availability Zone**: Chọn **_ap-southeast-1a_**
   - **IPv4 CIDR block**: Nhập `10.0.0.0/24`
   - Nhấn **Create subnet**  
     ![Subnet](/images/4.networking/subnet02.png)

4. Xác nhận subnet đã được tạo thành công  
   ![Subnet](/images/4.networking/subnet03.png)

{{%notice info%}}
**Availability Zone (AZ)**: Tên hiển thị dễ đọc (ví dụ: ap-southeast-1a)
{{%/notice%}}

{{%notice info%}}
**AZ ID**: Mã định danh thực tế của AZ  
AWS ánh xạ tên AZ sang AZ ID khác nhau cho từng tài khoản để phân bổ tài nguyên đồng đều hơn.
{{%/notice%}}
