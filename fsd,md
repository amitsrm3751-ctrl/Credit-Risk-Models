# Functional Specification Document (FSD)
## Credit Risk Modelling Project

### 1. Purpose
This FSD explains how the Credit Risk Model will work technically — including data inputs, processing steps, model logic, and outputs.

---

### 2. Data Requirements
**Input Dataset (from Kaggle):**
- Customer ID  
- Age  
- Income  
- Loan Amount  
- Credit Utilization  
- Number of Delinquencies  
- Credit Score (if available)  
- Employment Information  
- Default Flag (Target Variable)

**Data Format:**
- CSV file  
- All columns should be clean and numeric where possible  

---

### 3. Functional Workflow

#### **3.1 Data Collection**
- Download dataset from Kaggle  
- Save in `/data/raw/` folder  
- Load into Python using pandas  

#### **3.2 Data Preprocessing**
- Handle missing values  
- Remove duplicates  
- Convert categorical variables  
- Standardize or normalize values  
- Create train/test split  

#### **3.3 Exploratory Data Analysis (EDA)**
- Summary statistics  
- Histograms  
- Boxplots  
- Correlation heatmap  
- Target variable distribution  
- Identify key drivers of default  

#### **3.4 Feature Engineering**
- Debt-to-Income Ratio (DTI)  
- Credit Utilization Rate  
- Delinquency Flags  
- Age Bins (if needed)  
- Interaction features (optional)

#### **3.5 Model Development**
**Model Type:** Logistic Regression (baseline)

**Steps:**
- Fit model on training data  
- Predict probability of default (PD)  
- Use threshold = 0.5 (default)  

#### **3.6 Model Evaluation**
Metrics to calculate:
- AUC (Area Under ROC Curve)  
- KS Statistic  
- Confusion Matrix  
- Accuracy, Precision, Recall  

#### **3.7 IFRS-9 ECL Calculation**
- ECL = PD × LGD × EAD  
- LGD can be assumed (e.g., 45%)  
- EAD = Loan Amount  
- Stage Classification (optional):  
  - Stage 1 → PD < 30 days  
  - Stage 2 → SICR  
  - Stage 3 → Default  

---

### 4. Outputs

#### **4.1 Model Outputs**
- Probability of Default for each customer  
- Risk classification (Good/Bad)  
- Confusion Matrix results  

#### **4.2 ECL Outputs**
- ECL for each customer  
- Aggregate portfolio ECL  

#### **4.3 Visual Outputs**
- ROC curve  
- KS plot  
- Feature importance chart  
- ECL distribution  

---

### 5. Folder Structure

