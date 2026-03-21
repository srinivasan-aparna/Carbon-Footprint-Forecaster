# Carbon Emission Prediction using Machine Learning
This project focuses on predicting individual carbon emissions using demographic, lifestyle, and consumption patterns. The goal is to identify key drivers of emissions and build interpretable as well as high-performing predictive models.

# 🚀 Key Contributions

## Data Preprocessing & Feature Engineering

Cleaned and transformed raw survey data with 60%+ missing values handling
Encoded categorical variables and engineered features from multi-label fields (e.g., cooking methods, recycling habits)
Standardized numerical features using training statistics to avoid data leakage
Created domain-specific transformations (e.g., transport → vehicle type mapping)

##  Modeling & Experimentation

Built and compared multiple models:
Linear Regression (baseline, interaction-heavy)
Regularized models (Elastic Net via glmnet)
Random Forest
XGBoost
Neural Networks
Designed interaction-rich models capturing nonlinear relationships between lifestyle variables
Performed 10x5 repeated cross-validation for robust evaluation

## Model Evaluation

Evaluated models using:
RMSE, MAE, MSE
AIC/BIC for model complexity comparison
Identified best-performing model based on generalization performance

## Interpretability & Insights

Analyzed feature importance across models
Built Partial Dependence Plots (PDPs) to understand interaction effects
Conducted error analysis to identify hard-to-predict user segments
Used Bland-Altman plots to assess prediction reliability

# 📊 Key Insights
Transportation type and distance traveled are strong predictors of emissions
Interaction effects (e.g., transport × vehicle type) significantly improve performance
Certain user groups (e.g., high consumption + large waste generation) are harder to model accurately

# 🖥️ Tech Stack
Languages: R, Python

Libraries: tidyverse, caret, tidymodels, glmnet, xgboost, pdp, GGally 

Concepts: Feature engineering, model tuning, cross-validation, interpretability
