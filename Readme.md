# Analysis of Covid Dataset through Bayesian Regression

## Overview

This repository contains the implementation of a Bayesian regression analysis on a COVID-19 dataset. The objective is to predict hospital (`hospH8`) and ICU (`intcarH8`) admissions seven days ahead, leveraging Bayesian methods to achieve robust and interpretable results.

## Project Summary

The project involves the following steps:

1. **Data Preprocessing**:
   - Removal of unnecessary columns.
   - One-hot encoding of categorical variables.
   - Normalization of continuous variables.
   - Dataset shuffling for cross-validation.

2. **Modeling**:
   - Bayesian linear regression with the following priors:
     - Zellner g-prior.
     - Zellner-Siow prior.
     - Non-informative prior (BIC).
   - Model evaluation via cross-validation (Mean Squared Error as the metric).

3. **Predictive Analysis**:
   - Comparison of Bayesian Model Averaging (BMA) and Highest Posterior Model (HPM) estimators.
   - Identification of key covariates impacting predictions.

4. **Results**:
   - Non-informative prior (BIC) outperformed the other priors.
   - Covariates like `hosp` and `newpos_av7D` were most influential for hospital admission predictions, while `intcar` and `newpos_av7D` dominated ICU predictions.

## Repository Contents

- **`final_project_Baroni_Menozzi.pdf`**: Comprehensive project report with detailed explanations, results, and plots.
- Additional code and data files, if included, support the analysis.

## Main Findings

- Bayesian regression provides robust predictions for both hospital and ICU admissions.
- The choice of prior influences model performance, with BIC providing the best balance of accuracy and interpretability.
- Insights into the dataset revealed key predictors and highlighted the importance of handling outliers.

## Authors

- Stefano Baroni
- Alessia Menozzi
