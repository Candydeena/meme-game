# 🎮 Flip Game – AWS CI/CD Deployment Project

## 📌 Project Overview

This project demonstrates how to build and deploy a **Flip Card Game** using a **Continuous Deployment (CI/CD) pipeline** on **AWS**. The game source code is hosted on **GitHub**, and every code change is automatically deployed to an **AWS S3 bucket** using **AWS CodePipeline**, with global content delivery powered by **Amazon CloudFront**.

The goal of this project is to showcase **DevOps skills**, **cloud deployment**, and **automation** using AWS services for a real-world gaming application.

---

## 🕹️ Game Description

The **Flip Game** is a browser-based memory card game where players flip cards to find matching pairs. The game is lightweight, responsive, and optimized for fast loading using AWS infrastructure.

**Game Features:**

* Interactive card flip animations
* Score and match tracking
* Responsive UI for desktop and mobile
* Static web-based game built using **HTML, CSS, and JavaScript**

---

## 🏗️ Architecture Overview

**CI/CD Flow:**

1. Developer pushes code to the GitHub repository
2. AWS CodePipeline detects changes automatically
3. Build/Deploy stage triggers deployment
4. Files are uploaded to an S3 bucket (static hosting)
5. Amazon CloudFront distributes content globally

```
GitHub → AWS CodePipeline → Amazon S3 → Amazon CloudFront → Users
```

---

## 🧩 Frontend Technologies Used

* **HTML5** – Structure of the game UI
* **CSS3** – Styling, layout, and flip animations
* **JavaScript** – Game logic, card flipping, scoring, and interactivity

---

## ☁️ AWS Services Used

### 🔹 Amazon S3

* Hosts the Flip Game as a **static website**
* Stores HTML, CSS, JavaScript, and assets

### 🔹 AWS CodePipeline

* Automates deployment from GitHub to S3
* Ensures continuous delivery on every commit

### 🔹 Amazon CloudFront

* Provides low-latency global content delivery
* Improves performance and security

### 🔹 GitHub

* Source code management
* Triggers CI/CD pipeline on code changes

---

## 🔁 CI/CD Pipeline Stages

1. **Source Stage**

   * Connected to GitHub repository
   * Detects commits automatically

2. **Deploy Stage**

   * Deploys updated files to S3 bucket
   * Makes the latest version live instantly

---

## 🚀 Deployment Steps (High-Level)

1. Create an S3 bucket and enable static website hosting
2. Upload initial game files (HTML, CSS, JS)
3. Create an AWS CodePipeline

   * Source: GitHub
   * Deploy: Amazon S3
4. Configure CloudFront distribution with S3 as origin
5. Access the game using CloudFront URL

---

## 🌐 Live Access

Once deployed, the game can be accessed via:

* **CloudFront Distribution URL** (recommended)
* **S3 Static Website Endpoint**

---

## 🔐 Security & Best Practices

* S3 bucket access restricted to CloudFront
* IAM roles used for secure pipeline execution
* No hard-coded credentials

---

## 📈 Learning Outcomes

* Hands-on experience with AWS CI/CD services
* Understanding of static web hosting on AWS
* Automating deployments using GitHub and CodePipeline
* Using CloudFront for performance optimization

---

## 🧑‍💻 Author

**Deenadayalan R**
Cloud & DevOps Enthusiast | Python Developer | AWS Learner

---

## 📄 License

This project is for educational and portfolio purposes.

---

⭐ *If you like this project, feel free to star the repository!*
