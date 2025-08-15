---
title: "Kiến trúc Hệ thống"
date: "2024-03-20"
weight: 4
chapter: false
pre: " <b> 1.4 </b> "
---

Hệ thống tuân theo mô hình kiến trúc **Client – Server – Cloud**, kết hợp giữa các công nghệ thời gian thực (qua GetStream), RESTful API và hạ tầng cloud-native để đảm bảo khả năng mở rộng, hiệu suất và dễ bảo trì. Cả **backend** và **frontend** đều được triển khai trên nền tảng **AWS**.

### Các thành phần của hệ thống

#### Frontend – Giao diện người dùng (React.js)

- Giao diện người dùng tương tác (UI/UX)
- Giao tiếp với backend thông qua REST API và GetStream SDK
- Được triển khai bằng **AWS Amplify CI/CD**
- Các chức năng chính bao gồm:
  - Xác thực người dùng (đăng ký/đăng nhập)
  - Nhắn tin thời gian thực (1-1)
  - Truyền phát hoặc gọi video (qua GetStream Video)
  - Quản lý nhóm/kênh trò chuyện

#### Backend – Máy chủ (Node.js + Express.js)

- Xử lý logic lõi: xác thực, quản lý người dùng & nhóm, tích hợp chat, đồng bộ dữ liệu
- Sử dụng **Prisma ORM** để thao tác với **MongoDB**
- Được triển khai trên **Amazon EC2**

#### Cơ sở dữ liệu – MongoDB Atlas

- Cơ sở dữ liệu NoSQL lưu trữ trên cloud
- Lưu trữ thông tin người dùng, lịch sử chat, dữ liệu nhóm, phiên video
- Có khả năng mở rộng cao và tối ưu cho ứng dụng thời gian thực

#### Lưu trữ Media – Cloudinary

- Lưu trữ và phân phối nội dung media (ảnh, video) thông qua CDN
- Tích hợp với hệ thống chat để gửi avatar, chia sẻ hình ảnh, xem trước video, v.v.

---

### Sơ đồ hệ thống

#### Kiến trúc tổng thể (AWS Architecture)

![Kiến trúc tổng thể](/images/1.introduction/generalArchitecture.png)

### Quy trình hoạt động

![Sơ đồ tuần tự](/images/1.introduction/workflow.png)

---
