---
title: "Development and Deployment"
date: "2025-07-30"
weight: 1
chapter: false
---

# Building a Real-Time Chat & Video Streaming Application with MERN Stack and Deploying on AWS

### Project Objectives

This project aims to develop a real-time chat and video streaming application using the MERN Stack, while implementing on AWS infrastructure. The application combines a modern user interface with real-time communication capabilities and secure deployment on the cloud.

### Technologies Used

#### 🧑‍💻 Development Stack – MERN

- **Frontend**:

  - React.js
  - Tailwind CSS, DaisyUI
  - GetStream.io (real-time chat and video handling)

- **Backend**:
  - Node.js + Express.js
  - Prisma ORM
  - MongoDB Atlas (cloud database)
  - Cloudinary (media storage and delivery)

#### ☁️ Deployment Stack – AWS Services

- **CI/CD for Frontend**:

  - **AWS Amplify** – Automatically builds, deploys, and hosts the React frontend from GitHub.

- **Backend**:
  - **EC2** – Automatically builds and deploys the Express.js backend to Amazon EC2.

#### 📂 Source Code Management

- **GitHub** – Manages source code and triggers CI/CD workflows.

### Expected Outcomes

- A fully functional real-time chat and video streaming application.
- A modern, smooth, and responsive user interface across all devices.
- A scalable, cloud-native architecture that is easy to maintain and upgrade in the future.

### Contents

1. [Introduction](1-introduce/)
2. [Prerequisites](2-prerequiste/)
3. [Create Budget](3-budget)
4. [Networking](4-networking/)
5. [Amplify](5-amplify/)
6. [CodePipeline](6-codepipeline/)
7. [Achievements](7-achievements/)
8. [Resource Cleanup](8-cleanup/)
