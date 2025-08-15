---
title: "Deploying Backend"
date: "2025-07-30"
weight: 2
chapter: false
pre: " <b> 5.2 </b> "
---

### Environment Preparation

- Install NVM (Node Version Manager).

```
    curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.7/install.sh |
```

![Backend](/images/5.ec2/backend01.png)

- Reload the shell to use nvm:

```
    . ~/.nvm/nvm.sh
```

- Install the latest Node.js version:

```
    nvm install node
```

- Check installed versions of Node and npm:

```
   node -v
```

```
   npm -v
```

![Backend](/images/5.ec2/backend02.png)

### Install Git and Clone Project

- Update system and install Git:

```
   sudo yum update -y
```

```
   sudo yum install git -y
```

Check Git version:

```
    git --version
```

![Backend](/images/5.ec2/backend03.png)

- Clone the project source code from GitHub:

```
    git clone https://github.com/nhat3107/CloudTalkr.git
```

- Navigate to the backend folder:

```bash
   ls
```

```
   cd CloudTalkr/backend
```

![Backend](/images/5.ec2/backend04.png)

---

### Install and Run the Server

- Install npm packages for the backend:

```
    npm i
```

- Create .env file - Paste **the API keys**, **Database Url**,...
  ![Backend](/images/5.ec2/backend05.png)
  ![Backend](/images/5.ec2/backend06.png)
- Start server using the new .env configuration:

```
    npm run start
```

![Backend](/images/5.ec2/backend08.png)

- Install and Configure PM2 for Background Process

- Install PM2 to manage Node.js processes:

```
    npm i pm2 -g
```

- Enable PM2 to auto-start on system boot:

```
    pm2 startup
```

- Paste the code appeare and run.

- Start the server with PM2, check status, and monitor:

```
   pm2 start ecosystem.config.cjs
```

![Backend](/images/5.ec2/backend07.png)

```
   pm2 status
```

![Backend](/images/5.ec2/backend09.png)

```
    pm2 monit
```

![Backend](/images/5.ec2/backend10.png)

- Stop and delete all current PM2 processes:

```
   pm2 stop all
```

```
   pm2 delete all
```

![Backend](/images/5.ec2/backend11.png)

- Restart the server from the config:

```
    pm2 start ecosystem.config.cjs
```

![Backend](/images/5.ec2/backend12.png)

- API Test
  ![Backend](/images/5.ec2/backend13.png)
