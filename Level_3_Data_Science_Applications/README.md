Level 3: Data Science Applications

This folder contains two projects completed as part of the Codveda Technology Data Science Internship:

1. Time-Series Analysis of USD Exchange Rates
2. NLP Text Classification using the SMS Spam Collection dataset

The projects apply statistical analysis and machine-learning techniques to two different problems: understanding exchange-rate behaviour over time and classifying text messages.

Project 1: Time-Series Analysis

Notebook: Time_Series_Analysis.ipynb

Dataset: cbn_exchange_rates_cleaned.csv

Objective

Analyse historical USD central exchange rates using data collected from the Central Bank of Nigeria (CBN), identify time-series patterns, compare forecasting methods, and generate future forecasts.

Workflow

* Filter the cleaned exchange-rate data to US dollar observations.
* Handle duplicate dates and aggregate daily observations into monthly averages.
* Explore the series and decompose it into trend, seasonal, and residual components.
* Apply moving averages and exponential smoothing.
* Test stationarity using the Augmented Dickey–Fuller (ADF) test.
* Explore autocorrelation and partial autocorrelation.
* Fit and compare ARIMA and SARIMA models.
* Evaluate forecasts using RMSE and MAE, including comparisons with naive baselines.
* Examine residuals and use the Ljung–Box test to check for residual autocorrelation.
* Visualise a 12-month forecast and its prediction interval.

Key Finding

In the walk-forward evaluation, the ordinary naive baseline achieved lower forecast errors than the ARIMA and SARIMA models tested. The future forecasts illustrate the limitations of extrapolating historical exchange-rate patterns when substantial changes occur.

The forecasts are model-based estimates, not guarantees of future exchange-rate movements. The latest monthly observation is incomplete because the available daily data ends on 9 October 2026.

Project 2: NLP Text Classification

Notebook: NLP_Text_Classification.ipynb

Dataset: SMSSpamCollection

Objective

Develop a text-classification workflow to distinguish spam messages from legitimate SMS messages, commonly labelled spam and ham.

Workflow

* Load and inspect the SMS dataset.
* Examine labels, missing values, duplicates, and class distribution.
* Clean and preprocess text.
* Convert text into numerical features using text-vectorisation techniques.
* Train classification models.
* Evaluate performance using appropriate classification metrics, including precision, recall, and F1-score.
* Interpret the results and consider the limitations of automated spam detection.

Dataset Files

* SMSSpamCollection — SMS message data and labels.
* SMSSpamCollection_readme.txt — accompanying dataset documentation.

Files in This Folder

File	Purpose
Time_Series_Analysis.ipynb	Time-series analysis, forecasting, and model evaluation
cbn_exchange_rates_cleaned.csv	Cleaned exchange-rate dataset
NLP_Text_Classification.ipynb	SMS spam text-classification workflow
SMSSpamCollection	SMS message dataset
SMSSpamCollection_readme.txt	Dataset documentation
README.md	Overview of the Level 3 projects

Tools and Libraries

* Python
* pandas and NumPy
* Matplotlib and Seaborn
* statsmodels
* scikit-learn
* NLTK
* Jupyter Notebook

Reproducing the Work

1. Ensure Python and the libraries used in the relevant notebook are installed.
2. Open the notebook in Jupyter Notebook or Visual Studio Code.
3. Confirm that the dataset files are available at the paths expected by the notebook.
4. Run the notebook cells in order to reproduce the analysis and results.

The exact results depend on the dataset, preprocessing decisions, model settings, and software environment.

Summary

These projects demonstrate the application of time-series analysis, forecasting, natural-language processing, and classification techniques to practical data-science tasks. They also highlight the importance of comparing models against baselines, evaluating results honestly, and documenting analytical limitations.