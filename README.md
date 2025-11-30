📘 Credit Risk Modelling Project

An end-to-end credit risk analytics project using Python, IFRS-9 ECL, and real-world banking workflows.

---

📌 1. Project Overview

This project demonstrates the complete lifecycle of a Credit Risk Modelling project used in banks and NBFCs. It includes:

- Data Collection (Kaggle Dataset)
- Data Cleaning & Preprocessing
- Exploratory Data Analysis (EDA)
- Feature Engineering
- PD (Probability of Default) Model
- Model Evaluation (AUC, KS, Confusion Matrix)
- IFRS-9 Expected Credit Loss (ECL) Calculation
- Documentation (User Stories, BRD, FSD)
- Jira-based Agile Workflow

The goal is to build a transparent, auditable, and end-to-end risk analytics framework.

---

⚙️ 2. Tech Stack

- Python (pandas, numpy, scikit-learn, matplotlib)
- Jupyter Notebook
- SQL (for portfolio-style queries)
- IFRS-9 Framework (PD × LGD × EAD)
- Jira (Scrum workflow)
- GitHub (Version control & documentation)

---

📂 3. Project Structure

Credit-Risk-Models/
│
├── data/
│ ├── raw/ # Original dataset (from Kaggle)
│ └── processed/ # Cleaned/transformed data for modelling
│
├── notebooks/
│ ├── 01_data_cleaning.ipynb
│ ├── 02_eda.ipynb
│ ├── 03_pd_model.ipynb
│ └── 04_ecl_calculation.ipynb
│
├── docs/
│ ├── User_Stories.md
│ ├── BRD.md
│ └── FSD.md
│
├── jira_screenshots/
│ ├── jira_board_progress_1.png
│ ├── Jira_Board_Progress_2.png
│
├── ifrs9_ecl/
├── pd_model/
├── lgd_ead_models/
└── README.md

---

📜 4. Documentation

🔹 **User Stories**  
Defines functional expectations and user needs.  
👉 `/docs/User_Stories.md`

🔹 **Business Requirements Document (BRD)**  
Explains business goals, scope, and credit risk objectives.  
👉 `/docs/BRD.md`

🔹 **Functional Specification Document (FSD)**  
Technical workflow and model specifications.  
👉 `/docs/FSD.md`

---

🚀 5. Agile Workflow (Enhanced Jira Section)

This project follows a structured **Scrum/Kanban hybrid Agile workflow**, tracked in Jira.

## 🧭 Project Management Approach

I managed this project using **Jira Scrum Board**, including:

- Epics for each major workstream  
- User stories aligned with credit risk modelling  
- Technical tasks under each story  
- Tracking progress through Backlog → In Progress → In Review → Done  
- Daily updates and weekly sprint planning  

---

## 🧩 Jira Structure

### **Epics**
- Data Understanding & Requirement Gathering  
- Data Cleaning & Transformation  
- EDA & Feature Engineering  
- PD Model Development  
- LGD Model Development (future)  
- EAD Model Development (future)  
- Documentation & Reporting  

---

## 📝 Sample User Stories

### **US-01: Dataset Understanding**  
*As a Credit Risk Analyst, I want to understand the dataset so that I can plan the modeling steps.*

**Tasks:**  
- Import raw datasets  
- Data dictionary creation  
- Missing value and outlier identification  

---

### **US-02: Data Cleaning**  
*As a Model Developer, I want to clean and preprocess the dataset so that it becomes modeling-ready.*

**Tasks:**  
- Missing value treatment  
- Outlier capping  
- Data type corrections  
- Feature formatting  

---

### **US-03: PD Model Development**  
*As a Risk Modeler, I want to build a PD model so that I can assess borrower default probability.*

**Tasks:**  
- Train/test split  
- Logistic Regression baseline  
- ROC, AUC, KS evaluation  

---

## 🏃 Sprint Overview

### **Sprint 1**  
- Requirement analysis  
- Dataset exploration  
- Initial data cleaning  
- Jira board setup  

### **Sprint 2**  
- EDA  
- Feature engineering  
- PD model baseline development  

### **Sprint 3**  
- LGD/EAD modelling (future phase)  
- Model validation  

### **Sprint 4**  
- Documentation  
- Repo structuring  
- Cleanup and versioning  

---

## 📸 Jira Progress Screenshots

Actual Jira board screenshots from this project:

### **1️⃣ Board Progress – Screenshot 1**  
![Jira Board 1](./jira_screenshots/jira_board_progress_1.png)

### **2️⃣ Board Progress – Screenshot 2**  
![Jira Board 2](./jira_screenshots/Jira_Board_Progress_2.png)

---

🔬 6. Modelling Steps

**Step 1 — Data Cleaning**
- Handle missing values  
- Remove duplicates  
- Fix data types  
- Treat outliers  

**Step 2 — EDA**
- Statistical summary  
- Risk indicator exploration  
- Correlation heatmap  
- Target variable patterns  

**Step 3 — Feature Engineering**
- DTI  
- Utilization rate  
- Delinquency flags  
- Credit behaviour metrics  

**Step 4 — PD Model**
- Logistic Regression baseline  
- PD scoring & risk bands  
- Threshold tuning  

**Step 5 — Model Evaluation**
- AUC  
- KS Statistic  
- Confusion Matrix  
- Precision/Recall  

**Step 6 — IFRS-9 ECL Calculation**
- Stage 1 / Stage 2 / Stage 3 logic  
- Lifetime PD (future enhancement)  
- ECL = PD × LGD × EAD  

---

🛠️ 7. Future Enhancements

- XGBoost & Random Forest PD models  
- LGD and EAD modelling  
- Power BI dashboard  
- SQL-driven portfolio analytics  
- Streamlit model deployment  

---

👤 8. About the Author

**Amitabh Gogoi**  
Senior Manager – Credit Risk • Business Analyst • IFRS-9 ECL • Portfolio Analytics  
11+ years of professional experience in banking risk.

---

⭐ 9. Target Roles

- Credit Risk Modelling  
- Risk Analytics  
- IFRS-9 Model Validation  
- Data Analyst (Banking)  
- Business Analyst – Risk  

---

📌 10. Project Status

**Status:** In Progress  
**Next Milestone:** Complete EDA and begin baseline PD modelling.

