# 🚀 AWS CI/CD Deployment with Elastic Beanstalk & CodePipeline

This project demonstrates how to deploy a web application to **AWS Elastic Beanstalk** using **AWS CodePipeline**, with **GitHub** as the source repository.  

It follows a **staging → approval → production** workflow to ensure safe deployments.

---

## 🏗️ Architecture Workflow
1. **Source Stage**  
   - CodePipeline fetches the latest code directly from **GitHub**.  

2. **Staging Deployment**  
   - Application is deployed to the **Staging Elastic Beanstalk Environment**.  
   - Used for initial verification and testing.  

3. **Approval Stage**  
   - A **manual approval step** is triggered.  
   - An email notification is sent to approvers.  
   - The pipeline halts until approval is granted.  

4. **Production Deployment**  
   - Once approved, the application is deployed to the **Production Elastic Beanstalk Environment**.  

---

## 🔑 Key Features
- Continuous Integration & Deployment (CI/CD) via **AWS CodePipeline**  
- Source code stored in **GitHub**  
- Deployment artifacts stored in **Amazon S3**  
- Two environments in **Elastic Beanstalk**:
  - `staging` → automatic deployments
  - `production` → requires **manual approval**  
- Email-based approval for secure production releases  

---

## 📦 How It Works
1. Developer pushes code changes to **GitHub**.  
2. **CodePipeline** automatically:
   - Pulls the latest changes  
   - Deploys them to the **staging environment**  
3. An **email approval request** is sent.  
4. Once approved, deployment continues to the **production environment**.  

---

## 🛠️ Prerequisites
- AWS Account  
- GitHub repository connected to **CodePipeline**  
- S3 bucket configured for pipeline artifacts  
- Two Elastic Beanstalk environments:
  - `staging`
  - `production`  
- SNS (Simple Notification Service) configured for **email approvals**  

---

## 📂screenshots:

<img width="1920" height="1080" alt="Screenshot (9)" src="https://github.com/user-attachments/assets/b3ad697e-65f0-4a6f-8f79-06d2f26ded9e" />
<img width="1920" height="1080" alt="Screenshot (10)" src="https://github.com/user-attachments/assets/feaf0636-4205-4ff0-9d34-a370f1f6adaa" />
<img width="1920" height="1080" alt="Screenshot (11)" src="https://github.com/user-attachments/assets/59761b16-feae-431e-8085-3d34f63f09f5" />
<img width="1920" height="1080" alt="Screenshot (13)" src="https://github.com/user-attachments/assets/df24c589-f467-4521-83f0-7aadb3e8a369" />
<img width="1920" height="1080" alt="project2-1" src="https://github.com/user-attachments/assets/b12a2d6a-aecd-487d-8233-8261e58a8051" />
<img width="1920" height="1080" alt="project2-2" src="https://github.com/user-attachments/assets/c1685340-0f9b-4658-ba96-d14990f1e71b" />
<img width="1920" height="1080" alt="Screenshot (14)" src="https://github.com/user-attachments/assets/dc767924-8b48-4eab-9f96-089ff91a7b49" />
<img width="1920" height="1080" alt="Screenshot (17)" src="https://github.com/user-attachments/assets/ec42a726-f605-4299-abd9-0cf2e126d042" />
<img width="1920" height="1080" alt="Screenshot (18)" src="https://github.com/user-attachments/assets/8701e0f6-a174-4bba-8c04-9485b82dbec1" />
<img width="1920" height="1080" alt="Screenshot (19)" src="https://github.com/user-attachments/assets/885c3912-7576-424e-af2d-1ba3b56b95aa" />
<img width="1920" height="1080" alt="project2-3" src="https://github.com/user-attachments/assets/51912e13-c85b-4b2e-aa50-12ecfe51e413" />



