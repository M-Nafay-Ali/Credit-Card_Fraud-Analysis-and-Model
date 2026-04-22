Note:- All of this is done on Mobile phone and with the guidance of Ai and for practice purpose


Credit Card Fraud Detection Pipeline:-

End-to-End Machine Learning & Fraud Analytics:-
This project focuses on identifying fraudulent credit card transactions using a dataset of 339,000+ records. The goal was to build a robust system capable of distinguishing normal spending behavior from high-risk fraudulent activity, specifically addressing the challenge of Class Imbalance.


🎯 Project Objectives:-
Exploratory Data Analysis (EDA): Identify behavioral patterns in fraud, such as time of day and transaction categories.
Feature Engineering: Transform raw timestamps into usable features like hour and calculate customer age from date-of-birth data.
Predictive Modeling: Train a Random Forest Classifier to automate fraud detection.
Optimization: Implement Random Over-Sampling (ROS) to improve the model's ability to catch rare fraud cases (Recall).


📊 Key Findings from Analysis:-
The Midnight Spike: Data analysis revealed a significant increase in fraudulent activity between 11 PM and 3 AM, suggesting that attackers target hours when cardholders are less likely to monitor their phones.
Category Vulnerability: Certain categories like grocery_pos and shopping_net showed higher rates of suspicious activity compared to others.
Demographic Insights: By calculating age, I was able to visualize whether specific age groups were disproportionately affected by fraudulent attempts.


🛠️ Machine Learning Implementation:-
1. Handling Class Imbalance
In the raw data, fraud accounted for less than 1% of total transactions. To prevent the model from being biased toward "Normal" transactions, I used the imblearn library to perform Random Over-Sampling. This balanced the training set and allowed the model to learn the specific characteristics of fraudulent behavior.
2. Feature Importance
Using the feature_importances_ attribute of the Random Forest model, I identified that the Transaction Amount (amt) and the Time of Day (hour) were the most critical factors in predicting fraud.


📂Tech Stack:-
Language: Python
Libraries: Pandas, NumPy, Scikit-Learn, Imbalanced-Learn
Visualization: Plotly (Interactive Charts), Seaborn (Heatmaps)
Environment: Google Colab

📈 Results & Performance:-
Initial Model: High accuracy, but low Recall for fraud (missed nearly half of the fraudulent cases).
Optimized Model: After oversampling, the Recall improved significantly, ensuring that a much higher percentage of actual frauds were successfully flagged by the system.


📬 Connect with Me
M. Nafay Ali
2nd Year ICS Student | Data Science Aspirant
[https://github.com/M-Nafay-Ali] | [https://www.linkedin.com/in/mohammed-nafay-ali-16519138a?utm_source=share&utm_campaign=share_via&utm_content=profile&utm_medium=android_app]
