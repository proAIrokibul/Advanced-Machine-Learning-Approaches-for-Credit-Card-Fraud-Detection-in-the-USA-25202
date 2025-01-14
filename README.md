# Advanced Machine Learning Approaches for Credit Card Fraud Detection in the USA

## Project Overview
Credit card fraud poses significant challenges to financial institutions, leading to billions of dollars in losses annually. This project leverages advanced machine learning algorithms to build an effective fraud detection system. The primary goal is to identify fraudulent transactions accurately while minimizing false positives, thereby ensuring customer trust and operational efficiency.

The dataset used in this project consists of 100,000 transactions with the following attributes:
- **TransactionID**: Unique identifier for each transaction.
- **TransactionDate**: Date of the transaction.
- **Amount**: Transaction amount in USD.
- **MerchantID**: Unique identifier for the merchant.
- **TransactionType**: Type of transaction (e.g., purchase, refund).
- **Location**: Geographical location of the transaction.
- **IsFraud**: Binary target variable indicating fraud (1) or legitimate transaction (0).

---

## Methodology

### 1. Data Preprocessing
- **Data Cleaning**: Addressed missing values and outliers for robust analysis.
- **Feature Engineering**: Encoded categorical features and standardized numerical variables for uniformity.
- **Class Imbalance Handling**: Applied **SMOTE (Synthetic Minority Oversampling Technique)** to address the significant class imbalance in the target variable.

### 2. Exploratory Data Analysis (EDA)
- Conducted detailed visualizations to identify patterns in transaction amounts, types, locations, and time-series trends.
- Uncovered insights into fraudulent transaction distributions, seasonal patterns, and high-risk categories.

### 3. Machine Learning Models
Implemented the following supervised classification models:
1. **Logistic Regression**: A baseline model to understand linear relationships.
2. **Random Forest Classifier**: A robust ensemble method leveraging bagging and feature importance.
3. **XGBoost Classifier**: A gradient-boosted decision tree model optimized for performance.

### 4. Model Evaluation and Comparison
Each model was assessed using the following metrics:
- **Accuracy**: Overall correctness of predictions.
- **Precision**: The proportion of predicted fraud cases that were actual frauds.
- **Recall**: The ability to identify actual fraud cases.
- **F1-Score**: The harmonic mean of precision and recall.
- **Confusion Matrix**: Visualization of prediction results.
- **Classification Report**: Detailed analysis of precision, recall, and F1-scores for each class.

---

## Results and Insights

### Logistic Regression
- **Accuracy**: 58.62%
- **Classification Report**:
            precision    recall  f1-score   support

       0       0.99      0.59      0.74     19602
       1       0.01      0.44      0.02       198
      accuracy                     0.59     19800
