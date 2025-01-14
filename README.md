# Advanced-Machine-Learning-Approaches-for-Credit-Card-Fraud-Detection-in-the-USA-25202
## Overview
This project focuses on detecting fraudulent credit card transactions using advanced machine learning techniques. Fraud detection is crucial for reducing financial losses, safeguarding customers, and maintaining the integrity of financial institutions.

The dataset consists of 100,000 transactions with the following columns:
- **TransactionID**: Unique identifier for each transaction.
- **TransactionDate**: Date of the transaction.
- **Amount**: Transaction amount in USD.
- **MerchantID**: Unique identifier for the merchant.
- **TransactionType**: Type of transaction (e.g., purchase, refund).
- **Location**: Location of the transaction.
- **IsFraud**: Target variable (1 indicates fraud, 0 indicates legitimate).

---

## Methodology

### 1. Data Preprocessing
- Handled missing values and outliers.
- Converted categorical variables using encoding techniques.
- Standardized numerical columns for uniform scaling.
- Addressed the class imbalance using **SMOTE** (Synthetic Minority Oversampling Technique).

### 2. Exploratory Data Analysis (EDA)
- Visualized transaction distribution by amount, type, location, and merchant.
- Explored time-series patterns to identify peaks in fraudulent activities.

### 3. Machine Learning Models
Implemented the following classification models to detect fraud:
1. **Logistic Regression**
2. **Random Forest Classifier**
3. **XGBoost Classifier**

Each model was trained on the processed dataset and evaluated using metrics like Accuracy, Precision, Recall, and F1-Score.

### 4. Model Evaluation and Comparison
The models were assessed based on their performance metrics and confusion matrices.

---

## Results

### 1. Logistic Regression
- **Accuracy**: 0.5862
- **Classification Report**:
| Metric       | Class 0 (Legit) | Class 1 (Fraud) | Macro Avg | Weighted Avg |
|--------------|----------------|-----------------|-----------|--------------|
| Precision    | 0.99           | 0.01            | 0.50      | 0.98         |
| Recall       | 0.59           | 0.44            | 0.51      | 0.59         |
| F1-Score     | 0.74           | 0.02            | 0.38      | 0.73         |

---

### 2. Random Forest Classifier
- **Accuracy**: 0.9741
- **Classification Report**:
| Metric       | Class 0 (Legit) | Class 1 (Fraud) | Macro Avg | Weighted Avg |
|--------------|----------------|-----------------|-----------|--------------|
| Precision    | 0.99           | 0.00            | 0.50      | 0.98         |
| Recall       | 0.98           | 0.01            | 0.49      | 0.97         |
| F1-Score     | 0.99           | 0.00            | 0.50      | 0.98         |

---

### 3. XGBoost Classifier
- **Accuracy**: 0.8721
- **Classification Report**:
| Metric       | Class 0 (Legit) | Class 1 (Fraud) | Macro Avg | Weighted Avg |
|--------------|----------------|-----------------|-----------|--------------|
| Precision    | 0.99           | 0.01            | 0.50      | 0.98         |
| Recall       | 0.88           | 0.12            | 0.50      | 0.87         |
| F1-Score     | 0.93           | 0.02            | 0.47      | 0.92         |

---

## Business Impact

### 1. Fraud Mitigation
- Improved fraud detection reduces financial losses for institutions and merchants.

### 2. Customer Protection
- Ensures the safety of customers’ financial assets and boosts trust in banking systems.

### 3. Operational Efficiency
- Automated fraud detection minimizes manual investigation efforts, saving time and resources.

### 4. Scalability
- The models, especially **Random Forest** and **XGBoost**, can handle large-scale datasets, making them suitable for real-world applications.

### Conclusion
This project demonstrates the application of advanced machine learning techniques to detect fraudulent credit card transactions. While Random Forest showed the highest accuracy, XGBoost provided a balance between precision and recall, making it a viable option for fraud detection. Future work may involve optimizing the SMOTE implementation and exploring deep learning approaches to further enhance detection capabilities.



