# Credit-Risk-Analysis-Loan-Default-Prediction
Machine learning model that predicts loan default risk from applicant financial data, achieving up to 96% accuracy.
Credit Risk Analysis – Loan Default Prediction

A machine learning project that predicts whether a loan applicant is likely to default (high credit risk) or repay (low credit risk), achieving up to 96% accuracy.

1. Problem Statement

Banks and NBFCs lend money every day, and some borrowers fail to repay. Each default causes financial loss, so lenders must decide who to lend to, how much, and at what interest rate.

Manual assessment is slow, subjective and inconsistent. This project builds a data-driven model that:

Learns patterns from historical borrower data
Predicts whether a new applicant is Good (low risk) or Bad (high risk)
Helps lenders approve safer loans faster and reduce Non-Performing Assets (NPAs)

Type of problem: Supervised learning, binary classification Target variable: 


Typical features used:

Demographics: age, gender, education, marital status
Financial: income, loan amount, loan term, existing debt, credit history
Behavioural: past payment delays, credit utilisation, number of credit lines
Employment: employment type, years of experience
3. Approach
Data Cleaning – handled missing values, duplicates and outliers
Exploratory Data Analysis (EDA) – distributions, correlations, default rate by segment
Feature Engineering – encoding categorical variables, scaling numeric features, creating ratios such as debt-to-income
Handling Class Imbalance – 
Model Building – trained and compared multiple classifiers:
Logistic Regression (baseline)
Decision Tree
Random Forest

Evaluation – train/test split with cross-validation, hyperparameter tuning
Model Selection – picked the best-performing model
4. Results
Model	Accuracy
Logistic Regression	86%
Decision Tree	94%
Random Forest	96%
Best model: Random Forest	up to 96%

Other metrics: Precision [], Recall [], F1-score [], ROC-AUC []

Credit data is usually imbalanced (far fewer defaulters than good borrowers), so accuracy alone can be misleading. Recall and ROC-AUC on the default class show how well the model catches risky borrowers.

5. Tech Stack
Python 3
pandas, NumPy
scikit-learn 
matplotlib, seaborn
Jupyter Notebook
6. Project Structure
credit-risk-analysis/
├── data/                # dataset (raw and cleaned)
├── notebooks/           # EDA and model training notebooks
├── src/                 # scripts (preprocessing, training)
├── models/              # saved model files
├── reports/             # project report PDF
├── requirements.txt
└── README.md
7. How to Run
bash
git clone <your-repo-url>
cd credit-risk-analysis
pip install -r requirements.txt
jupyter notebook notebooks/credit_risk_analysis.ipynb
