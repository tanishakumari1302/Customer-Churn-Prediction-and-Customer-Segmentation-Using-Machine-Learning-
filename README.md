Customer Churn Prediction and Customer Segmentation Using Machine Learning
ML project that predicts customer churn using classification models like Logistic Regression and Random Forest. Includes EDA, feature engineering, model training, and customer segmentation to help businesses reduce churn rate.

Project Overview
Customer churn is one of the major challenges faced by telecom companies. This project predicts whether a customer is likely to leave the company and segments customers into different groups using Machine Learning techniques. The insights generated from this project can help businesses improve customer retention and make better marketing decisions.

 Objectives

* Analyze customer behavior using Exploratory Data Analysis (EDA)
* Predict customer churn using Machine Learning
* Identify important features affecting churn
* Segment customers using K-Means Clustering
* Generate business insights for customer retention

Dataset

Dataset: Telco Customer Churn Dataset

The dataset contains customer demographic information, services subscribed, billing details, and churn status.

Target Variable:

Churn Value
1:Customer Left
0:Customer Stayed

Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* SciPy
* Google Colab

Project Workflow

1. Data Cleaning & Preprocessing
2. Exploratory Data Analysis (EDA)
3. Hypothesis Testing
4. Feature Engineering & Encoding
5. Train-Test Split
6. Random Forest Classification
7. Hyperparameter Tuning
8. Feature Importance Analysis
9. Churn Probability Prediction
10. Customer Segmentation using K-Means
11. Model Evaluation & Business Insights

Machine Learning Model

Algorithm Used: Random Forest Classifier

Model evaluation was performed using:

* Accuracy
* Precision
* Recall
* F1-Score
* Confusion Matrix
* Classification Report

Hyperparameter tuning and class balancing were applied to improve model performance.
Customer Segmentation

K-Means Clustering was used to group customers based on:

* Tenure Months
* Monthly Charges
* Total Charges
* Churn Probability

The Elbow Method was used to determine the optimal number of clusters.

Key Features

* Customer Churn Prediction
* Customer Segmentation
* Feature Importance Analysis
* Hyperparameter Tuning
* Churn Probability Analysis
* Business Insights through Data Visualization

 Business Impact

This project helps organizations:

* Predict customer churn in advance
* Identify high-risk customers
* Improve customer retention strategies
* Support data-driven business decisions

Future Improvements

* XGBoost / LightGBM Implementation
* Streamlit Dashboard
* Real-Time Prediction API
* Automated Customer Retention Recommendations

Project Structure

text
Dataset/
EDA & Data Cleaning/
Machine Learning/
Segmentation/
README.md

How to Run

1. Clone this repository.
2. Install the required libraries.
3. Add the **Telco_customer_churn.xlsx** dataset.
4. Run the notebooks in sequence:

   * EDA & Data Cleaning
   * Machine Learning
   * Segmentation

 Conclusion

This project demonstrates an end-to-end Machine Learning workflow for predicting customer churn and segmenting customers based on their behavior. By combining Random Forest Classification with K-Means Clustering, the project provides meaningful business insights that can help telecom companies reduce customer churn and improve retention strategies.
