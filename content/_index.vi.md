---
title: "Phát Triển và Triển Khai"
date: "2024-03-20"
weight: 1
chapter: false
---

# Xây dựng Ứng dụng Chat & Video Streaming Thời Gian Thực bằng MERN Stack và Triển khai trên AWS

### Mục Tiêu Dự Án

Dự án này nhằm xây dựng một ứng dụng chat và video streaming thời gian thực sử dụng MERN Stack, đồng thời triển khai trên hạ tầng AWS. Ứng dụng kết hợp giao diện người dùng hiện đại với khả năng giao tiếp thời gian thực và triển khai an toàn trên nền tảng đám mây.

### Công Nghệ Sử Dụng

#### 🧑‍💻 Stack Phát Triển – MERN

- **Frontend**:

  - React.js

  - Tailwind CSS, DaisyUI

  - GetStream.io (xử lý chat và video thời gian thực)

- **Backend**:

  - Node.js + Express.js

  - Prisma ORM

  - MongoDB Atlas (cơ sở dữ liệu đám mây)

  - Cloudinary (lưu trữ và phân phối media)

#### ☁️ Stack Triển Khai – Dịch Vụ AWS

- **CI/CD cho Frontend**:

  - **AWS Amplify** – Tự động build, deploy và host giao diện React từ GitHub.

- **Backend**:

  - **EC2** – Tự động build và triển khai backend Express.js lên Amazon EC2.

#### 📂 Quản Lý Mã Nguồn

- **GitHub** – Quản lý source code và kích hoạt các quy trình CI/CD.

### Kết Quả Mong Đợi

- Một ứng dụng chat và video thời gian thực hoạt động đầy đủ.

- Giao diện người dùng hiện đại, mượt mà và phản hồi tốt trên mọi thiết bị.

- Một kiến trúc cloud-native có khả năng mở rộng cao, dễ bảo trì và nâng cấp trong tương lai.

### Nội dung

1.  [Giới thiệu ](1-introduce/)
2.  [Các bước chuẩn bị](2-prerequiste/)
3.  [Tạo Budget](3-budget)
4.  [Networking](4-networking/)
5.  [Amplify](5-amplify/)
6.  [CodePipeline](6-codepipeline/)
7.  [Kết quả đạt được](7-achievements/)
8.  [Dọn dẹp tài nguyên](8-cleanup/)
