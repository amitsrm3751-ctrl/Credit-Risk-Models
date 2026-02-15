📊 Probability of Default (PD) Model

This module contains the complete development of the Probability of Default (PD) model using a WOE-based logistic regression approach.

🎯 Objective

Estimate borrower-level Probability of Default (PD) in a transparent and interpretable manner aligned with regulated banking practices and IFRS-9 PD estimation requirements.

🧱 Model Development Approach
1️⃣ Data Preparation

Train–test split performed prior to feature engineering

WOE (Weight of Evidence) transformation applied using training data only

Identical bin mappings applied to the test dataset

Variables evaluated using Information Value (IV)

2️⃣ Final Features Used

age_woe

DPD_30_59_woe

DPD_60_89_woe

MonthlyIncome_woe

Delinquency variables showed strongest predictive power, consistent with real-world retail credit portfolios.

🧠 Model Type

Logistic Regression (Maximum Likelihood Estimation using statsmodels)

Why statsmodels?

Provides coefficient significance (p-values)

Enables statistical inference

Suitable for regulatory documentation

📈 Model Performance (Test Set)
Metric	Value
AUC	~0.79
Gini	~0.59
KS	~0.44

The model demonstrates strong discriminatory power and clear separation between good and bad accounts.

🔢 Scorecard Conversion

The logistic regression output (log-odds) was converted into an operational credit score using:

Base Score: 600

Points to Double Odds (PDO): 20

Score scaling formula:

Score = Offset − Factor × Log(Odds)

Risk bands were created using:

Quantile segmentation

Fixed operational cut-offs

Observed default rates show strong monotonic behavior across score bands.

✅ Strengths

Fully interpretable

Monotonic risk structure via WOE

Regulatory-friendly framework

Suitable for IFRS-9 PD integration

Transparent scorecard implementation

📂 Related Files

WOE-transformed datasets: data/processed/

Model notebook: notebooks/

IFRS-9 integration: /ifrs9_ecl/
