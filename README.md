# 🎓 Cloud Based Student Performance Predictor

A cloud-deployed machine learning project to analyze and predict student exam performance based on socio-demographic and preparation-related features. This end-to-end system leverages statistical analysis, machine learning models, and robust MLOps practices using **AWS EC2 + ECR** and **Azure Container Deployment**.

---

## 📊 Problem Statement

Understand how a student's performance (test scores in Math, Reading, and Writing) is influenced by variables such as:

- Gender
- Ethnicity
- Parental level of education
- Lunch type (standard/free-reduced)
- Completion of a test preparation course

---

## 📁 Dataset

- **Source**: [Kaggle - Students Performance in Exams](https://www.kaggle.com/datasets/spscientist/students-performance-in-exams?datasetId=74977)
- **Size**: 1,000 rows × 8 columns
- **Features**:
  - Gender
  - Race/Ethnicity
  - Parental Level of Education
  - Lunch
  - Test Preparation Course
  - Scores: Math, Reading, Writing

---

## 📌 Features & Techniques Used

### ✅ Data Analysis & Preprocessing
- Exploratory Data Analysis (EDA)
- Handling categorical variables using Label Encoding & One-Hot Encoding
- Feature scaling (StandardScaler)
- Train-Test splitting

### ✅ Modeling & Evaluation
- Applied and compared the following models:
  - Decision Tree Regressor
  - AdaBoost Regressor
  - Ridge Regression
- Hyperparameter tuning using GridSearchCV
- Evaluated models based on RMSE, MAE, and R² Score
- Final model selection based on performance trade-offs

### ✅ Exception Handling
- Custom exception handling using logging
- Fail-safe data ingestion and preprocessing pipeline
- Structured code with modular functions for reusability

---

## ☁️ Deployment

### 🚀 AWS EC2 + ECR
- Dockerized the ML application
- Built and pushed Docker images to Amazon Elastic Container Registry (ECR)
- Deployed the container on an **AWS EC2 instance**
- Set up inference API using **Flask + Gunicorn**
- Ensured scalability and fault-tolerance on deployment

### ☁️ Azure Container Deployment
- Built Azure-compatible Docker image
- Pushed to Azure Container Registry
- Deployed on Azure Container Instances with autoscaling support

---

## 🛠️ Tech Stack

| Component        | Technology |
|------------------|------------|
| Programming      | Python     |
| Data Handling    | Pandas, NumPy |
| Modeling         | scikit-learn |
| Visualization    | Matplotlib, Seaborn |
| Model Tuning     | GridSearchCV |
| Logging          | Python Logging |
| Deployment       | Docker, Flask |
| Cloud            | AWS EC2, AWS ECR, Azure Container Registry |
| DevOps           | Git, GitHub, CI/CD (basic scripts) |

---

