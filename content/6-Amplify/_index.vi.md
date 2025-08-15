---
title: "Amplify"
date: "2025-07-30"
weight: 6
chapter: false
pre: " <b> 6. </b> "
---

1. Truy cập **AWS Management Console**

- Tìm kiếm **AWS Amplify**
- Chọn **AWS Amplify** từ kết quả tìm kiếm  
  ![Amplify](/images/6.amplify/amplify01.png)  
  ![Amplify](/images/6.amplify/amplify02.png)

---

2. Nhấn **Deploy An App**

- Bắt đầu xây dựng với Amplify:

  - Chọn **GitHub**
  - Nhấn **Next**  
    ![Amplify](/images/6.amplify/amplify03.png)

- Thêm repository và branch:

  - Chọn repo **CloudTalkr**
  - Tick **My app is a monorepo**
  - **Monorepo root directory**: `frontend`
  - Nhấn **Next**  
    ![Amplify](/images/6.amplify/amplify04.png)

- Cài đặt ứng dụng:

  - **Key**: `VITE_BACKEND_URL`
  - **Value**: _< Public IPv4 Address :3000>_
  - Nhấn **Next**  
    ![Amplify](/images/6.amplify/amplify05.png)  
    ![Amplify](/images/6.amplify/amplify06.png)

- Xem lại cấu hình:
- Nhấn **Save and Deploy**

  ![Amplify](/images/6.amplify/amplify07.png)  
  ![Amplify](/images/6.amplify/amplify08.png)

  ![Amplify](/images/6.amplify/amplify09.png)

---

{{% notice warning %}}
Mở EC2 và thêm: `FRONTEND_URL=<Amplify_Url>` vào file `.env`
{{% /notice %}}
