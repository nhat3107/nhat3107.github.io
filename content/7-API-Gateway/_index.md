---
title: "API Gateway"
date: "2025-07-30"
weight: 7
chapter: false
pre: " <b> 7. </b> "
---

1. Access AWS Management Console

- Search for **API Gateway**
- Select **API Gateway** from the search results
  ![API Gateway](/images/7.apigateway/api01.png)
  ![API Gateway](/images/7.apigateway/api02.png)

2. Navigate to the REST API section

- Click **Build**
  ![API Gateway](/images/7.apigateway/api03.png)

3. Create a REST API

- Select **New API**
- **API name**: `cloudtalkr-API`
- Click **Create API**
  ![API Gateway](/images/7.apigateway/api04.png)

4. Navigate to the **Resources** section
   ![API Gateway](/images/7.apigateway/api05.png)
5. Click **Create Resource**

- Enable **Proxy Resource**
- **Resource name**: `{proxy+}`
- Check **CORS (Cross-Origin Resource Sharing)**
- Click **Create Resource**
  ![API Gateway](/images/7.apigateway/api06.png)
  ![API Gateway](/images/7.apigateway/api07.png)
  ![API Gateway](/images/7.apigateway/api08.png)

6. In the Resource Methods

- Choose **ANY**

- Click **Edit integration**
  - **Integration Type**: `HTTP`
  - Enable **HTTP proxy integration**
  - **HTTP Method**: `ANY`
  - **Endpoint URL**: `<Public IPv4 Address>/{proxy}`
  - **Content handling**: `Passthrough`
- Click **Save**
  ![API Gateway](/images/7.apigateway/api09.png)
  ![API Gateway](/images/7.apigateway/api10.png)

7. Deploy the API

- **Stage**: _New stage_
- **Stage name**: `prod`
- Click **Deploy**
  ![API Gateway](/images/7.apigateway/api11.png)
  ![API Gateway](/images/7.apigateway/api12.png)

8. Test the API
   ![API Gateway](/images/7.apigateway/api13.png)

   {{% notice note %}}
   API run correctly because be prevented by middleware
   {{% /notice %}}

9. Access AWS Management Console

- Search for **AWS Amplify**
- Select **AWS Amplify** from the search results

10. Click **View app - CloudTalkr**
    ![API Gateway](/images/7.apigateway/api14.png)
11. Open Environment Variables

- Click **Manage Variables**
  ![API Gateway](/images/7.apigateway/api15.png)
- Update the **Value** of the variable **VITE_BACKEND_URL**
- Click **Save**
  ![API Gateway](/images/7.apigateway/api16.png)

12. Go to **Overview**

- Click **Redeploy this version**
  ![API Gateway](/images/7.apigateway/api17.png)
