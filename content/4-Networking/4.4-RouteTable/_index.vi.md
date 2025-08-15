---
title: "Route Table"
date: "2025-07-30"
weight: 4
chapter: false
pre: " <b> 4.4 </b> "
---

## Tổng quan

- **Route Table** (Bảng định tuyến) xác định cách lưu lượng mạng được điều hướng trong một VPC
- Nó quyết định đường đi của các gói tin giữa các subnet và internet
- Cho phép kiểm soát lưu lượng vào/ra của VPC

---

## Hướng dẫn

1. Truy cập dịch vụ **VPC**

   - Chọn **Route Tables** từ menu bên trái
   - Chọn Route Table của **CloudTalkr-VPC**  
     ![RTB](/images/4.networking/rtb01.png)

2. Thêm tuyến đường cho Internet Gateway

   - Nhấn **Actions**
   - Chọn **Edit routes**  
     ![RTB](/images/4.networking/rtb02.png)

3. Thêm tuyến đường mới

   - Nhấn **Add route**
   - **Destination**: Nhập `0.0.0.0/0` (đại diện cho internet)
   - **Target**: Chọn **Internet Gateway** và chọn IGW đã tạo trước đó
   - Nhấn **Save changes**  
     ![RTB](/images/4.networking/rtb03.png)
