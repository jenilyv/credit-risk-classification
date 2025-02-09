#Credit Risk Classification Analysis

## Overview
This analysis aims to predict the credit risk of loans using a logistic regression model trained on historical lending data. By evaluating the model's performance, we assess its ability to classify loans as either **healthy (0)** or **high-risk (1)** with a focus on accuracy, precision, recall, and overall reliability.

## Results

- **Accuracy:** 99%
- **Precision:**
  - Class **0 (Healthy Loans)**: 1.00  
  - Class **1 (High-Risk Loans)**: 0.84  
- **Recall:**
  - Class **0 (Healthy Loans)**: 0.99  
  - Class **1 (High-Risk Loans)**: 0.94  
- **F1-score:**
  - Class **0 (Healthy Loans)**: 1.00  
  - Class **1 (High-Risk Loans)**: 0.89  

## Analysis
- The model demonstrates **high overall accuracy (99%)**, meaning it correctly classifies the vast majority of loan applications.
- **Precision for high-risk loans (0.84)** indicates that when the model predicts a loan as high-risk, there is a slight chance of false positives.
- **Recall for high-risk loans (0.94)** is strong, meaning the model successfully identifies most of the actual high-risk loans.
- **The model performs exceptionally well on healthy loans** (Precision & Recall both near 1.00), but some misclassifications occur for high-risk loans.
- A **Convergence Warning** was observed, suggesting that the model reached the iteration limit before full optimization. This could be addressed by increasing `max_iter` or scaling the data.

## Recommendation
While the model performs very well, **there is a slight trade-off in precision for high-risk loans**. If the company wants to avoid false positives (incorrectly labeling a loan as high-risk), further tuning or alternative models (e.g., Random Forest, Gradient Boosting) could be considered. However, given its strong recall and high overall accuracy, **this model is reliable for credit risk classification.**

## Next Steps
- **Address the Convergence Warning** by increasing `max_iter` in the logistic regression model.
- **Further improve high-risk loan classification** by testing other models like Decision Trees, Random Forest, or Gradient Boosting.
- **Perform feature engineering** to improve model performance by identifying key predictors of loan risk.

