---
title: "Launching EC2"
date: "2025-07-30"
weight: 1
chapter: false
pre: " <b> 5.1 </b> "
---

## Instance Configuration

1. Go to the **EC2 Dashboard**

   - Search for the **EC2** service

   - Select **EC2** from the search results
     ![EC2](/images/5.ec2/ec201.png)

2. Launch a new Instance

   - Select **Instances** from the left-hand menu

   - Click **Launch instances**
     ![EC2](/images/5.ec2/ec202.png)

3. Set the Instance Name

   - Under **Name and tags**, enter `cloudtalkr-server`
     ![EC2](/images/5.ec2/ec203.png)

4. Choose Amazon Machine Image (AMI)

   - Select **Quick Start**

   - Choose **Amazon Linux 2023 kernel-6.1**

   - Pick a suitable AMI version
     ![EC2](/images/5.ec2/ec204.png)

5. Configure Instance Type and Key Pair

   - Choose an appropriate **Instance type**

   - Click **Create new key pair**
     ![EC2](/images/5.ec2/ec205.png)

6. Create a new Key Pair

   - **Key pair name**: `cloudtalkr-keypair`

   - **Key pair type**: Select **RSA**

   - **Private key format**: Select **.pem**
     ![EC2](/images/5.ec2/ec206.png)

#### Network Settings

7. Configure Network

   - **VPC**: Select the **CloudTalkr-VPC** VPC

   - **Subnet**: Select **_Public Subnet 1_**

   - **Auto-assign public IP**: Select **_Enable_**

   - **Security Group**: Choose **Create Security Group**

   - **Security Group Name**: `CloudTalkr-sg`

   - **Description**: `CloudTalkr Secutity Group`

     ![EC2](/images/5.ec2/ec207.png)
     ![EC2](/images/5.ec2/ec208.png)

   - Remember to set up these **Inbound Rules**

   {{% notice warning %}}
   Remember to open Custom TCP for PORT 3000 FROM 0.0.0.0: just use for lab/test, dangerous for production environment
   {{% /notice %}}

   - Click **Launch instance**

8. Confirm the instance was launched successfully
   ![EC2](/images/5.ec2/ec209.png)

#### Connect

Access the **EC2** service:

{{% notice note %}}
Many kind of connection tools could be used, but this lab uses MobaXterm.
{{% /notice %}}

[MobaXterm Guideline Here](https://000004.awsstudygroup.com/vi/4-launchlinuxinstance/4.2-connectlinuxinstance/)

- Click **Instances**

- Select _**cloudtalkr-server**_
  ![EC2](/images/5.ec2/ec210.png)
- Copy **Public IP** and connect to this instance
  ![EC2](/images/5.ec2/ec211.png)
  ![EC2](/images/5.ec2/ec212.png)
