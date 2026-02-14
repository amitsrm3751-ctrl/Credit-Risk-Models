# 📘 Credit Risk Modelling & Scorecard Project

An end-to-end retail credit risk modelling project built using real-world banking methodology, including WOE transformation, PD modelling, statistical validation, and credit scorecard development aligned with IFRS-9 principles.

---

## 📌 Project Overview

This project demonstrates the complete lifecycle of a retail Probability of Default (PD) model used in banks and NBFCs:

- Data cleaning & preprocessing  
- Exploratory Data Analysis (EDA)  
- WOE (Weight of Evidence) transformation  
- Information Value (IV) validation  
- Logistic Regression (scikit-learn & statsmodels)  
- Model evaluation (AUC, KS, Gini)  
- Credit Scorecard creation  
- Risk band segmentation  
- IFRS-9 ECL framework integration (PD × LGD × EAD)

The objective is to build a transparent, interpretable, regulator-aligned credit risk model consistent with real-world scorecard practices.

---

## 🧱 Modelling Workflow

### 1️⃣ Data Preparation
- Missing value treatment  
- Outlier handling  
- Feature validation  
- Train–test split (performed before binning to avoid leakage)

### 2️⃣ WOE & IV Transformation
- Quantile and business-driven binning  
- WOE calculated using training data only  
- IV used for variable selection  
- Monotonic risk behavior validation  
- Identical bin mapping applied to test data  

### 3️⃣ PD Model Development
- Logistic Regression using WOE-transformed features  
- Statistical inference using **statsmodels** (p-values, coefficients)  
- Feature significance validation  

### 4️⃣ Model Evaluation (Out-of-Sample Test Set)

| Metric | Result |
|--------|--------|
| AUC | ~0.80 |
| Gini | ~0.60 |
| KS | ~0.44 |

The model demonstrates strong discriminatory power and stable separation between good and bad borrowers.

### 5️⃣ Credit Scorecard Implementation
- Log-odds converted to score using linear scaling  
- Score range approx. **550–725**  
- Higher score → Lower probability of default  
- Monotonic risk ranking validated  

#### 📊 Business Risk Segmentation (Fixed Cut-offs)

| Risk Band | Approx. Default Rate |
|------------|----------------------|
| Very High Risk | ~51% |
| High Risk | ~27% |
| Medium Risk | ~6% |
| Low Risk | ~1% |

Default rates decrease consistently as score increases, confirming correct calibration.

---

## 📁 Project Structure

```
credit-risk-models/
│
├── data/
│   ├── raw/
│   └── processed/
│       ├── pd_model_train_woe.csv
│       └── pd_model_test_woe.csv
│
├── notebooks/
│   ├── 01_data_cleaning.ipynb
│   ├── 02_eda.ipynb
│   ├── 03_woe_binning.ipynb
│   ├── 04_pd_model_logistic.ipynb
│   └── 05_scorecard.ipynb
│
├── docs/
│   ├── BRD.md
│   ├── FSD.md
│   └── User_Stories.md
│
└── README.md
```

---

## ⚙️ Tech Stack

- Python (pandas, numpy)
- scikit-learn
- statsmodels
- matplotlib
- Jupyter Notebook
- IFRS-9 Framework (PD × LGD × EAD)
- GitHub
- Jira (Agile tracking)

---

## 📐 Key Credit Risk Concepts Implemented

- Weight of Evidence (WOE)
- Information Value (IV)
- Logistic Regression (MLE)
- Statistical significance (p-values)
- ROC Curve
- AUC / Gini
- KS Statistic
- Score scaling
- Risk band segmentation
- IFRS-9 staging logic (conceptual integration)

---

## 🚀 Future Enhancements

- Random Forest / XGBoost benchmarking
- LGD and EAD modelling
- Lifetime PD framework
- Portfolio analytics dashboard
- Streamlit scorecard deployment

---

## 👤 About the Author

**Amitabh Gogoi**  
Manager – Credit Risk  
11+ years of experience in retail banking credit analysis risk and portfolio analytics.

---

## 📌 Project Status

✅ PD Model & Credit Scorecard Completed  
🔄 IFRS-9 ECL Expansion In Progress  
📅 Last Updated: February 2026
