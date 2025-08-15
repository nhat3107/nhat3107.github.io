---
title: "Chuẩn Bị MongoDB"
date: "2025-07-30"
weight: 5
chapter: false
pre: " <b> 2.5 </b> "
---

### Tổng quan

**MongoDB** là một cơ sở dữ liệu **NoSQL** phổ biến, hướng tài liệu (_document-oriented_), được thiết kế để đạt hiệu năng cao, khả năng mở rộng và linh hoạt.  
Thay vì lưu trữ dữ liệu trong bảng và hàng như cơ sở dữ liệu quan hệ, MongoDB lưu trữ dữ liệu dưới dạng **tài liệu JSON-like** (định dạng **BSON**), cho phép cấu trúc lồng nhau và lược đồ động (_dynamic schema_).

MongoDB được sử dụng rộng rãi trong các ứng dụng hiện đại vì:

- Xử lý tốt khối lượng lớn dữ liệu không có cấu trúc hoặc bán cấu trúc.
- Dễ dàng mở rộng bằng **phân mảnh ngang (sharding)** và **nhân bản (replication)**.
- Tích hợp linh hoạt với nhiều ngôn ngữ lập trình và framework.

---

### Hướng dẫn

1. Truy cập MongoDB: https://www.mongodb.com/

   - Chọn **đăng nhập bằng Google**  
     ![MongoDB](/images/2.prerequisite/mongodb01.png)

2. Trong giao diện MongoDB

   - Chọn **Create**  
     ![MongoDB](/images/2.prerequisite/mongodb02.png)

3. Cấu hình cụm cơ sở dữ liệu (_cluster settings_)

   - Chọn phiên bản **Free**  
     ![MongoDB](/images/2.prerequisite/mongodb03.png)
   - Chọn **AWS Provider**
   - Chọn vùng (**Region**): **Hong Kong (ap-east-1)**  
     ![MongoDB](/images/2.prerequisite/mongodb04.png)

4. Cấu hình kết nối

   - Tạo **Database User**  
     ![MongoDB](/images/2.prerequisite/mongodb05.png)
   - Sao chép **Username** và **Password**
   - Nhấn **Choose a connection method**  
     ![MongoDB](/images/2.prerequisite/mongodb06.png)
   - Chọn **Drivers**  
     ![MongoDB](/images/2.prerequisite/mongodb07.png)
   - Sao chép **chuỗi kết nối** (_connection string_) và lưu lại để sử dụng sau  
     ![MongoDB](/images/2.prerequisite/mongodb08.png)

   - Chuỗi kết nối có dạng:

     ```
     mongodb+srv://<your_username>:<your_password>@cluster0.vbxyrhh.mongodb.net/<your_appname>?retryWrites=true&w=majority&appName=Cluster0
     ```

     Thay thế:

     - <your_username> : tên người dùng cơ sở dữ liệu
     - <your_password> : mật khẩu cơ sở dữ liệu
     - <your_appname> : tên cơ sở dữ liệu của bạn
