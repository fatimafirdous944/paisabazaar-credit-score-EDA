# Paisabazaar Credit Score Analysis (EDA + Classification)

Exploratory data analysis and a machine learning model to predict customer credit scores (Poor / Standard / Good) for Paisabazaar.

## Project Overview
Paisabazaar helps customers find and apply for banking and credit products. Assessing creditworthiness accurately helps reduce loan defaults and improve financial product recommendations. This project analyses customer data to find what drives credit score and builds a model to predict it.

## Dataset
- 100,000 monthly records for 12,500 customers (8 months each), 28 columns
- Features include income, number of loans and credit cards, interest rate, payment delays, outstanding debt, credit utilisation, credit history and payment behaviour
- Target: `Credit_Score` (Poor 29.0%, Standard 53.2%, Good 17.8%)
- Dataset provided by Paisabazaar as part of the internship project

## What is in the notebook
- Data exploration, missing-value checks and data wrangling
- 15 charts (univariate, bivariate and multivariate) with insights and business impact
- 3 hypothesis tests (Mann-Whitney U, Chi-square, Kruskal-Wallis)
- Feature engineering and preprocessing (outlier capping, transformation, encoding, scaling)
- 3 models with hyperparameter tuning: Logistic Regression, Random Forest, Gradient Boosting
- Feature importance and saved model (joblib)

## Key Findings
- Credit mix, interest rate, payment delay, outstanding debt and credit-history length are the strongest drivers of credit score
- Poor-score customers: average interest rate 20.2%, payment delay about 30 days, 4.8 loans
- Good-score customers: average interest rate 7.7%, payment delay about 11 days, 2.2 loans
- Paying only the minimum amount is a strong warning sign
- Occupation and credit utilisation have little effect

## Model Result
The tuned Random Forest was selected: **69.0% accuracy, macro-F1 0.681** on a customer-level held-out test set.

## How to run
1. Open `Paisabazaar_Credit_Score_EDA.ipynb` in Google Colab
2. Upload `dataset-2.csv` to the Colab Files panel
3. Run all cells (Runtime > Run all)

## Tools
Python, pandas, NumPy, Matplotlib, Seaborn, SciPy, scikit-learn

## Author
[Fatima Firdous]
