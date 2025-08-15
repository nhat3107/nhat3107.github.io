+++
title = "Dọn dẹp tài nguyên  "
date = 2021
weight = 9
chapter = false
pre = "<b>9. </b>"
+++

Chúng ta sẽ thực hiện các bước sau để xóa các tài nguyên đã tạo trong bài thực hành này.

---

## Xóa Amplify

1. Truy cập **AWS Amplify Console**

   - Mở [AWS Amplify Console](https://console.aws.amazon.com/amplify/home#)
   - Trong danh sách ứng dụng, chọn ứng dụng bạn muốn xóa

2. Mở phần cài đặt ứng dụng

   - Tại trang chi tiết ứng dụng, chọn tab **App settings**
   - Nhấn **General** để xem các cài đặt chung

3. Xóa ứng dụng

   - Cuộn xuống và nhấn **Delete app**
   - Nhập tên ứng dụng để xác nhận
   - Nhấn **Delete** để hoàn tất  
     ![Clean Amplify](/images/9.clean/cleanamplify.png)

---

## Xóa EC2 instance

1. Truy cập [Bảng điều khiển quản lý EC2](https://console.aws.amazon.com/ec2/v2/home)

   - Nhấn **Instances**
   - Chọn instance
   - Nhấn **Instance state**
   - Chọn **Terminate instance**, sau đó nhấn **Terminate** để xác nhận  
     ![Clean EC2](/images/9.clean/cleanec2.png)
   - Sau đó chuyển sang **Security Group** và xóa **Security Group** của EC2  
     ![Clean SG](/images/9.clean/cleansecuritygroup.png)

---

## Xóa API Gateway

1. Truy cập **Amazon API Gateway**

   - Mở [API Gateway Console](https://console.aws.amazon.com/apigateway)
   - Chọn **APIs** ở thanh điều hướng bên trái

2. Chọn API để xóa

   - Tìm API bạn muốn xóa (HTTP, REST hoặc WebSocket)
   - Nhấn vào tên API để mở chi tiết

3. Thực hiện xóa

   - Nhấn **Actions > Delete**
   - Nhập tên API để xác nhận (nếu được yêu cầu)
   - Nhấn **Delete** để hoàn tất  
     ![Clean API](/images/9.clean/cleanapi.png)

---

## Xóa VPC

1. Truy cập [Bảng điều khiển quản lý VPC](https://console.aws.amazon.com/vpc/home)

   - Nhấn **Your VPCs**
   - Chọn **Lab VPC**
   - Nhấn **Actions**
   - Chọn **Delete VPC**

2. Trong hộp xác nhận, nhập **delete** để xác nhận, sau đó nhấn **Delete** để xóa **Lab VPC** và các tài nguyên liên quan (Subnets, Internet Gateway,...)  
   ![Clean VPC](/images/9.clean/cleanvpc.png)
