---
title: "Triển khai Backend"
date: "2025-07-30"
weight: 2
chapter: false
pre: " <b> 5.2 </b> "
---

### Chuẩn bị môi trường

- Cài đặt NVM (Node Version Manager).

```
    curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.7/install.sh |
```

![Backend](/images/5.ec2/backend01.png)

- Reload shell để dùng nvm:

```
    . ~/.nvm/nvm.sh
```

- Cài đặt phiên bản mới nhất của Node.js:

```
    nvm install node
```

- Kiểm tra phiên bản:

```
   node -v
```

```
   npm -v
```

![Backend](/images/5.ec2/backend02.png)

### cài Đặt Git và Clone Code

- Update hệ thống and cài đặt Git:

```
   sudo yum update -y
```

```
   sudo yum install git -y
```

Kiểm tra phiên bản:

```
    git --version
```

![Backend](/images/5.ec2/backend03.png)

- Clone source code từ GitHub:

```
    git clone https://github.com/nhat3107/CloudTalkr.git
```

- Di chuyển tới thư mục backend:

```bash
   ls
```

```
   cd CloudTalkr/backend
```

![Backend](/images/5.ec2/backend04.png)

---

### Cài Đặt và Chạy Server

- Cài đặt npm packages cho backend:

```
    npm i
```

- Tạo file .env - Dán các **the API keys**, **Database Url**,...
  ![Backend](/images/5.ec2/backend05.png)
  ![Backend](/images/5.ec2/backend06.png)
- Chạy server dùng file .env vừa tạo:

```
    npm run start
```

![Backend](/images/5.ec2/backend08.png)

- Cài đặt PM2 để quản lý NodeJs processes:

```
    npm i pm2 -g
```

- Bật PM2 auto-start trên system boot bằng câu lệnh:

```
    pm2 startup
```

- Dán phần hiện ra vào terminal của EC2 và chạy.

- Chạy server bằng PM2, kiểm tra status, và monitor:

```
   pm2 start ecosystem.config.cjs
```

![Backend](/images/5.ec2/backend07.png)

```
   pm2 status
```

![Backend](/images/5.ec2/backend09.png)

```
    pm2 monit
```

![Backend](/images/5.ec2/backend10.png)

- Dừng và xóa tất cả PM2 processes hiện tại:

```
   pm2 stop all
```

```
   pm2 delete all
```

![Backend](/images/5.ec2/backend11.png)

- Khởi động lại server bằng config:

```
    pm2 start ecosystem.config.cjs
```

![Backend](/images/5.ec2/backend12.png)

- Kiểm tra API
  ![Backend](/images/5.ec2/backend13.png)
