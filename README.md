# AWS Amplify React + Vite Fullstack Application

A fullstack cloud-native web application built using **AWS Amplify React + Vite starter Template** and deployed using **AWS Amplify and GitHub CI/CD integration**.

This project demonstrates authentication, user-specific data management, and automatic cloud deployment using AWS managed services.
It was developed solely for learning purposes to gain practical experience with AWS Amplify, cloud architecture, and CI/CD workflows.

---

## 📌 Project Overview

This application was created from the **AWS Amplify React + Vite Starter Template** and extended with:

* 🔐 User Authentication (AWS Cognito)
* 🗄️ GraphQL API with AppSync
* 📦 DynamoDB Database
* 🗑️ Delete Feature
* 👥 User-based Authorization
* 🔄 Automatic CI/CD Deployment via GitHub Integration

---

## 🏗️ Architecture

| Layer           | Service               |
| --------------- | --------------------- |
| Frontend        | React + Vite          |
| Authentication  | AWS Cognito           |
| API             | AWS AppSync (GraphQL) |
| Database        | DynamoDB              |
| Hosting & CI/CD | AWS Amplify Hosting   |
| Source Control  | GitHub                |

---

## ☁️ Deployment Workflow (GitHub Integrated CI/CD)

Instead of deploying manually using Amplify CLI, this project uses:

### ✅ Amplify GitHub Repository Integration

### Workflow Used:

1. Created project using AWS Amplify React+Vite starter template
2. Connected GitHub repository to AWS Amplify Hosting
3. Amplify automatically provisioned backend services
4. Downloaded `amplify_outputs.json` from **Amplify Data Manager Tab**
5. Added `amplify_outputs.json` to local cloned repository
6. Made feature updates locally
7. Committed & pushed changes to GitHub
8. AWS Amplify automatically:

   * Detected new commit
   * Triggered build
   * Deployed updated app

### 🔄 Continuous Deployment

Every new feature pushed to GitHub automatically triggers:

* Build
* Backend sync
* Deployment
* Hosting update

No manual redeployment required.

---

## 📂 Project Structure

```
.
├── src/
├── public/
├── amplify_outputs.json
├── package.json
├── vite.config.js
└── README.md
```

---

## 🔐 Authentication & Authorization

* Secure authentication using AWS Cognito
* Separate user sessions
* Data isolation per authenticated user
* Token-based access control

---

## 🗑️ Features Implemented

* User Sign Up / Login
* Session management
* Create records
* Delete records
* User-specific data visibility
* Automatic cloud deployment

---

## 🛠️ Local Development

### Clone repository

```bash
git clone <repo-url>
cd <project-folder>
```

### Install dependencies

```bash
npm install
```

### Run locally

```bash
npm run dev
```

App runs at:

```
http://localhost:5173
```

---

## 🚀 Production Deployment

Deployment is fully managed by:

**AWS Amplify Hosting (GitHub Integrated)**

Any push to the main branch triggers:

* Build
* Deployment
* Hosting refresh

---

## 🔒 Security

For security reporting, refer to:

```
CONTRIBUTING.md#security-issue-notifications
```

AWS-managed:

* IAM Policies
* Cognito Authentication
* Secure API Gateway
* HTTPS Hosting

---

## 📈 Scalability

The app is built on fully managed AWS services:

* Serverless architecture
* Automatic scaling
* Managed database
* Managed authentication

---

## 📜 License

Licensed under the **MIT-0 License**.
See the `LICENSE` file for details.

---
