---
title: "Internet Gateway"
date: "2025-07-30"
weight: 3
chapter: false
pre: " <b> 4.3 </b> "
---

## Hướng dẫn

1. Truy cập dịch vụ **VPC**

   - Chọn **Internet Gateways** từ menu bên trái
   - Nhấn **Create internet gateway**  
     ![IGW](/images/4.networking/IGW01.png)

2. Cấu hình Internet Gateway

   - Trong trường **Name tag**, nhập `CloudTalkr-IGW`
   - Nhấn **Create internet gateway**  
     ![IGW](/images/4.networking/IGW02.png)

3. Xác nhận Internet Gateway đã được tạo thành công  
   ![IGW](/images/4.networking/IGW03.png)

#### Gắn vào VPC

4. Gắn Internet Gateway vào VPC của bạn

   - Nhấn **Actions**
   - Chọn **Attach to VPC**
   - Chọn VPC **CloudTalkr-VPC** từ danh sách thả xuống (VPC ID sẽ tự động điền)
   - Nhấn **Attach internet gateway**  
     ![IGW](/images/4.networking/IGW04.png)

#### Xác nhận trạng thái

5. Sau khi gắn thành công:

   - **State** của Internet Gateway sẽ chuyển sang **Attached**
   - IGW đã sẵn sàng để định tuyến lưu lượng internet cho VPC của bạn  
     ![IGW](/images/4.networking/IGW05.png)
