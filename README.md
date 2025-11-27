# Gold Price Forecasting: A Machine Learning Approach

![Python](https://img.shields.io/badge/Python-3.7%2B-blue)
![Machine Learning](https://img.shields.io/badge/Machine-Learning-orange)
![Finance](https://img.shields.io/badge/Finance-Forecasting-green)

A comprehensive machine learning project that predicts gold price directions using economic indicators and technical analysis.

## 📊 Project Overview

This project develops predictive models to forecast whether gold prices will move **UP or DOWN** in the next month. The system combines:
- **Economic indicators** (Interest rates, USD Index, Inflation)
- **Technical indicators** (Moving averages, Momentum, Volatility)
- **Market sentiment** (VIX, Oil prices, Silver prices)

## 🚀 Key Features

- **Multi-source Data Integration**: Fetches real-time data from Yahoo Finance and FRED
- **Multiple ML Models**: Random Forest, XGBoost, and SVM with hyperparameter tuning
- **Economic Feature Engineering**: Real yield calculation based on Federal Reserve research
- **Comprehensive Visualization**: Correlation analysis and trend visualization
- **Time Series Validation**: Proper temporal splitting for financial data

## 📈 Model Performance

| Model | Accuracy | Precision | F1-Score |
|-------|----------|-----------|----------|
| Random Forest | 58.3% | 71.4% | 54.5% |
| XGBoost | 48.3% | 56.5% | 45.6% |
| SVM | 60.0% | 59.3% | 72.7% |

*SVM demonstrated the most balanced performance with the highest F1-Score*

## 🛠️ Installation

```bash
# Clone the repository
git clone https://github.com/yourusername/gold-price-forecasting.git

# Navigate to project directory
cd gold-price-forecasting

# Install required packages
pip install -r requirements.txt
