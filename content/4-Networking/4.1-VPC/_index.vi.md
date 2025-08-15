---
title: "VPC"
date: "2025-07-30"
weight: 1
chapter: false
pre: " <b> 4.1 </b> "
---

## Mục tiêu

- Tạo một môi trường mạng ảo riêng biệt trong AWS
- Xác định dải địa chỉ IP cho VPC
- Cấu hình các tính năng DNS cơ bản

---

## Hướng dẫn

1. Truy cập **AWS Management Console**

   - Tìm kiếm dịch vụ **VPC**
   - Chọn **VPC** từ kết quả tìm kiếm  
     ![VPC](/images/4.networking/vpc01.png)

2. Trong **VPC Dashboard**

   - Chọn **Your VPCs** từ menu bên trái
   - Nhấn **Create VPC**  
     ![VPC](/images/4.networking/vpc02.png)

3. Cấu hình thông số VPC

   - **Resources**: Chọn **VPC only**
   - **Name tag**: Nhập `CloudTalkr-VPC`
   - **IPv4 CIDR**: Nhập `10.0.0.0/16`

{{% notice note %}}
Giữ nguyên tùy chọn **Tenancy** là **Default**. Chuyển sang **Dedicated** có thể giới hạn loại EC2 Instance được hỗ trợ trong VPC này.
{{% /notice %}}

4. Xác nhận tạo VPC

   - Nhấn **Create VPC** để hoàn tất  
     ![VPC](/images/4.networking/vpc03.png)

5. Kiểm tra trạng thái VPC sau khi tạo  
   ![VPC](/images/4.networking/vpc04.png)

6. Bật các tính năng DNS cho VPC

   - Nhấn **Edit VPC settings**
   - Chuyển sang tab **DNS settings**
   - Bật **DNS hostnames** và **DNS resolution**
   - Lưu thay đổi  
     ![VPC](/images/4.networking/vpc05.png)
