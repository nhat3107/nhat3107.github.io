+++
title = "Clean up resources"
date = 2022
weight = 9
chapter = false
pre = "<b>9. </b>"
+++

We will take the following steps to delete the resources we created in this exercise.

---

### Delete Amplify

1. Access AWS Amplify Console

   - Open [AWS Amplify Console](https://console.aws.amazon.com/amplify/home#)
   - From the application list, choose the app you want to delete

2. Open app settings

   - In the app details page, select the App settings tab
   - Click General to view general settings

3. Delete the app

   - Scroll down and click Delete app
   - Enter the app name to confirm
   - Click Delete to complete
     ![Clean Amplify](/images/9.clean/cleanamplify.png)

---

### Delete EC2 instance

1. Go to [EC2 service management console](https://console.aws.amazon.com/ec2/v2/home)

   - Click **Instances**.
   - Select the instance
   - Click **Instance state**.
   - Click **Terminate instance**, then click **Terminate** to confirm.
     ![Clean EC2](/images/9.clean/cleanec2.png)
   - Then move to Security Group and Delete EC2's Security Group
     ![Clean SG](/images/9.clean/cleansecuritygroup.png)

---

### Delete API GateWay

1. Access Amazon API Gateway

   - Open [API Gateway Console](https://console.aws.amazon.com/apigateway)
   - Select APIs from the left-hand navigation

2. Select the API to delete

   - Find the API you want to delete (HTTP, REST, or WebSocket)

   - Click the API name to open details

3. Delete

   - Click Actions > Delete
   - Confirm by entering the API name (if required)
   - Click Delete to finish
     ![Clean API](/images/9.clean/cleanapi.png)

---

### Delete VPC

1. Go to [VPC service management console](https://console.aws.amazon.com/vpc/home)

   - Click **Your VPCs**.
   - Click on **Lab VPC**.
   - Click **Actions**.
   - Click **Delete VPC**.

2. In the confirm box, enter **delete** to confirm, click **Delete** to delete **Lab VPC** and related resources(Subnets, Internet Gateway...)
   ![Clean VPC](/images/9.clean/cleanvpc.png)

---
