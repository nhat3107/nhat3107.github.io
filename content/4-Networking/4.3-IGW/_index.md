---
title: "Internet Gateway"
date: "2025-07-30"
weight: 3
chapter: false
pre: " <b> 4.3 </b> "
---

## Overview

- An Internet Gateway (IGW) is a VPC component that enables internet connectivity
- Acts as a bridge between your VPC and the internet
- Supports bidirectional communication for resources inside the VPC

---

## Instructions

1. Go to the **VPC** service

   - Select **Internet Gateways** from the left-hand menu
   - Click on **Create internet gateway**
     ![IGW](/images/4.networking/IGW01.png)

2. Configure the Internet Gateway

   - In the **Name tag** field, enter `CloudTalkr-IGW`
   - Click **Create internet gateway**
     ![IGW](/images/4.networking/IGW02.png)

3. Confirm the Internet Gateway was created successfully
   ![IGW](/images/4.networking/IGW03.png)

#### Attach to VPC

4. Attach the Internet Gateway to your VPC

   - Click **Actions**
   - Choose **Attach to VPC**
   - Select the **CloudTalkr-VPC** VPC from the dropdown (VPC ID will auto-fill)
   - Click **Attach internet gateway**
     ![IGW](/images/4.networking/IGW04.png)

#### Confirm Status

5. Once attached:

   - The **State** of the Internet Gateway will change to **Attached**
   - The IGW is now ready to route internet traffic for your VPC
     ![IGW](/images/4.networking/IGW05.png)
