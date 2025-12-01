# Coustmer-Churn-Predection




# Overview
Customer churn prediction is essential for businesses—especially telecom, banking, and subscription-based companies. By building accurate churn prediction models, organizations can reduce revenue loss and improve customer satisfaction.
This repository contains a data science project aimed at predicting customer churn using machine learning techniques. The entire analysis, from data preprocessing to model evaluation, is conducted in a Jupyter Notebook environment.This project implements several ML algorithms, applies proper preprocessing techniques, and compares performance metrics to determine the most effective model.

# Objectives

- Understand the factors that influence customer churn.
- Build predictive models to identify potential churners.
- Provide actionable insights to reduce churn rates.

# Dataset

The dataset contains customer records including demographic information, account details, and service usage metrics. The target variable indicates whether a customer has churned (1) or not (0).


# Customer Churn Prediction using Machine Learning:
This project focuses on predicting customer churn using multiple machine learning models and comparing their performance. The dataset contains customer demographic details and service usage behavior. The main objective is to identify customers likely to churn so that proactive retention strategies can be implemented.


# Key Features of the Project
Data preprocessing with dataset splitting and feature scaling
Multiple ML algorithms implemented
Model performance comparison using Accuracy, Precision, Recall, and F1-score
Hybrid Logit Ensemble model for improved performance
Ensures reproducibility with fixed random seed
Visualization and evaluation included (if present in notebook)

# Dataset Processing
## 1. Dataset Splitting
For a dataset with 505,257 samples, and an 80-20 split:

ntrain = 505,257 × 0.8 = 404,205  
ntest  = 505,257 × 0.2 = 101,052
A fixed random seed ensures consistent results and avoids data leakage.

## 2. Feature Scaling
Numerical features are standardized using:
𝑋 scaled = 𝑋−𝜇/𝜎

This ensures:
Faster model convergence
Equal contribution of all features
Improved performance in distance-based algorithms like KNN, SVM, and Logistic Regression

# Machine Learning Models Used
The following models were trained and evaluated:
Logistic Regression
K-Nearest Neighbors (KNN)
Decision Tree
Random Forest
XGBoost
LightGBM
AdaBoost
Logit Hybrid Ensemble (custom ensemble)

Each model was tested on unseen test data to ensure robust evaluation.

# Model Performance Comparison:

| Model                       | Accuracy (%) | F1-score (%) | Precision (%) | Recall (%) |
| --------------------------- | ------------ | ------------ | ------------- | ---------- |
| Logistic Regression         | 84.62        | 83.00        | 82.00         | 85.00      |
| K-Nearest Neighbors         | 89.41        | 97.04        | 96.38         | 97.70      |
| Decision Tree               | 91.63        | 99.12        | 99.03         | 99.20      |
| Random Forest               | 93.37        | 99.39        | 99.55         | 99.23      |
| XGBoost                     | 93.26        | 99.51        | 99.49         | 99.52      |
| LightGBM                    | 93.43        | 99.51        | 99.49         | 99.52      |
| AdaBoost                    | 86.30        | 86.00        | 82.00         | 85.00      |
| **Logit (Hybrid Ensemble)** | **93.44**    | **99.72**    | **99.60**     | **99.85**  |


 Hybrid Ensemble (Logit) performed the best overall, showing strong capability in identifying churn-prone customers.

# Technologies Used:
Python
NumPy, Pandas
Scikit-learn
XGBoost
LightGBM
Matplotlib / Seaborn 
Jupyter Notebook

# Conclusion
This project demonstrates the importance of preprocessing and model comparison in churn prediction. Ensemble models—especially the Hybrid Logit model—outperform individual models and provide superior predictive accuracy.

The workflow ensures:
No data leakage
Consistent reproducibility
Strong model generalization

The results show that advanced ensemble techniques can significantly enhance churn prediction accuracy.


