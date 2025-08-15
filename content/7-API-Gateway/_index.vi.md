---
title: "API Gateway"
date: "2025-07-30"
weight: 7
chapter: false
pre: " <b> 7. </b> "
---

1. Truy cập **AWS Management Console**

- Tìm kiếm **API Gateway**
- Chọn **API Gateway** từ kết quả tìm kiếm  
  ![API Gateway](/images/7.apigateway/api01.png)  
  ![API Gateway](/images/7.apigateway/api02.png)

---

2. Điều hướng đến phần **REST API**

- Nhấn **Build**  
  ![API Gateway](/images/7.apigateway/api03.png)

---

3. Tạo một REST API

- Chọn **New API**
- **API name**: `cloudtalkr-API`
- Nhấn **Create API**  
  ![API Gateway](/images/7.apigateway/api04.png)

---

4. Mở phần **Resources**  
   ![API Gateway](/images/7.apigateway/api05.png)

---

5. Nhấn **Create Resource**

- Bật **Proxy Resource**
- **Resource name**: `{proxy+}`
- Tick **CORS (Cross-Origin Resource Sharing)**
- Nhấn **Create Resource**  
  ![API Gateway](/images/7.apigateway/api06.png)  
  ![API Gateway](/images/7.apigateway/api07.png)  
  ![API Gateway](/images/7.apigateway/api08.png)

---

6. Trong phần **Resource Methods**

- Chọn **ANY**
- Nhấn **Edit integration**
  - **Integration Type**: `HTTP`
  - Bật **HTTP proxy integration**
  - **HTTP Method**: `ANY`
  - **Endpoint URL**: `<Public IPv4 Address>/{proxy}`
  - **Content handling**: `Passthrough`
- Nhấn **Save**  
  ![API Gateway](/images/7.apigateway/api09.png)  
  ![API Gateway](/images/7.apigateway/api10.png)

---

7. Triển khai API

- **Stage**: _New stage_
- **Stage name**: `prod`
- Nhấn **Deploy**  
  ![API Gateway](/images/7.apigateway/api11.png)  
  ![API Gateway](/images/7.apigateway/api12.png)

---

8. Kiểm tra API  
   ![API Gateway](/images/7.apigateway/api13.png)

   {{% notice note %}}
   API hoạt động đúng nhưng bị chặn bởi middleware
   {{% /notice %}}

---

9. Truy cập lại **AWS Management Console**

- Tìm kiếm **AWS Amplify**
- Chọn **AWS Amplify** từ kết quả tìm kiếm

---

10. Nhấn **View app - CloudTalkr**
    ![API Gateway](/images/7.apigateway/api14.png)

---

11. Mở **Environment Variables**

- Nhấn **Manage Variables**
  ![API Gateway](/images/7.apigateway/api15.png)

- Cập nhật **Value** của biến **VITE_BACKEND_URL**
- Nhấn **Save**  
  ![API Gateway](/images/7.apigateway/api16.png)

---

12. Vào **Overview**

- Nhấn **Redeploy this version**  
  ![API Gateway](/images/7.apigateway/api17.png)
