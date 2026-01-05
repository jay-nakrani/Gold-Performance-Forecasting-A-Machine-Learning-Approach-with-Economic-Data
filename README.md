# Gold Price Forecasting: A Machine Learning Approach

![Python](https://img.shields.io/badge/Python-3.7%2B-blue)
![Machine Learning](https://img.shields.io/badge/Machine-Learning-orange)
![Finance](https://img.shields.io/badge/Finance-Forecasting-green)

A machine learning project that explores the prediction of gold price direction using economic and market data. The repository includes both monthly and weekly forecasting frameworks developed at different stages of the project.

## Project Overview

This project investigates whether machine learning models can forecast whether gold prices will move **UP or DOWN** over future time periods. Two separate forecasting horizons are implemented:

- A **monthly forecasting framework**, used as an initial exploratory approach  
- A **weekly forecasting framework**, used for the final analysis and evaluation  

The models use U.S. economic indicators and market variables to capture macroeconomic conditions, financial stress, and commodity market dynamics.

## Data Sources

The project uses publicly available financial and economic data, including:

- Gold future prices (Yahoo Finance)
- U.S. Treasury yields (30-year)(Yahoo Finance)
- Inflation (CPI, FRED)
- U.S. Dollar Index (Yahoo Finance)
- Market volatility (Yahoo Finance)
- Oil and silver future prices (Yahoo Finance)

All datasets are cleaned, aligned, and transformed before feature engineering.

## Monthly Forecasting Framework

The monthly framework represents the early development stage of the project and focuses on predicting gold price direction on a **monthly horizon**.

### Characteristics
- Monthly resampled data  
- Basic economic and market features  
- No hyperparameter tuning  
- Simpler feature construction    

### Purpose
This framework was used to:
- Explore relationships between gold prices and macroeconomic variables  
- Test baseline machine learning models  
- Inform design decisions for the weekly framework  

## Weekly Forecasting Framework (Main Analysis)

The weekly framework forms the core contribution of the project and is used for the final modelling and analysis.

### Characteristics
- Weekly, non-overlapping sampling  
- More advanced feature engineering  
- Inclusion of real yield measures  
- Correlation-based and change-based features  
- Time-series cross-validation  
- Hyperparameter tuning  

### Feature Engineering
The weekly framework includes engineered features such as:
- Changes in real yields  
- Gold–yield and gold–silver correlations  
- Volatility-based indicators  
- Relative changes in market variables  
- Inflation changes aligned to weekly data  

Real yields are constructed following established economic research and represent the opportunity cost of holding gold.

## Machine Learning Models

The following classification models are implemented across the project:

- Logistic Regression  
- Ridge Classifier  
- Random Forest  

Models are trained to predict whether gold prices will move **up or down** in the following period. Feature scaling, regularisation, and class weighting are applied where appropriate.

## Model Evaluation

Model evaluation is carried out using:
- Accuracy  
- Balanced accuracy  
- Precision  
- Recall  
- F1 score  
- Confusion matrices  

Time-series cross-validation is used in the weekly framework to ensure that models are evaluated on unseen future data and to avoid look-ahead bias.
