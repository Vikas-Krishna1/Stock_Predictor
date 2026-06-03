# Stock Predictor App

A machine learning project that uses historical S&P 500 market data to predict whether the market will move up or down on the following trading day. The project leverages Yahoo Finance data and a Random Forest classification model to generate predictions and evaluate performance.

## Overview

This project demonstrates an end-to-end machine learning workflow for financial market prediction:

* Download historical S&P 500 data from Yahoo Finance
* Clean and preprocess market data
* Engineer prediction targets
* Train a Random Forest classifier
* Generate market direction predictions
* Evaluate model performance using historical test data

The project is intended for educational purposes and provides hands-on experience with data science, machine learning, and financial data analysis.

## Features

* Historical S&P 500 data retrieval using Yahoo Finance
* Data preprocessing and feature engineering
* Binary classification of market direction
* Random Forest machine learning model
* Train/test split evaluation
* Performance analysis and prediction reporting

## Technologies Used

* Python
* Jupyter Notebook
* Pandas
* NumPy
* Scikit-learn
* yfinance
* Matplotlib

## Project Structure

```text
stock_predictor_app/
│
├── stock_trader.ipynb      # Main notebook
├── requirements.txt        # Project dependencies
├── README.md               # Documentation
├── .gitignore
└── venv/                   # Virtual environment (excluded from Git)
```

## Installation

### Clone the Repository

```bash
git clone https://github.com/YOUR_USERNAME/stock-predictor-app.git
cd stock-predictor-app
```

### Create a Virtual Environment

```bash
python -m venv venv
```

Activate the environment:

macOS/Linux:

```bash
source venv/bin/activate
```

Windows:

```bash
venv\Scripts\activate
```

### Install Dependencies

```bash
pip install pandas numpy yfinance scikit-learn matplotlib jupyter
```

## Running the Project

Launch Jupyter Notebook:

```bash
jupyter notebook
```

Open:

```text
stock_trader.ipynb
```

Run all cells to:

1. Download S&P 500 historical data
2. Create prediction targets
3. Train the Random Forest model
4. Generate predictions
5. Evaluate results

## Machine Learning Model

The project uses a Random Forest Classifier with:

```python
RandomForestClassifier(
    n_estimators=200,
    min_samples_split=100,
    random_state=1
)
```

### Input Features

* Open
* High
* Low
* Close
* Volume

### Target Variable

The target is whether the market closes higher on the next trading day.

* 1 = Market increases
* 0 = Market decreases or remains unchanged

## Educational Objectives

This project demonstrates:

* Financial data collection
* Feature engineering
* Classification models
* Model training and testing
* Performance evaluation
* Python data science workflows

## Future Improvements

Potential enhancements include:

* Additional technical indicators
* Moving averages
* RSI and MACD indicators
* Hyperparameter tuning
* Cross-validation
* Deep learning models
* Real-time prediction dashboard
* Streamlit web application deployment

## Disclaimer

This project is intended for educational and research purposes only. It does not provide financial advice, investment recommendations, or guarantees of future market performance. Always conduct independent research before making investment decisions.

## Author

Vikas Krishna

