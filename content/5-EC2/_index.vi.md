---
title: "EC2"
date: "2025-07-30"
weight: 5
chapter: false
pre: " <b> 5. </b> "
---

## Tổng quan

Amazon EC2 (Elastic Compute Cloud) là dịch vụ máy chủ ảo của AWS, cho phép bạn chạy ứng dụng một cách linh hoạt và theo nhu cầu. Trong dự án này, EC2 được sử dụng để triển khai ứng dụng backend.

Các bước chính bao gồm:

- **Khởi tạo một EC2 instance**: Chọn hệ điều hành, cấu hình thông số phần cứng, tạo key pair và gắn instance vào mạng VPC phù hợp.

- **Kết nối và thiết lập môi trường**: Sử dụng SSH để truy cập instance, cài đặt Node.js, Git và các thư viện cần thiết để chạy backend Node.js.

- **Quản lý tiến trình với PM2**: Chạy máy chủ ở chế độ nền và kích hoạt tự khởi động lại khi hệ thống reboot.
