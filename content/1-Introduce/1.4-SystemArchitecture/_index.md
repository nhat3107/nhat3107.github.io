---
title: "System Architecture"
date: "2024-03-20"
weight: 4
chapter: false
pre: " <b> 1.4 </b> "
---

The system follows a Client – Server – Cloud architecture, combining real-time technologies (via GetStream), RESTful APIs, and cloud-native infrastructure to ensure scalability, performance, and maintainability. Both backend and frontend are deployed on AWS platform.

### System Components

#### Frontend – Client Side (React.js)

- Interactive user interface (UI/UX)

- Communicates with the backend via REST APIs and GetStream SDK

- Deployed via AWS Amplify CI/CD

- Main functionalities include:

  - User authentication (sign-up/login)

  - Real-time messaging (one-on-one)

  - Video streaming or calling (via GetStream Video)

  - Group/channel management

#### Backend – Server Side (Node.js + Express.js)

- Handles core logic: authentication, user and group management, chat integration, data sync

- Uses **Prisma ORM** to interact with **MongoDB**

- Deployed on **Amazon EC2**

#### Database – MongoDB Atlas

- Cloud-hosted NoSQL database
- Stores user profiles, chat history, group metadata, video session details
- Scalable and optimized for real-time applications

#### Media Storage – Cloudinary

- Stores and delivers media content (images, videos) via CDN
- Integrated with chat for sending avatars, image sharing, video previews, etc.

---

### System Diagrams

#### Overall Architecture Diagram (AWS Architecture)

![General Architecture](/images/1.introduction/generalArchitecture.png)

### WorkFlow

![Sequence Diagram](/images/1.introduction/workflow.png)

---
