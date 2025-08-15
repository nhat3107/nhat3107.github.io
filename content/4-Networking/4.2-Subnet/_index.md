---
title: "Subnet"
date: "2025-07-30"
weight: 2
chapter: false
pre: " <b> 4.2 </b> "
---

## Overview

- A subnet is a smaller network segment within a VPC
- Allows distribution of resources across Availability Zones (AZ)

---

## Instructions

1. Go to the **VPC** service

   - Select **Subnets** from the left-hand menu
   - Click **Create subnet**
     ![Subnet](/images/4.networking/subnet01.png)

2. Select a VPC

   - In the **Create subnet** screen
   - Choose the **CloudTalkr-VPC** VPC created earlier

3. Configure the first subnet

   - **Subnet name**: Enter `Public Subnet 1`
   - **Availability Zone**: Choose **_ap-southeast-1a_**
   - **IPv4 CIDR block**: Enter `10.0.0.0/24`
   - Click **Create subnet**
     ![Subnet](/images/4.networking/subnet02.png)

4. Confirm the subnet was created successfully
   ![Subnet](/images/4.networking/subnet03.png)

{{%notice info%}}
**Availability Zone (AZ)**: Human-readable name (e.g., ap-southeast-1a)
{{%/notice%}}

{{%notice info%}}
**AZ ID**: The actual identifier for the AZ  
 AWS maps AZ names to AZ IDs differently for each account to distribute resource allocation more evenly.
{{%/notice%}}
