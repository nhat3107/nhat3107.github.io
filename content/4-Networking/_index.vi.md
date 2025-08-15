---
title: "Thiết Lập Mạng"
date: "2024-03-20"
weight: 4
chapter: false
pre: " <b> 4. </b> "
---

## 🛰️ Tổng quan về AWS Networking

Hệ thống **AWS Networking** được xây dựng dựa trên **VPC (Virtual Private Cloud)** – một mạng ảo được cô lập logic trong môi trường đám mây AWS.  
Việc thiết lập các thành phần mạng cốt lõi như **VPC**, **Subnet**, **Internet Gateway** và **Route Table** là nền tảng để triển khai an toàn các dịch vụ như EC2 và nhiều dịch vụ khác.

---

### **VPC – Virtual Private Cloud**

- Hoạt động như một mạng riêng trong AWS.
- Cho phép bạn định nghĩa dải địa chỉ IP, cài đặt DNS, quyền truy cập và các quy tắc định tuyến.
- Là lớp cơ sở chứa các subnet, gateway và các tài nguyên bảo mật.

---

### **Subnet – Phân đoạn mạng**

- Chia VPC thành các không gian địa chỉ nhỏ hơn, phân bố trên các **Availability Zones (AZs)**.
- Có thể được cấu hình là **Public** (truy cập internet) hoặc **Private** (chỉ nội bộ).
- Cho phép bố trí tài nguyên như EC2 và RDS một cách logic và an toàn.

---

### **Internet Gateway (IGW)**

- Cổng kết nối VPC với internet.
- Phải được gắn vào VPC để cho phép subnet công khai giao tiếp ra ngoài.
- Hỗ trợ giao tiếp hai chiều cho các tài nguyên có thể truy cập từ internet.

---

### **Route Table – Bảng định tuyến**

- Xác định cách lưu lượng mạng được định tuyến trong VPC.
- Ánh xạ lưu lượng tới các đích như **Internet Gateway**, các subnet khác hoặc kết nối VPN.
- Mỗi subnet phải được liên kết với một bảng định tuyến phù hợp với chức năng của nó (public/private).

---

### ✅ Tóm tắt

| Thành phần           | Mô tả                                                                    |
| -------------------- | ------------------------------------------------------------------------ |
| **VPC**              | Mạng riêng được cô lập, chứa tất cả các tài nguyên mạng khác             |
| **Subnet**           | Chia nhỏ VPC và giới hạn phạm vi hiển thị/truy cập của tài nguyên        |
| **Internet Gateway** | Kết nối VPC với internet để giao tiếp vào/ra                             |
| **Route Table**      | Kiểm soát luồng dữ liệu bằng cách định nghĩa đường đi trong và ngoài VPC |
