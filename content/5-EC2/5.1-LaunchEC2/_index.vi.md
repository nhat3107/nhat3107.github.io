---
title: "Khởi Chạy EC2"
date: "2025-07-30"
weight: 1
chapter: false
pre: " <b> 5.1 </b> "
---

## Cấu hình Instance

1. Truy cập **EC2 Dashboard**

   - Tìm kiếm dịch vụ **EC2**

   - Chọn **EC2** từ kết quả tìm kiếm
     ![EC2](/images/5.ec2/ec201.png)

2. Khởi chạy một Instance mới

   - Chọn **Instances** từ menu bên trái

   - Nhấn **Launch instances**
     ![EC2](/images/5.ec2/ec202.png)

3. Đặt tên cho Instance

   - Trong mục **Name and tags**, nhập `cloudtalkr-server`
     ![EC2](/images/5.ec2/ec203.png)

4. Chọn Amazon Machine Image (AMI)

   - Chọn **Quick Start**

   - Chọn **Amazon Linux 2023 kernel-6.1**

   - Chọn phiên bản AMI phù hợp
     ![EC2](/images/5.ec2/ec204.png)

5. Cấu hình Loại Instance và Key Pair

   - Chọn **Instance type** phù hợp

   - Nhấn **Create new key pair**
     ![EC2](/images/5.ec2/ec205.png)

6. Tạo Key Pair mới

   - **Key pair name**: `cloudtalkr-keypair`

   - **Key pair type**: Chọn **RSA**

   - **Private key format**: Chọn **.pem**
     ![EC2](/images/5.ec2/ec206.png)

#### Cấu hình Mạng

7. Cấu hình Network

   - **VPC**: Chọn **CloudTalkr-VPC**

   - **Subnet**: Chọn **_Public Subnet 1_**

   - **Auto-assign public IP**: Chọn **_Enable_**

   - **Security Group**: Chọn **Create Security Group**

   - **Security Group Name**: `CloudTalkr-sg`

   - **Description**: `CloudTalkr Security Group`

     ![EC2](/images/5.ec2/ec207.png)
     ![EC2](/images/5.ec2/ec208.png)

   - Đảm bảo thiết lập các **Inbound Rules** cần thiết

{{% notice warning %}}
Nhớ mở Custom TCP cho PORT 3000 từ 0.0.0.0: chỉ dùng cho lab/test, nguy hiểm khi dùng môi trường production
{{% /notice %}}

- Nhấn **Launch instance**

8. Xác nhận Instance đã được khởi tạo thành công
   ![EC2](/images/5.ec2/ec209.png)

#### Kết nối

Truy cập dịch vụ **EC2**:

{{% notice note %}}
Có nhiều công cụ khác nhau có thể dùng để kết nối, nhưng trong bài lab này sử dụng MobaXterm.
{{% /notice %}}

[Hướng dẫn sử dụng MobaXterm tại đây](https://000004.awsstudygroup.com/vi/4-launchlinuxinstance/4.2-connectlinuxinstance/)

- Chọn **Instances**

- Chọn _**cloudtalkr-server**_
  ![EC2](/images/5.ec2/ec210.png)
- Sao chép **Public IP** và kết nối đến Instance này
  ![EC2](/images/5.ec2/ec211.png)
  ![EC2](/images/5.ec2/ec212.png)
