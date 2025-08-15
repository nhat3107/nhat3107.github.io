---
title: "VPC"
date: "2025-07-30"
weight: 1
chapter: false
pre: " <b> 4.1 </b> "
---

## Objective

- Create a separate virtual network environment in AWS
- Define the IP address range for the VPC
- Configure basic DNS features

---

## Instructions

1. Access the **AWS Management Console**

   - Search for the **VPC** service
   - Select **VPC** from the search results
     ![VPC](/images/4.networking/vpc01.png)

2. In the **VPC Dashboard**

   - Select **Your VPCs** from the left menu
   - Click **Create VPC**
     ![VPC](/images/4.networking/vpc02.png)

3. Configure VPC parameters

   - **Resources**: Select **VPC only**
   - **Name tag**: Enter `CloudTalkr-VPC`
   - **IPv4 CIDR**: Enter `10.0.0.0/16`

{{% notice note %}}
Keep the **Tenancy** option as **Default**. Switching to **Dedicated** may restrict the types of EC2 Instances supported in this VPC.
{{% /notice %}}

4. Confirm VPC creation

   - Click **Create VPC** to complete the process
     ![VPC](/images/4.networking/vpc03.png)

5. Verify VPC status after creation
   ![VPC](/images/4.networking/vpc04.png)
6. Enable DNS features for the VPC

   - Click **Edit VPC settings**
   - Go to the **DNS settings** tab
   - Enable **DNS hostnames** and **DNS resolution**
   - Save changes
     ![VPC](/images/4.networking/vpc05.png)
