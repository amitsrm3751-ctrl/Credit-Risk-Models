# Business Requirements Document (BRD)
## Credit Risk Modelling Project

### 1. Project Purpose
The purpose of this project is to build a basic Credit Risk Model that predicts the Probability of Default (PD) and calculates IFRS-9 Expected Credit Loss (ECL).  
The project uses publicly available data from Kaggle.

---

### 2. Objectives
- Understand key drivers of credit risk.
- Build a simple PD model to classify good vs bad customers.
- Calculate ECL using PD × LGD × EAD.
- Present the results with clear insights and visualizations.
- Document the entire workflow for reference.

---

### 3. Scope
**In Scope**
- Data collection from Kaggle  
- Data cleaning and preprocessing  
- Exploratory Data Analysis (EDA)  
- PD model development  
- Model evaluation (AUC, KS, Confusion Matrix)  
- Basic IFRS-9 ECL calculation  
- Final report/dashboard  

**Out of Scope**
- Production deployment  
- Real bank data  
- Advanced ML algorithms  

---

### 4. Stakeholders
- **Data Analyst:** Collect and prepare the data  
- **Credit Risk Analyst:** Perform EDA and insights  
- **Modeller:** Build the PD model  
- **Reviewer:** Validate model performance  
- **Manager:** Use outputs for decision-making  

---

### 5. High-Level Requirements
1. Download dataset from Kaggle.  
2. Prepare and clean the dataset.  
3. Perform EDA to understand key variables.  
4. Build a PD model (Logistic Regression or similar).  
5. Evaluate model using AUC, KS, and Confusion Matrix.  
6. Calculate IFRS-9 ECL.  
7. Create final summary/report.  

---

### 6. Success Criteria
- PD model AUC ≥ 0.70  
- KS score ≥ 25  
- Clean and well-organized GitHub repository  
- Clear and understandable documentation  

---

### 7. Deliverables
- User Stories  
- BRD  
- FSD  
- Clean dataset  
- EDA notebook  
- PD model notebook  
- Validation metrics  
- IFRS-9 ECL calculations  
- Final dashboard or summary report  
