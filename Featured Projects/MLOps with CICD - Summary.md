# 🏥 MLOps for Clinical Decision Support

This project focuses on designing a secure, scalable MLOps pipeline to support AI-assisted clinical decision-making for heart disease and stroke risk assessment. The system was built to reflect real-world healthcare constraints, including data privacy, regulatory compliance, model governance, and continuous monitoring.

The goal was to demonstrate how machine learning models can be safely deployed, monitored, and improved over time in a regulated medical environment.

---

## ☁️ Cloud Architecture (AWS)

The full system was deployed in a secure AWS environment to align with healthcare-style privacy and security requirements:

- Virtual Private Cloud (VPC) with restricted access  
- Encrypted S3 storage for clinical data  
- SageMaker for training and evaluation  
- Feature Store for consistent data pipelines  
- IAM for role-based access control  
- CloudWatch for monitoring and alerts  

<img width="1441" height="810" alt="Systems AWS Architecture" src="https://github.com/user-attachments/assets/12389295-e43f-4ff1-81ff-ebc78927ede1" />



This setup ensured sensitive data was isolated from public networks and handled using industry-standard security practices.

---

## 🔁 MLOps Pipeline

The pipeline supports the full machine learning lifecycle:

- Secure data ingestion and preprocessing  
- Feature engineering and storage  
- Model training and evaluation  
- Model registry and versioning  
- Automated CI/CD retraining  
- Shadow deployments for safe testing  
- Human-in-the-loop approvals  
- Production batch inference  
- Ongoing performance and bias monitoring  

The system emphasizes reliability, traceability, and safety over raw model speed.

---

## 📊 Data

Two clinical datasets were used for proof-of-concept:

- Heart disease risk data (UCI)  
- Stroke risk prediction data (Kaggle)  

Both datasets were processed using consistent feature pipelines and stored in the AWS Feature Store to ensure reproducibility.

---

## 🧠 Models

- **XGBoost** (primary model)  
- Logistic Regression (baseline)  

Models were evaluated using clinically relevant metrics such as AUC-ROC, precision, recall, and F1 score, with additional monitoring for demographic bias.

---

## 🔍 Monitoring & Governance

The system continuously monitors:

- Model performance drift  
- Feature distribution changes  
- Bias across protected attributes  
- Data quality issues  
- Infrastructure health  

Alerts are triggered when performance deviates from expected baselines, enabling proactive retraining or investigation.

---

## 🏆 Results

The pipeline successfully demonstrated:

- Automated model retraining  
- Safe shadow deployments  
- Secure batch inference  
- Continuous performance monitoring  
- Bias-aware evaluation  
- Human approval before production release  

This mirrors how ML systems are deployed in regulated industries such as healthcare and finance.

---

## 👨‍💼 My Role

- Designed AWS-based MLOps architecture  
- Built CI/CD training pipelines  
- Implemented monitoring and governance workflows  
- Evaluated clinical ML models  
- Framed system for regulatory compliance  
- Led documentation and presentation  

---

## 🛠️ Tech Stack

Python • XGBoost • Scikit-learn  
AWS (S3, SageMaker, Feature Store, CloudWatch, IAM, VPC)  
Pandas • NumPy  

