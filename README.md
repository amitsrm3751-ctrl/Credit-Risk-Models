# 📘 Credit Risk Modelling & Scorecard Project

An end-to-end Probability of Default (PD) modelling and monitoring project built using Python and structured risk governance practices.

This repository demonstrates a realistic banking-style credit risk workflow including feature engineering, model validation, scorecard logic, and model monitoring using PSI.

---

# 🎯 Project Objective

To build a transparent, interpretable, and governance-ready PD model using structured risk modelling practices consistent with regulated banking environments.

This project focuses on:

- Data cleaning & preprocessing  
- Exploratory Data Analysis (EDA)  
- Feature engineering with WOE & IV  
- Logistic Regression PD modelling  
- Model validation (AUC, KS, Gini, Confusion Matrix)  
- Population Stability Index (PSI) for monitoring  
- IFRS-9 staging logic (conceptual demonstration)  
- Agile project tracking using Jira  

---

# ⚠️ Scope Clarification

This dataset does **not** contain recovery or exposure-level information required for robust LGD and EAD modelling.

Accordingly:

- This project delivers a complete **PD modelling lifecycle**
- LGD and EAD modelling are formally deferred to a future project using suitable recovery/exposure datasets

This reflects proper model governance and dataset suitability review.

---

# 📊 Exploratory Data Analysis (EDA) Summary

The EDA phase focused on identifying behavioral risk indicators and validating statistical integrity before modelling.

## 🔍 Key Observations

### 1️⃣ Borrower Age
- Right-skewed distribution
- Majority between 30–60 years
- Limited noise from extreme age bands

### 2️⃣ Revolving Utilization
- Highly skewed
- Strong relationship with default
- Outliers present

### 3️⃣ Debt Ratio
- Wide distribution
- Defaulters show higher median DTI

### 4️⃣ Delinquency Buckets (Most Predictive)

| Bucket | Interpretation |
|--------|----------------|
| 30–59 DPD | Early stress signal |
| 60–89 DPD | Escalating financial distress |
| 90+ DPD | Strong default proxy |

Strong correlations exist between delinquency stages, reflecting behavioral progression risk.

---

# 🧱 Feature Engineering & WOE Transformation

The modelling workflow follows regulated credit risk practices.

## Controls Implemented

- Train–test split performed before binning
- WOE & IV calculated using training data only
- Identical bin mappings applied to test data
- Monotonic risk behavior validated

## Variables Retained

| Variable | Treatment | Decision |
|-----------|-----------|----------|
| Age | Quantile WOE binning | ✅ Kept |
| 30–59 DPD | Business bins | ✅ Kept |
| 60–89 DPD | Business bins | ✅ Kept |
| Monthly Income | Quantile bins | ✅ Kept |

Variables showing instability or weak predictive strength were excluded.

---

# 📈 PD Model Development

## Model Type
- Logistic Regression

## Training Approach
- WOE-transformed features
- No data leakage
- Proper train-test separation

## Evaluation Metrics

- ROC-AUC
- KS Statistic
- Gini Coefficient
- Confusion Matrix
- Threshold tuning

The model demonstrates strong discriminatory power while maintaining interpretability.

---

# 📊 Model Monitoring — Population Stability Index (PSI)

To ensure model robustness over time, PSI was implemented.

## PSI Measures:

- Distribution shift between training and new population
- Score-level monitoring
- Drift interpretation thresholds

This step reflects real-world model governance and post-deployment validation.

---

# 🏦 IFRS-9 Staging Logic (Conceptual Demonstration)

The project demonstrates IFRS-9 staging logic using PD outputs:

- Stage 1 → Performing (12-month PD)
- Stage 2 → Significant Increase in Credit Risk
- Stage 3 → Default (90+ DPD proxy)

ECL formula illustrated:

ECL = PD × LGD × EAD

(Note: LGD and EAD modelling require separate recovery/exposure dataset and are scoped for future project.)

---

# ⚙️ Tech Stack

- Python (pandas, numpy, scikit-learn, matplotlib)
- Jupyter Notebook
- Jira (Scrum tracking)
- GitHub (Version control & documentation)

---

# 📁 Project Structure

Credit-Risk-Models/
│
├── data/
│   ├── raw/
│   ├── processed/
│
├── notebooks/
│   ├── 01_data_cleaning.ipynb
│   ├── 02_eda.ipynb
│   ├── 03_woe_binning.ipynb
│   ├── 04_pd_model_logistic.ipynb
│   ├── 05_psi_monitoring.ipynb
│
├── jira_screenshots/
│
├── BRD.md
├── FSD.md
├── User_Stories.md
└── README.md

---

# 🧭 Agile Workflow (Jira)

The project was tracked using a structured Scrum-style workflow:

- Epics aligned with modelling phases
- User stories tied to credit risk objectives
- Tasks moved across:
  - Backlog → In Progress → In Review → Done
- Scope revision formally documented after dataset suitability review

This reflects governance-driven risk project execution.

---

# 🚀 Future Enhancements

- XGBoost PD comparison
- Bayesian PD modelling
- Survival analysis (Cox PH)
- LGD modelling using recovery datasets
- EAD modelling using exposure datasets
- Full IFRS-9 ECL production pipeline

---

# 📌 Project Status

✅ EDA Completed  
✅ Feature Engineering & WOE Completed  
✅ PD Model Built & Validated  
✅ PSI Monitoring Implemented  
🔜 LGD & EAD Modelling (Future Dataset-Based Project)

📅 Last Updated: February 2026

---

# 👤 About the Author

**Amitabh Gogoi**  
Manager – Credit Analysis and Risk  
IFRS-9 • Scorecards • Portfolio Analytics • Risk Governance  

11+ years of banking risk experience.
