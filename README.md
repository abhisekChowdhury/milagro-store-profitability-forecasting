# Milagro Store Profitability Forecasting

## Case Attribution

This project is based on the business case **“Milagro: Predicting Store Profitability at a Fast-Casual Restaurant Chain”**,  
originally written by Prof. Robert Freund and Phil Zakahi.

The analysis and modeling work in this repository represents my own
implementation and interpretation of the case, adapted and extended
for educational and portfolio purposes.

## How to Run

### Option 1: Run in Google Colab (Recommended)
1. Open the notebook:
   `notebooks/profitability_modeling.ipynb`
2. Upload the notebook to Google Colab
3. Upload the CSV files from the `data/` folder when prompted
4. Run all cells top to bottom

### Option 2: Run Locally
1. Clone the repository
2. Install dependencies:
	pip install pandas numpy statsmodels scikit-learn matplotlib
3. Run the notebook using Jupyter:

## Problem Statement
A fast-casual restaurant chain is expanding aggressively and needs to
forecast profitability for 48 new store locations currently under construction.
The analysis was conducted in the context of a private equity due diligence
process, where both predictive accuracy and business constraints matter.

## Dataset
- 459 existing store locations
- 374 used for training, 85 for testing
- Features include demographics, store size, competition, labor costs,
  and location characteristics

## Approach
- Built multiple linear regression models
- Evaluated out-of-sample performance using test R²
- Assessed statistical significance and multicollinearity
- Compared four models with different complexity and business alignment

## Models Evaluated
- **Model A:** Baseline regression with core predictors
- **Model B:** Full model using all available features
- **Model C:** Parsimonious model reducing multicollinearity
- **Model D:** Business-constrained model balancing accuracy and profitability

## Key Results
- Best predictive accuracy: Model C (Test R² ≈ 0.84)
- Business-aligned choice: Model D
  - Test R² ≈ 0.77
  - Total predicted profitability ≈ $40.1M (meets business target)

## Business Insight
This project highlights a common real-world analytics tradeoff:
the most statistically accurate model is not always the best decision-making
tool when business constraints are present.

## Tech Stack
Python, pandas, numpy, statsmodels, scikit-learn

## Data Disclaimer
The dataset used in this project is based on a classroom business case
and is shared here strictly for educational and demonstration purposes.

