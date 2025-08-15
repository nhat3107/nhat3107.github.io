---
title: "Route Table"
date: "2025-07-30"
weight: 4
chapter: false
pre: " <b> 4.4 </b> "
---

## Overview

- A Route Table defines how network traffic is directed within a VPC
- It determines the paths that packets take between subnets and the internet
- Enables control over inbound/outbound traffic in your VPC

---

## Instructions

1. Access the **VPC** service

   - Select **Route Tables** from the left-hand menu
   - Select Route Table of CloudTalkr-VPC
     ![RTB](/images/4.networking/rtb01.png)

2. Add route for Internet Gateway

   - Click **Actions**
   - Select **Edit routes**
     ![RTB](/images/4.networking/rtb02.png)

3. Add new route

   - Click **Add route**
   - **Destination**: Enter `0.0.0.0/0` (represents internet)
   - **Target**: Select **Internet Gateway** and choose the previously created IGW
   - Click **Save changes**
     ![RTB](/images/4.networking/rtb03.png)
