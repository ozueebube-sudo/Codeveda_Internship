Codveda Technology Data Science Internship

This repository documents my practical work during the Codveda Technology Data Science Internship. It contains projects covering data collection and preprocessing, machine learning, and data science applications.

The projects demonstrate my developing skills in Python, data analysis, data preprocessing, statistical modelling, machine learning, text classification, and time-series forecasting.

Repository Overview

Level	Focus	Projects
Level 1	Data Collection and Preprocessing	CBN exchange-rate data scraping and preprocessing
Level 2	Machine Learning	Regression modelling and K-Means customer segmentation
Level 3	Data Science Applications	SMS spam classification and USD exchange-rate time-series analysis

Level 1: Data Collection and Preprocessing

Folder: Level_1_Data_Collection_and_Preprocessing/

This level focuses on collecting, inspecting, and preparing real-world data for analysis.

Project: CBN Exchange-Rate Data

The project involves collecting exchange-rate data from the Central Bank of Nigeria (CBN) and preparing it for subsequent analysis.

Key files:

* CBN_Exchange_Rate_Scraping.ipynb — notebook for collecting exchange-rate data.
* cbn_exchange_rates_raw.csv — raw collected data.
* cbn_exchange_rates_cleaned.csv — cleaned exchange-rate data.
* cbn_exchange_rates_preprocessed.csv — preprocessed data.

Level 2: Machine Learning

Folder: Level_2_Machine_Learning/

This level explores supervised and unsupervised machine-learning techniques.

Project 1: Regression Modelling

* Notebook: Regression_Modeling.ipynb
* Dataset: California Housing dataset, accessed through scikit-learn.
* Objective: Predict a continuous housing-value target and compare regression models.
* Methods: Regression modelling, model evaluation, hyperparameter tuning, and feature-importance analysis.

Project 2: Customer Segmentation

* Notebook: Kmeans_Clustering.ipynb
* Dataset: Mall Customers.
* Objective: Explore customer groups using demographic and spending-related features.
* Methods: Feature scaling, the elbow method, silhouette analysis, K-Means clustering, and PCA visualisation.

Key data files:

* Mall_Customers.csv — original customer dataset.
* Mall_Customers_clustered.csv — customer data with cluster assignments.

Level 3: Data Science Applications

Folder: Level_3_Data_Science_Applications/

This level applies data-science techniques to text classification and time-series forecasting.

Project 1: Time-Series Analysis

* Notebook: Time_Series_Analysis.ipynb
* Dataset: CBN exchange-rate data, filtered to the US dollar.
* Objective: Examine historical exchange-rate patterns and develop forecasts.
* Methods: Time-series decomposition, moving averages, exponential smoothing, stationarity testing, ARIMA/SARIMA modelling, forecast evaluation, and residual diagnostics.

Project 2: NLP Text Classification

* Notebook: NLP_Text_Classification.ipynb
* Dataset: SMS Spam Collection.
* Objective: Classify SMS messages as spam or legitimate messages (ham).
* Methods: Text preprocessing, numerical text representation, machine-learning classification, and evaluation using classification metrics.

Key data files:

* cbn_exchange_rates_cleaned.csv — cleaned exchange-rate data used for the time-series project.
* SMSSpamCollection — SMS messages and their labels.
* SMSSpamCollection_readme.txt — accompanying dataset documentation.

Tools and Technologies

* Programming: Python
* Data manipulation: pandas, NumPy
* Visualisation: Matplotlib, Seaborn
* Machine learning: scikit-learn
* Statistical and time-series modelling: statsmodels
* Text processing: NLTK and scikit-learn
* Development environment: Jupyter Notebook and Visual Studio Code
* Version control: Git and GitHub

How to Explore the Projects

1. Open the folder for the level you want to explore.
2. Read its README.md for project-specific details, where available.
3. Open the relevant Jupyter notebook to review the workflow, code, visualisations, and conclusions.
4. Check the accompanying dataset files and the dataset documentation where provided.

Learning Outcomes

Through these projects, I have gained practical experience in:

* Collecting, inspecting, cleaning, and preparing datasets.
* Exploring data and communicating findings through visualisations.
* Building and evaluating regression and clustering models.
* Processing text and developing classification workflows.
* Analysing time-series patterns and evaluating forecasts.
* Documenting analytical decisions, interpreting model results, and recognising limitations.
* Organising project files and publishing work with Git and GitHub.

About This Repository

This repository serves as a record of my hands-on learning and project development during the Codveda Technology Data Science Internship. Each level builds on practical analytical skills, from preparing data to applying machine-learning and forecasting techniques.