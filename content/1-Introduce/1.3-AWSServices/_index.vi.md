---
title: "Dịch Vụ Của AWS"
date: "2025-07-30"
weight: 3
chapter: false
pre: " <b> 1.3 </b> "
---

### 🔧 1. AWS Amplify

![Amplify](/images/1.introduction/amplify.png)
**Mục đích**: Triển khai và tự động hóa CI/CD cho frontend (React.js)

**Chức năng**:

- Tự động build & deploy frontend từ GitHub.

- Hỗ trợ preview từng pull request.

- Cấu hình môi trường (dev, staging, production) dễ dàng.

---

### 🖥 2. Amazon EC2 (Elastic Compute Cloud)

![EC2](/images/1.introduction/ec2.png)
**Mục đích**: Chạy server backend (Node.js + Express).

**Chức năng**:

- Tạo máy chủ ảo (instance) có thể cấu hình linh hoạt.

- Triển khai backend thủ công hoặc tự động từ CodePipeline.

- Dễ dàng mở rộng hoặc thu nhỏ tài nguyên theo tải thực tế.

---

### 🔄 3. Amazon API Gateway

![API Gateway](/images/1.introduction/amazon-API-Gateway.png)
**Mục đích**: Quản lý và định tuyến các yêu cầu API giữa frontend và backend.

**Chức năng**:

- Tạo, quản lý và bảo mật các endpoint API cho ứng dụng.
- Hỗ trợ REST API và WebSocket API, phù hợp cho giao tiếp thời gian thực.
- Kết hợp với backend chạy trên EC2 để xử lý yêu cầu.

---
