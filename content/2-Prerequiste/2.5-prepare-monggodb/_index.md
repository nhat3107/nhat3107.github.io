---
title: "Preparing MongoDB"
date: "2025-07-30"
weight: 5
chapter: false
pre: " <b> 2.5 </b> "
---

### Overview

MongoDB is a popular **NoSQL**, document-oriented database designed for high performance, scalability, and flexibility.
Instead of storing data in tables and rows (like relational databases), MongoDB stores data as **JSON-like documents** (in BSON format), which allows for nested structures and **dynamic schemas**.

MongoDB is widely used in modern applications because:

- It handles large volumes of unstructured or semi-structured data.

- It scales easily with **horizontal sharding** and **replication**.

- It integrates seamlessly with many programming languages and frameworks.

---

### Instructions

1. Access MongoDB: https://www.mongodb.com/

   - Choose login by Google
     ![MongoDB](/images/2.prerequisite/mongodb01.png)

2. In the MongoDB user interface
   - Choose **Create**
     ![MongoDB](/images/2.prerequisite/mongodb02.png)
3. Configure your cluster settings
   - Select **Free** version
     ![MongoDB](/images/2.prerequisite/mongodb03.png)
   - Choose **AWS Provider**
   - Select Region: **Hong Kong(ap-east-1)**
     ![MongoDB](/images/2.prerequisite/mongodb04.png)
4. Configure the connection

   - Create Database User
     ![MongoDB](/images/2.prerequisite/mongodb05.png)
   - Copy **Username** and **Password**
   - Click **Choose a connection method**
     ![MongoDB](/images/2.prerequisite/mongodb06.png)
   - Choose **Drivers**
     ![MongoDB](/images/2.prerequisite/mongodb07.png)
   - Copy _connection string_ and use it later
     ![MongoDB](/images/2.prerequisite/mongodb08.png)

   - The String should be in this structure

   ```
   mongodb+srv://<your_username>:<your_password>@cluster0.vbxyrhh.mongodb.net/<your_appname>?retryWrites=true&w=majority&appName=Cluster0
   ```

   Replacing:

   - <your_usename> : your Database username
   - <your_password>: your Database password
   - <your_appname>: your Database name
