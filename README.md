# **Bank Marketing Effectiveness Prediction**
------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
This project aims to predict whether clients will subscribe to a bank's term deposit by employing various machine learning techniques, including Logistic Regression, Decision Trees, Random Forest, Gradient Boosting, XGBoost, K Nearest Neighbor, Naive Bayes, and Support Vector Machine. The objective is to determine the most effective method for forecasting client subscriptions to term deposits.

# **Problem Statement**
The project analyzes data from a Portuguese bank's phone-based marketing campaigns to forecast if clients will subscribe to a term deposit ('yes' or 'no'). The dataset includes client details and campaign information. The primary objectives are data cleaning, handling class imbalance, building prediction models, and evaluating their performance to enhance marketing campaign targeting and effectiveness.

# **Dataset Attributes**

-Age: Age of the client

-Job: Type of job

-Marital: Marital status

-Education: Qualification of the client

-Default: Indicates if the client has credit in default

-Balance: Account balance of the client

-Housing: Indicates if the client has a housing loan

-Loan: Indicates if the client has a personal loan

-Contact: Communication type

-Month: Last contact month of the year

-Day: Last contact day of the month

-Duration: Last contact duration in seconds

-Campaign: Number of contacts performed during this campaign and for this client

-Pdays: Number of days that passed by after the client was last contacted from a previous campaign

-Previous: Number of contacts performed before this campaign and for this client

-Poutcome: Outcome of the previous marketing campaign

-Y (Target Variable): Indicates if the client subscribed to a term deposit ('yes' or 'no')

#**Data Cleaning and Preprocessing**

Handling Duplicates: Dataset contained no duplicated values.
Handling Null Values: Replaced null values with mode; features with null values over 50% were removed.
Handling Outliers: Used Interquartile Range to remove outliers.
Feature Encoding: Applied label encoding for limited categories and one-hot encoding for large categories.
Handling Imbalanced Dataset: Employed SMOTE technique to address class imbalance.
Data Scaling: Utilized MinMaxScaler to scale the dataset.
Exploratory Data Analysis (EDA)
Performed extensive EDA using Matplotlib and Seaborn, drawing conclusions regarding client demographics, behaviors, and their likelihood to subscribe based on various features.

#**ML Model Building**
Implemented several models: Logistic Regression, Decision Tree, Random Forest, Gradient Boosting Machine, XGBoost, K Nearest Neighbor, Naive Bayes, and Support Vector Machine.

#**Model Evaluation**
Models and their accuracy scores:

- Logistic Regression: 0.91
- Decision Tree: 0.82
- Random Forest: 0.86
- Gradient Boosting Machine: 0.92
- XGBoost: 0.93
- K Nearest Neighbor: 0.91
- Naive Bayes: 0.85
- Support Vector Machine: 0.91
- XGBoost outperformed other models across various classification evaluation metrics.

#**Model Explainability and Feature Importance**

Identified top five features impacting predictions: Duration, Age, Month (May), Housing, and Day, indicating their influence on the model's predictions.

#**Conclusion**

-XGBoost Model Performance: Exhibited the highest accuracy, precision, recall, F1-score, and a close-to-one roc auc score.

-Recommendation: The XGBoost classification model, trained using cross-validation, stands out as the ideal model for predicting client subscriptions to term deposits due to its superior performance metrics (accuracy: 0.936, precision: 0.93, recall: 0.93, F1-score: 0.93, roc auc: 0.93).
