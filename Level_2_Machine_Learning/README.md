Level 2 — Machine Learning

This folder contains two machine learning projects completed as part of my Codveda Technology internship. The projects demonstrate predictive modeling using supervised learning and customer segmentation using unsupervised learning.

Project 1: Regression Modeling

Notebook: Regression_Modeling.ipynb

Objective

Build and evaluate regression models to predict California house values using the California Housing dataset.

Methods

* Inspected the dataset and checked for missing values.
* Split the data into training and testing sets.
* Trained Linear Regression, Decision Tree, and Random Forest models.
* Evaluated performance using Mean Squared Error (MSE) and R².
* Used Optuna to explore Random Forest hyperparameters.
* Examined feature importance from the Random Forest model.

Results

The original Random Forest model performed best among the models tested, achieving an MSE of 0.2560 and an R² of 0.8046 on the test set. Hyperparameter tuning did not improve upon the original model’s performance.

Dataset

The California Housing dataset was loaded using fetch_california_housing from scikit-learn.

Project 2: Clustering (Unsupervised Learning)

Notebook: Kmeans_Clustering.ipynb

Selected internship task: Task 3 — Clustering (Unsupervised Learning).

Objective

Apply K-Means clustering to group customers according to similarities in age, annual income, and spending score.

Methods

* Inspected the dataset and checked for missing values and duplicate records.
* Explored the features using descriptive statistics and visualizations.
* Standardized the selected features.
* Used the elbow method to explore suitable cluster counts.
* Compared silhouette scores for cluster counts from 2 to 10.
* Compared four-cluster and six-cluster solutions.
* Used Principal Component Analysis (PCA) to visualize the clusters.
* Examined cluster sizes and average customer characteristics.

Results

The six-cluster solution achieved the highest silhouette score among the tested options, at 0.428. The resulting clusters revealed different customer profiles, including high-income customers with high spending and high-income customers with low spending.

The findings are exploratory. The silhouette score indicates moderate separation, and the identified groups should be interpreted in the context of the dataset.

Dataset

The project uses the Mall Customers dataset, saved locally as Mall_Customers.csv.

Tools and Libraries

* Python
* pandas and NumPy
* Matplotlib and Seaborn
* scikit-learn
* Optuna (regression project)
* Jupyter Notebook

How to Run

1. Clone or download this repository.
2. Open the Level_2_Machine_Learning folder in VS Code.
3. Open the required notebook.
4. Select a Python environment with the required libraries installed.
5. Run the notebook cells in order.

The regression notebook retrieves the California Housing dataset through scikit-learn. The clustering notebook uses the saved Mall_Customers.csv file.

Key Learning Outcomes

These projects provided practical experience in training and evaluating machine learning models, comparing model performance, tuning hyperparameters, standardizing features, selecting cluster counts, visualizing results, and interpreting model outputs.