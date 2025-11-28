📘 Credit Risk Modelling Project

An end-to-end credit risk analytics project using Python, IFRS-9 ECL, and real-world banking workflows.

📌 1. Project Overview

This project demonstrates the complete lifecycle of a Credit Risk Modelling project used in banks and NBFCs. It includes:

Data Collection (Kaggle Dataset)

Data Cleaning & Preprocessing

Exploratory Data Analysis (EDA)

Feature Engineering

PD (Probability of Default) Model

Model Evaluation (AUC, KS, Confusion Matrix)

IFRS-9 Expected Credit Loss (ECL) Calculation

Documentation (User Stories, BRD, FSD)

Jira-based Agile Workflow

The goal is to build a transparent, auditable, and end-to-end risk analytics framework.

⚙️ 2. Tech Stack

Python (pandas, numpy, scikit-learn, matplotlib)

Jupyter Notebook

SQL (for portfolio-style queries)

IFRS-9 Framework (PD × LGD × EAD)

Jira (Scrum workflow)

GitHub (Version control & documentation)

📂 3. Project Structure
Credit-Risk-Models/
│
├── data/
│   ├── raw/                # Original dataset (from Kaggle)
│   └── processed/          # Cleaned/transformed data for modelling
│
├── notebooks/
│   ├── 01_data_cleaning.ipynb
│   ├── 02_eda.ipynb
│   ├── 03_pd_model.ipynb
│   └── 04_ecl_calculation.ipynb
│
├── docs/
│   ├── User_Stories.md
│   ├── BRD.md
│   └── FSD.md
│
├── jira_screenshots/
│   ├── jira_board_progress_1.png
│   └── (more as project progresses)
│
├── ifrs9_ecl/              # Future ECL components
├── pd_model/               # PD model scripts
├── lgd_ead_models/         # LGD/EAD models (future)
└── README.md               # You are here

📜 4. Documentation
🔹 User Stories

Defines functional expectations and user needs.
👉 /docs/User_Stories.md

🔹 Business Requirements Document (BRD)

Explains business goals, scope, and credit risk objectives.
👉 /docs/BRD.md

🔹 Functional Specification Document (FSD)

Technical workflow and model specifications.
👉 /docs/FSD.md

🚀 5. Agile Workflow (Jira Board)

The project follows a Scrum/Kanban workflow.

Current Board Status:

DONE: Dataset Collection

IN PROGRESS: EDA

IN REVIEW: Data Cleaning & Preprocessing

TO DO: Feature Engineering, PD Model, Model Evaluation, ECL Calculation

📸 Screenshot:
👉 /jira_screenshots/jira_board_progress_1.png

🔬 6. Modelling Steps
Step 1 — Data Cleaning

Handle missing values

Remove duplicates

Fix data types

Treat outliers

Step 2 — EDA

Statistical summary

Risk indicator exploration

Correlation heatmap

Target variable patterns

Step 3 — Feature Engineering

DTI

Utilization rate

Past delinquency flags

Credit behaviour metrics

Step 4 — PD Model

Logistic Regression baseline

PD scoring & risk bands

Threshold tuning

Step 5 — Model Evaluation

AUC

KS Statistic

Confusion Matrix

Precision/Recall

Step 6 — IFRS-9 ECL Calculation

Stage 1 / Stage 2 / Stage 3 logic (optional)

Lifetime PD (future enhancement)

ECL = PD × LGD × EAD

🛠️ 7. Future Enhancements

XGBoost & Random Forest PD models

LGD and EAD modelling

Power BI / Tableau dashboards

SQL-driven portfolio analytics

Streamlit model deployment

👤 8. About the Author

Amitabh Gogoi
Senior Manager – Credit Risk • Business Analyst • IFRS-9 ECL • Portfolio Analytics
11+ years of professional experience in banking risk.

⭐ 9. Target Roles

Credit Risk Modelling

Risk Analytics

IFRS-9 Model Validation

Data Analyst (Banking)

Business Analyst – Risk

📌 10. Project Status

Status: In Progress
Next Milestone: Complete EDA & begin baseline PD modelling.
