# Customer-Churn-Prediction-and-Customer-Segmentation-Using-Machine-Learning-
ML project that predicts customer churn using classification models like Logistic Regression and Random Forest. Includes EDA, feature engineering, model training, and customer segmentation to help businesses reduce churn rate.

 Project Overview

Customer retention has become one of the most important challenges in the telecommunications industry. Acquiring new customers is often more expensive than retaining existing ones. Therefore, identifying customers who are likely to leave the service and understanding customer behavior patterns are crucial for business growth and profitability.

This project focuses on predicting customer churn using Machine Learning techniques and identifying different customer groups through customer segmentation. By combining predictive analytics and clustering techniques, the system helps businesses detect high-risk customers, understand customer behavior, and develop effective retention strategies.

The project incorporates data analysis, statistical testing, machine learning classification, model optimization, and customer segmentation techniques to generate meaningful business insights.

 Problem Statement

Telecommunication companies experience customer loss due to multiple factors such as:

* High monthly subscription charges
* Unsatisfactory customer support
* Contract type and billing plans
* Payment methods
* Lack of additional services
* Customer dissatisfaction

The challenge is to identify customers who are likely to churn before they leave and categorize customers into meaningful segments for targeted business actions.

 Project Objectives

The primary objectives of this project are:

* Analyze customer behavior using exploratory data analysis.
* Identify factors influencing customer churn.
* Perform statistical validation through hypothesis testing.
* Build an accurate churn prediction model using Random Forest.
* Improve model performance using hyperparameter tuning.
* Evaluate model performance using multiple metrics.
* Calculate churn probability for individual customers.
* Segment customers based on behavioral and financial characteristics.
* Generate actionable business insights for customer retention.

 Dataset Description

Dataset Used: Telco Customer Churn Dataset

The dataset contains demographic, service-related, billing, and customer behavior information.

 Customer Information

* Customer ID
* Gender
* Senior Citizen
* Partner
* Dependents

 Service Information

* Phone Service
* Multiple Lines
* Internet Service
* Online Security
* Online Backup
* Device Protection
* Tech Support
* Streaming TV
* Streaming Movies

 Billing Information

* Contract Type
* Paperless Billing
* Payment Method
* Monthly Charges
* Total Charges

Target Variable

* Churn Value

Where:

* 1 = Customer Left
* 0 = Customer Retained

---

 Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-Learn
* SciPy
* Google Colab

 Exploratory Data Analysis (EDA)

EDA was performed to understand customer behavior patterns and identify important relationships within the dataset.

The following analyses were conducted:

 Tenure Analysis

* Distribution of customer tenure.
* Relationship between tenure and churn.

 Monthly Charges Analysis

* Distribution of monthly charges.
* Impact of charges on customer churn.

 Contract Type Analysis

* Comparison of churn rates across different contract types.

 Payment Method Analysis

* Investigation of churn behavior across payment methods.

Tech Support Analysis

* Relationship between technical support availability and churn.

Correlation Analysis

* Heatmap visualization of numerical feature relationships.

Key observations revealed that customers with shorter tenure and higher monthly charges were more likely to churn.

---

Hypothesis Testing

To statistically validate important findings, hypothesis testing was performed.

 T-Test

The independent T-Test was used to determine whether Monthly Charges and Tenure Months differ significantly between churned and retained customers.

 Chi-Square Test

The Chi-Square Test was used to evaluate the relationship between Contract Type and Customer Churn.

These statistical tests provided evidence that certain customer characteristics significantly influence churn behavior.

 Data Preprocessing

 Missing Value Handling

The "Total Charges" column contained missing values.

Steps performed:

* Converted Total Charges to numeric format.
* Replaced missing values with zero.

 Feature Selection

The following columns were removed:

* CustomerID
* Country
* State
* City
* Zip Code
* Latitude
* Longitude
* Churn Label
* Churn Reason

These columns were either identifiers or contained information not useful for prediction.

Encoding

Categorical variables were converted into numerical form using One-Hot Encoding:

python
pd.get_dummies(drop_first=True)

This transformation made the dataset compatible with machine learning algorithms.

Machine Learning Model

Train-Test Split

The dataset was divided into:

* 80% Training Data
* 20% Testing Data

This ensured proper evaluation on unseen data.

Random Forest Classifier

Random Forest was selected because:

* Handles high-dimensional datasets effectively.
* Reduces overfitting through ensemble learning.
* Provides feature importance rankings.
* Produces reliable classification results.

Working Principle

Random Forest creates multiple decision trees using random subsets of data.

Each tree makes an independent prediction, and the final prediction is determined through majority voting.

Model Evaluation

The model was evaluated using:

 Accuracy

Measures overall prediction performance.

Precision

Measures correctness of churn predictions.

Recall

Measures the model's ability to identify actual churn customers.

 F1 Score

Balances Precision and Recall.

 Confusion Matrix

Provides detailed classification outcomes.

 Classification Report

Summarizes Precision, Recall, F1-Score, and Support.

 Model Optimization

Class Imbalance Handling

To improve churn detection:

python
class_weight='balanced'

was implemented.

Hyperparameter Tuning

Different combinations of:

* Number of Trees
* Maximum Tree Depth

were tested.

Performance metrics compared:

* Accuracy
* Precision
* Recall
* F1 Score

The best-performing configuration was selected.

Feature Importance Analysis

Feature importance scores were extracted from the Random Forest model.

This analysis identified the most influential variables affecting customer churn.

Examples include:

* Contract Type
* Monthly Charges
* Tenure Months
* Total Charges
* Internet Services

The results provided valuable business insights regarding customer retention.

Churn Probability Analysis

Instead of predicting only churn or non-churn status, the model also generated churn probabilities.

This helped classify customers into:

* High Risk Customers
* Medium Risk Customers
* Low Risk Customers

Businesses can use these probabilities to prioritize customer retention efforts.

Customer Segmentation Using K-Means Clustering

Customer segmentation was performed using K-Means Clustering.

 Features Used

* Tenure Months
* Monthly Charges
* Total Charges
* Churn Probability

 Feature Scaling

StandardScaler was applied before clustering.

Elbow Method

The Elbow Method was used to determine the optimal number of clusters.

Customer Segments

The clustering process identified distinct customer groups:

 Cluster 0 – Loyal Customers

* Long tenure
* Low churn probability

Cluster 1 – High Risk Customers

* Higher churn probability
* Require retention strategies

Cluster 2 – Premium Customers

* Higher spending
* Greater customer value

These segments help businesses develop personalized marketing and retention plans.

Business Impact

The developed system can help organizations:

* Predict customer churn before it occurs.
* Reduce revenue loss.
* Improve customer retention.
* Identify high-risk customers.
* Design targeted marketing campaigns.
* Improve customer lifetime value.
* Support strategic business decision-making.

 Future Enhancements

Future improvements may include:

* XGBoost and LightGBM Models
* Deep Learning Approaches
* Streamlit Dashboard Integration
* Real-Time Prediction System
* Automated Retention Recommendation Engine
* Cloud Deployment
* Customer Feedback Analysis

 MConclusion

This project successfully combines machine learning classification and customer segmentation techniques to address the critical problem of customer churn in the telecommunications industry.

The project began with comprehensive exploratory data analysis and statistical hypothesis testing to understand customer behavior and validate important relationships within the dataset. Data preprocessing techniques such as missing value handling, feature selection, and categorical encoding were applied to prepare the dataset for modeling.

A Random Forest Classifier was developed to predict customer churn with high reliability. Several optimization techniques including class balancing, hyperparameter tuning, feature importance analysis, and performance evaluation metrics were implemented to improve prediction quality and model robustness.

In addition to churn prediction, customer segmentation was performed using K-Means Clustering. This enabled the identification of distinct customer groups based on tenure, spending behavior, and churn probability. Such segmentation provides valuable business intelligence and supports personalized customer retention strategies.

Overall, the project demonstrates how machine learning can be used not only for prediction but also for generating actionable business insights. The developed system can assist telecom companies in reducing customer attrition, improving customer satisfaction, increasing profitability, and making data-driven business decisions.

The integration of predictive analytics, statistical validation, and customer segmentation makes this solution a practical and scalable framework for modern customer retention management systems.
