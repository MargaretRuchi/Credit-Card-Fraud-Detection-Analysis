💳 Credit Card Fraud Detection using Machine Learning
📌 Project Overview

Credit card fraud poses significant financial risks to banks, merchants, and customers. Detecting fraudulent transactions is challenging because fraud cases represent only a tiny fraction of all transactions.

In this project, I developed multiple machine learning classification models to identify fraudulent credit card transactions and compared their performance using industry-standard evaluation metrics.

🎯 Objectives
Explore and understand transaction patterns.
Detect fraudulent transactions using supervised machine learning.
Compare multiple classification models.
Evaluate models using Accuracy, Precision, Recall, F1-score, and ROC-AUC.
Identify the best-performing model for fraud detection.
📂 Dataset

Source: Kaggle

Credit Card Fraud Detection Dataset

https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud

Dataset Information
Total Transactions: 284,807
Features: 31
Fraudulent Transactions: 492
Legitimate Transactions: 284,315

Fraud represents only 0.17% of all transactions, making this a highly imbalanced classification problem.

🛠 Tools & Libraries
Python
Google Colab
Pandas
NumPy
Matplotlib
Seaborn
Scikit-learn
📊 Exploratory Data Analysis

The analysis focused on understanding transaction behavior and identifying fraud patterns.

Visualizations include:

Transaction Time Distribution
Transaction Amount Distribution
Fraud vs Legitimate Transactions
Correlation Heatmap
Transaction Amount by Class
Confusion Matrix
⚙️ Data Preprocessing

The following preprocessing steps were performed:

Checked dataset dimensions
Verified data types
Confirmed no missing values
Checked class distribution
Split dataset into training and testing sets
Standardized numerical features where appropriate
🤖 Machine Learning Models

Three classification algorithms were trained and evaluated:

Logistic Regression
Decision Tree
Random Forest
📈 Model Performance
Logistic Regression

Accuracy: 97.55%

Metric	Score
Precision	0.06
Recall	0.92
F1-score	0.11
ROC-AUC	0.947
Decision Tree

Accuracy: 99.89%

Metric	Score
Precision	0.68
Recall	0.72
F1-score	0.70
ROC-AUC	0.862
Random Forest

Accuracy: 99.95%

Metric	Score
Precision	0.96
Recall	0.76
F1-score	0.85
ROC-AUC	0.878
🏆 Best Model
Random Forest

Random Forest achieved the strongest overall performance by balancing fraud detection accuracy with a very low false-positive rate.

Although Logistic Regression achieved the highest recall, it generated many false alarms due to low precision.

Random Forest provided:

Highest Accuracy
Highest Precision
Strong F1-score
Reliable fraud detection performance
📊 Key Insights
Fraud accounts for only 0.17% of all transactions.
Legitimate transactions dominate the dataset.
Transaction amount alone is not enough to identify fraud.
Random Forest performed best overall.
Logistic Regression captured most fraud cases but produced many false positives.
💡 Business Recommendations
Deploy Random Forest for production fraud detection.
Combine machine learning with rule-based fraud detection systems.
Continuously retrain models with recent transaction data.
Monitor fraud trends to improve model performance over time.
Prioritize high-risk transactions for manual review.
📁 Project Structure
Credit-Card-Fraud-Detection/

│── Credit Card Fraud Detection.ipynb

│── creditcard.csv

│── README.md

│── fraud_distribution.png

│── correlation_heatmap.png

│── transaction_amount.png

│── confusion_matrix.png

│── presentation.pdf
🚀 Skills Demonstrated
Data Cleaning
Exploratory Data Analysis
Data Visualization
Machine Learning
Classification
Model Evaluation
Fraud Analytics
Feature Analysis
Business Insights
Python Programming
📌 Conclusion

This project demonstrates how machine learning can effectively detect fraudulent credit card transactions despite a highly imbalanced dataset. By comparing multiple algorithms, Random Forest was identified as the most reliable model for balancing fraud detection accuracy and minimizing false positives.
