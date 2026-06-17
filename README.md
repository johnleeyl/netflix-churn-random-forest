📊 Netflix Customer Churn Prediction (Random Forest)
📌 Project Overview

This project builds a machine learning model to predict whether a Netflix customer will churn (cancel subscription) based on their usage behavior and account details.

The goal is to help understand key drivers of churn so businesses can improve customer retention strategies.

📂 Dataset

The dataset contains 5,000 customers with the following features:

Demographics: age, gender, region
Usage behavior: watch hours, avg watch time per day, last login days
Subscription details: plan type, monthly fee, number of profiles
Preferences: device type, payment method, favorite genre
Target variable: churned (0 = stay, 1 = leave)
🧹 Data Preprocessing

Key steps performed:

Removed irrelevant column: customer_id
Handled categorical variables using One-Hot Encoding
Converted dataset into numerical format
Split data into training (80%) and testing (20%)
🤖 Model Used
Algorithm: Random Forest Classifier
Libraries: sklearn
Parameters:
n_estimators = 200
max_depth = 10
class_weight = "balanced"
📊 Model Performance
Accuracy: 97.3%
Precision / Recall / F1-score: ~0.97
Confusion Matrix:
[[489  10]
 [ 17 484]]
🔍 Feature Importance

Top features influencing churn:

avg_watch_time_per_day
watch_hours
last_login_days
number_of_profiles
monthly_fee

📌 Insight:
Customer engagement (watch behavior + login activity) is the strongest predictor of churn.

💡 Business Insight
Users with low engagement are more likely to churn
Improving watch time and activity can help reduce churn
Personalised recommendations and retention campaigns may improve customer retention
🛠️ Tech Stack
Python
Pandas, NumPy
Scikit-learn
Matplotlib
📈 Future Improvements
Try XGBoost / Gradient Boosting models
Add SHAP values for better explainability
Perform hyperparameter tuning
Build a dashboard (Streamlit / Power BI)
👤 Author

John Lee
Machine Learning Learning Project