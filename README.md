# Milagro Store Profitability Forecasting

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
