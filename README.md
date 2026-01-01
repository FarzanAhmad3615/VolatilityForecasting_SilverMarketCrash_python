# SilverMarketCrash_python29dec25


## Overview

This repository contains two sophisticated financial analysis projects leveraging **Machine Learning**, **State-Space Modeling**, and **Natural Language Processing (NLP)**. The projects focus on comparative model performance in stock price prediction and systemic risk analysis in the commodities market.

---

## Project 1: Silver Market Crash Analysis & Volatility Forecasting

This project investigates high-volatility silver futures () using a custom-built machine learning pipeline to identify liquidity vacuums and price reversal triggers.

### **Technical Highlights**

* **Predictive Modeling:** Implements a **Random Forest Regressor** to analyze commodity behavior, ranking price proximity to the 200-day Moving Average and volume changes as top indicators.
* **Sentiment Integration:** Synthesizes market psychology scores with technical indicators to quantify the impact of news events (e.g., Margin Hikes, ATHs) on price stability.
* **Visual Analytics:** Features a high-fidelity dark-themed dashboard built with **Matplotlib** to synchronize spot price action with underlying sentiment shifts.

---

## Project 2: Multi-Model Stock Price Forecasting

A comparative analysis framework evaluating four distinct modeling paradigms on their ability to capture stochastic market behavior.

### **The STAR Framework Analysis**

* **Situation:** Financial markets exhibit non-linear, stochastic behavior, making traditional linear forecasting often ineffective.
* **Task:** Build an end-to-end Python pipeline to implement, optimize, and compare **ARIMA**, **VARMAX**, **GARCH**, and **LSTM** models.
* **Action:** * Resolved **numerical stability issues** (`LinAlgError`) by implementing a `StandardScaler` and `diffuse initialization`.
* Developed a Deep Learning **LSTM** network in **TensorFlow/Keras** using a sliding window sequence generator.
* Optimized multivariate convergence using the **Powell optimizer**.


* **Result:** The LSTM model demonstrated clear superiority in capturing complex temporal patterns, achieving a **MAPE of 1.45%**, while traditional models struggled with mean-reversion flatlining.

### **Model Performance Metrics**

| Model | MAE | RMSE | MAPE |
| --- | --- | --- | --- |
| **LSTM** | **1.4552** | **1.7973** | **1.4533%** |
| **ARIMA** | 2.8053 | 3.6023 | 2.7842% |
| **VARMAX** | 4.8912 | 6.0239 | 4.8598% |

---

## Tech Stack

* **Languages:** Python (Pandas, NumPy, Scikit-learn)
* **Deep Learning:** TensorFlow, Keras
* **Econometrics:** Statsmodels (ARIMA, VARMAX), Arch (GARCH)
* **Data API:** yfinance
* **Visualization:** Matplotlib, Seaborn

## Setup and Execution

1. **Install Dependencies:**
`pip install pandas numpy matplotlib yfinance scikit-learn tensorflow statsmodels arch`
2. **Dataset:** The scripts automatically pull live/historical data via the Yahoo Finance API or use provided `stock_data.csv`.
3. **Run:** Execute the Python scripts to generate the performance metrics and synchronized visualizations.
<img width="923" height="634" alt="smc" src="https://github.com/user-attachments/assets/b185c84b-1a25-41ad-9a97-388bbbab778d" />
