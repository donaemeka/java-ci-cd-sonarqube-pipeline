# 🚀 Java CI/CD Pipeline with SonarQube & AWS Deployment

This project demonstrates a **production-style CI/CD pipeline for a Java Spring Boot application**, integrating **SonarQube for code quality analysis** and **automated deployment to AWS EC2** using GitHub Actions.

It simulates a real-world DevOps workflow where every code change is automatically built, tested, analyzed, and deployed.

---

## 📌 Project Overview

The goal of this project is to implement a **complete DevOps lifecycle**:

- Continuous Integration (build & test)
- Code Quality Analysis (SonarQube)
- Continuous Deployment (AWS EC2)

This ensures **fast, reliable, and high-quality software delivery**.

---

## 🎯 Problem It Solves

Modern development teams face:

- Manual and error-prone deployments  
- Poor code quality reaching production  
- Lack of automation in testing and deployment  

This project solves these by implementing:

- Automated CI/CD pipeline  
- Code quality enforcement with SonarQube  
- Continuous deployment to cloud infrastructure  

---

## 🏗️ Architecture

    Developer → GitHub → GitHub Actions → SonarQube → AWS EC2 → Users

---

## ⚡ CI/CD Pipeline Flow

    Code Push
        ↓
    GitHub Actions
        ↓
    Build & Test (Maven)
        ↓
    SonarQube Analysis
        ↓
    Package JAR
        ↓
    Upload Artifact
        ↓
    Deploy to EC2 (SSH)
        ↓
    Application Running

---

## 🔧 Technology Stack

| Category | Tools |
|----------|------|
| Language | Java 17 |
| Framework | Spring Boot |
| Build Tool | Maven |
| CI/CD | GitHub Actions |
| Code Quality | SonarQube |
| Cloud | AWS EC2 |
| Deployment | SSH |
| Monitoring | Application logs |

---

## 🚀 Key Achievements

- Automated CI/CD pipeline, reducing manual deployment steps by ~80%  
- Integrated SonarQube quality gates to prevent bad code from reaching production  
- Successfully deployed a Java application to AWS EC2 with automated updates  
- Implemented secure secret management using GitHub Actions  

---

## 📸 Pipeline Success Metrics

### ✅ SonarQube Analysis Results
![SonarQube Dashboard](images/sonarqube-dashboard.png)

### ✅ GitHub Actions Pipeline  
![GitHub Actions](images/github-actions.png)

### ✅ Application Deployment
![Spring PetClinic](images/running-app.png)

---

## 🚀 How to Run This Project

### 1️⃣ Clone the Repository

    git clone https://github.com/donaemeka/java-ci-cd-sonarqube-pipeline.git
    cd java-ci-cd-sonarqube-pipeline/spring-petclinic

---

### 2️⃣ Configure GitHub Secrets

Add the following secrets in your GitHub repository:

- SONAR_TOKEN → SonarQube authentication token  
- SONAR_HOST_URL → SonarQube server URL  
- EC2_SSH_KEY → Private SSH key  
- EC2_HOST → EC2 public IP  

---

### 3️⃣ Trigger Pipeline

    git push origin main

GitHub Actions will automatically:

- Build the application  
- Run tests  
- Perform SonarQube analysis  
- Deploy to AWS EC2  

---

### 4️⃣ Access Application

    http://<EC2-IP>:8080

---

## 🧠 Key Learnings

- Designing CI/CD pipelines for Java applications  
- Integrating SonarQube for automated code quality checks  
- Automating deployments using GitHub Actions  
- Managing secrets securely in CI/CD pipelines  
- Deploying Spring Boot applications to cloud infrastructure  

---

## ⚠️ Challenges & Solutions

### Pipeline Failures
- Problem: Missing environment variables caused pipeline failure  
- Solution: Configured GitHub Secrets correctly  

### Deployment Issues
- Problem: SSH connection to EC2 failed  
- Solution: Fixed SSH key permissions and security group rules  

### SonarQube Integration
- Problem: Analysis not triggering  
- Solution: Corrected SonarQube token and server URL  

---

## 🎯 DevOps Skills Demonstrated

- CI/CD Pipeline Design  
- Code Quality Automation (SonarQube)  
- Cloud Deployment (AWS EC2)  
- Secure Secret Management  
- Java Application Deployment  
- Automation & Workflow Optimization  

---

## 📈 Business Value

- Faster release cycles  
- Improved code quality  
- Reduced manual errors  
- Reliable deployments  
- Scalable DevOps pipeline  

---

## 👨‍💻 About Me

Donatus Emeka Anyalebechi  
Junior DevOps Engineer  

Germany  
donaemeka92@gmail.com  
https://www.linkedin.com/in/donatus-devops  
https://github.com/donaemeka  

Open to Junior DevOps & Cloud Engineering opportunities  

---

⭐ Built to demonstrate real-world DevOps CI/CD and automation practices