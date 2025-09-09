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
<img width="1920" height="1080" alt="Screenshot (9)" src="https://github.com/user-attachments/assets/c4098715-b857-47ff-9851-7342e3593512" />
<img width="1920" height="1080" alt="Screenshot (10)" src="https://github.com/user-attachments/assets/9566ffcd-f309-4718-8b76-e0e3b53c8423" />
<img width="1920" height="1080" alt="Screenshot (11)" src="https://github.com/user-attachments/assets/a429995b-ed10-48d9-ba61-274cbce0e9cb" />
<img width="1920" height="1080" alt="Screenshot (13)" src="https://github.com/user-attachments/assets/112720c2-0ae7-4a11-a738-6305a218516b" />
<img width="1920" height="1080" alt="project2-1" src="https://github.com/user-attachments/assets/aec5eede-07ea-4f39-8cb7-a0d9d29be96a" />
<img width="1920" height="1080" alt="project2-2" src="https://github.com/user-attachments/assets/9288620c-6edc-4c82-8d89-a0c1523ecf3d" />
<img width="1920" height="1080" alt="Screenshot (14)" src="https://github.com/user-attachments/assets/cc7391dc-8eeb-4851-b40e-671935f69a90" />
<img width="1920" height="1080" alt="Screenshot (17)" src="https://github.com/user-attachments/assets/19001734-4e0b-44ad-a9a5-4a8ba15fec47" />
<img width="1920" height="1080" alt="Screenshot (18)" src="https://github.com/user-attachments/assets/786e95d5-8368-42b4-8ca0-98d082346549" />
<img width="1920" height="1080" alt="Screenshot (19)" src="https://github.com/user-attachments/assets/04b31e28-be15-481a-8997-eb50d13b49ce" />
<img width="1920" height="1080" alt="project2-3" src="https://github.com/user-attachments/assets/23854c36-2930-4129-9a98-9856ea599367" />



