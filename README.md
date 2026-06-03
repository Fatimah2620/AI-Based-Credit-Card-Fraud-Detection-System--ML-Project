# AI-Based Credit Card Fraud Detection System

## Overview

This project presents a machine learning-based approach for detecting fraudulent credit card transactions. Due to the highly imbalanced nature of fraud datasets, the project focuses on improving fraud detection performance while minimizing false alarms.

The study compares multiple machine learning algorithms and evaluates their effectiveness using various performance metrics.

---

## Dataset

The dataset used in this project is the Credit Card Fraud Detection Dataset provided by ULB and available on Kaggle.

Dataset Link:
https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud

The dataset contains anonymized transaction features and a binary target variable indicating whether a transaction is fraudulent or legitimate.

---

## Installation

Clone the repository and install the required packages:

```bash
pip install -r requirements.txt
```

Download the dataset from Kaggle and place `creditcard.csv` in the project directory before running the notebook.

---

## Methodology

The project followed the following workflow:

1. Data preprocessing and exploratory data analysis (EDA)
2. Feature scaling using StandardScaler
3. Train-test split
4. Handling class imbalance using SMOTE
5. Model training and evaluation
6. Hyperparameter tuning using GridSearchCV
7. Feature selection analysis
8. Performance comparison and final model selection

---

## Models Evaluated

* Logistic Regression
* Decision Tree
* Random Forest

---

## Evaluation Metrics

The models were evaluated using:

* Accuracy
* Precision
* Recall
* F1-Score
* AUROC

These metrics were selected because the dataset is highly imbalanced and accuracy alone may be misleading.

---

## Results

### Best Model: Random Forest

| Metric    | Score  |
| --------- | ------ |
| Accuracy  | 99.95% |
| Precision | 92.41% |
| Recall    | 76.84% |
| F1-Score  | 83.91% |
| AUROC     | 0.9519 |

Random Forest achieved the best balance between fraud detection capability and false positive reduction, making it the final selected model.

---

## Key Findings

* Logistic Regression achieved the highest Recall but generated many false positives.
* Decision Tree showed moderate performance across metrics.
* Random Forest provided the best overall balance between Precision and Recall.
* Using all features achieved better performance than reduced feature subsets.
* SMOTE significantly improved learning from the minority fraud class.

---

## Project Files

* Credit_Card_Fraud_Detection.ipynb
* requirements.txt
* Final_Report.pdf
* Presentation.pdf

---

## Team Members

* Fatimah Alalawi
* Zainab Almousa
* Renad Aleid
* Shaikhah Aldossary
* Sara Buarish
* Fatimah Alnasser

Supervisor:
Dr. Sarah Alyami

---

## Technologies Used

* Python
* Pandas
* NumPy
* Scikit-learn
* Matplotlib
* Seaborn
* Google Colab

---

## License

This project was developed for academic purposes as part of the Machine Learning course at Imam Abdulrahman Bin Faisal University.
