# Digital Payment Fraud Detection & Risk Analysis

## Project Overview
Analysed 6.3 million financial transactions to identify 
fraud patterns, build a predictive model, and create an 
interactive dashboard for business decision making.

## Tools Used
- Python (Pandas, Scikit-learn, Seaborn, Matplotlib)
- SQL (SQLite)
- Tableau Public
- Google Colab

## Dataset
- Source: Kaggle — Financial Transactions Dataset
- Size: 6.3 million rows, 11 columns
- Fraud rate: 0.13% (highly imbalanced)

## Key Findings
1. Fraud occurs ONLY in TRANSFER and CASH_OUT transactions
2. Fraud rate peaks at 22% between 3-5 AM
3. 500K+ transactions have highest fraud concentration
4. Fraudsters target high balance accounts — avg fraud 
   amount is 8x higher than normal transactions (14.7L vs 1.78L)
5. Account drain pattern — fraud empties 88% of sender balance

## Model Performance
- Algorithm: Random Forest + SMOTE
- Fraud Catch Rate: 96.03%
- Overall Accuracy: 98%
- Strongest Predictor: Sender opening balance (37.6% importance)

## Dashboard
Live Tableau Dashboard: [Click Here] (https://public.tableau.com/app/profile/sucheta.de7420/viz/DigitalPaymentFraudDetectionAnalysis/DigitalPaymentFraudAnalysis?publish=yes))

## Project Structure
- `Fraud_Detection_Analysis.ipynb` — Complete Python notebook
- `sql_fraud_by_type.csv` — SQL analysis results by type
- `sql_fraud_by_amount.csv` — SQL analysis results by amount
- `sql_fraud_by_hour.csv` — SQL analysis results by hour
- `sql_account_drain.csv` — Account drain analysis
- `sql_fraud_by_day.csv` — Daily fraud trend

## Dashboard Preview
![Dashboard](fraud_by_type.png)
