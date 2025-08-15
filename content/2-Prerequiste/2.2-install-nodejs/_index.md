---
title: "Installing Nodejs"
date: "2024-07-30"
weight: 2
chapter: false
pre: " <b> 2.2 </b> "
---

## Overview

**NodeJs** is a server-side JavaScript runtime environment used to build the backend of this project. The backend leverages Node.js along with Express to handle APIs and connect to the database.

In addition to Node.js, the system also requires **npm** (Node Package Manager) — a tool for managing and installing dependencies for both frontend and backend.

Both the frontend (ReactJs) and backend (ExpressJs) require NodeJs to run and develop locally.

---

## Instructions

1. Go to the official Node.js download page: https://nodejs.org/en

2. Select the **LTS (Long Term Support)** version suitable for your operating system:

   - Windows: `.msi` installer
   - macOS: `.pkg` installer
   - Linux: choose the version that matches your distro

3. Download and install it like any other software (Next → Next → Install...).

4. Verify the installation by opening Terminal or Command Prompt and running:

   ```bash
   node -v
   npm -v
   ```

   ![Node Version](/images/2.prerequisite/nodeversion.png)
