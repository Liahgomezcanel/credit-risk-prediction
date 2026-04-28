# credit-risk-prediction
ML model predicting credit loan default risk using XGBoost | ROC-AUC 0.75 | Python
# Credit Default Risk Prediction

A machine learning project that predicts whether a loan applicant is likely to default,
built using real-world banking data from Home Credit Group.

## Overview

Financial institutions lose billions annually to loan defaults. This project builds
a predictive model that flags high-risk applicants before loan approval,
using demographic, financial, and behavioral features.

## Results

| Model | ROC-AUC |
|---|---|
| Logistic Regression | 0.74 |
| Random Forest | 0.72 |
| **XGBoost (best)** | **0.75** |

## Key Findings

- External credit scores (EXT_SOURCE_2 & 3) are the strongest predictors of default, 
  accounting for ~20% of model predictive power
- Education level, employment stability, and age are significant socioeconomic predictors
- Class imbalance (only 8% defaulters) required threshold optimization — best threshold 
  found at 0.65
- XGBoost outperformed other models due to its ability to handle non-linear relationships 
  in imbalanced financial data

## Tech Stack

- Python, Jupyter Notebook
- Pandas, NumPy
- Scikit-learn
- XGBoost
- Matplotlib, Seaborn

## Dataset

[Home Credit Default Risk](https://www.kaggle.com/competitions/home-credit-default-risk) — 
307,511 loan applications with 122 features.

## How to Run

1. Download application_train.csv from:
   https://www.kaggle.com/competitions/home-credit-default-risk/data
2. Place it in the same folder as the notebook
3. Install dependencies: pip install -r requirements.txt
4. Open credit_risk.ipynb in Jupyter Notebook
5. Run all cells in order

## Project Structure

- credit_risk.ipynb — Main notebook with full analysis
- requirements.txt — Project dependencies
- README.md — Project documentation

## Author

**Liah Gomez** — Economics graduate with banking experience  
[LinkedIn](www.linkedin.com/in/liah-gomez-010889324) · 
