---
title: "Amplify"
date: "2025-07-30"
weight: 6
chapter: false
pre: " <b> 6. </b> "
---

1. Access the **AWS Management Console**

- Search for **AWS Amplify**
- Select **AWS Amplify** from the search results
  ![Amplify](/images/6.amplify/amplify01.png)
  ![Amplify](/images/6.amplify/amplify02.png)

2. Click **Deploy An App**

- Start building with Amplify:

  - Select **GitHub**
  - Click **Next**
    ![Amplify](/images/6.amplify/amplify03.png)

- Add repository and branch:

  - Select the **CloudTalkr** repo
  - Check **My app is a monorepo**
  - **Monorepo root directory**: `frontend`
  - Click **Next**
    ![Amplify](/images/6.amplify/amplify04.png)

- App settings:

  - **Key**: `VITE_BACKEND_URL`
  - **Value**: _< Public IPv4 Address :3000>_
  - Click **Next**
    ![Amplify](/images/6.amplify/amplify05.png)
    ![Amplify](/images/6.amplify/amplify06.png)

- Review:
- Click **Save and Deploy**

  ![Amplify](/images/6.amplify/amplify07.png)
  ![Amplify](/images/6.amplify/amplify08.png)

  ![Amplify](/images/6.amplify/amplify09.png)

{{% notice warning%}}
Open EC2 and insert: FRONTEND_URL= <Amplify_Url> to .env
{{% /notice %}}
