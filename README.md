# Coupon Response Prediction and Budget Optimization

## 1. Project Overview

This project simulates a retail CRM scenario where coupon budgets are limited. The goal is to predict which customers are more likely to repurchase after receiving an offer and to optimize coupon targeting under budget constraints.

## 2. Business Problem

When coupon budget is limited, which customers should be prioritized to maximize repeat buyer coverage and coupon efficiency?

## 3. Data Source

The project is based on the Acquire Valued Shoppers Challenge dataset.

Raw data is not included in this repository due to file size. Please refer to `data/README.md` for data download and placement instructions.

## 4. Project Architecture

Business Problem  
→ Data Cleaning  
→ Feature Engineering  
→ RFM Baseline  
→ XGBoost Model  
→ TopK Business Evaluation  
→ Budget Simulation  
→ Business Review

## 5. Key Metrics

- Repeater Capture Rate@K
- Repeat Trips Capture Rate@K
- Lift@K
- Unit Coupon Efficiency
- AUC
- PR-AUC
- LogLoss

## 6. Project Boundary

This project focuses on response prediction and offline ranking evaluation. It does not directly estimate causal uplift or true incremental ROI because there is no randomized non-treatment control group.

## 7. Repository Structure

```text
coupon-response-prediction/
├── config/
├── data/
├── docs/
├── sql/
├── notebooks/
├── src/
├── reports/
├── outputs/
├── README.md
└── requirements.txt