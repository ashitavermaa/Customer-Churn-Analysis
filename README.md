# Telecom Churn Prediction Model

## Project Overview
This project focuses on predicting customer churn for a telecom company using machine learning models. The dataset consists of information from 7,043 telecom customers across 21 columns. The primary objective is to accurately predict whether a customer will churn, which is critical for the company to retain its customer base.

## Data Overview
The dataset is highly imbalanced, with the following distribution of the target variable, Churn:
- **No:** 73.46%
- **Yes:** 26.54%

This imbalance poses a significant challenge as it can lead to biased models that favor the majority class. The imbalance ratio is approximately 73:27.

## Models Used
We implemented the following models to predict churn:
1. **Decision Tree Classifier**
2. **Random Forest Classifier**
3. **Principal Component Analysis (PCA)**

## Handling Data Imbalance
Due to the significant imbalance in the dataset, the initial models struggled to deliver accurate predictions. To address this, we employed the SMOTE-ENN (Synthetic Minority Over-sampling Technique combined with Edited Nearest Neighbors) technique to balance the dataset. This approach helped in improving the model's ability to correctly identify churned customers.

## Model Performance
After balancing the data, the models showed significant improvement in performance. The **Random Forest Classifier** emerged as the best-performing model, achieving an accuracy of **94.03%**. On the other hand, the application of PCA did not enhance the model's performance, indicating that dimensionality reduction was not beneficial for this specific dataset.

## Conclusion
In conclusion, the Random Forest Classifier proved to be the most effective model for predicting telecom customer churn, especially after addressing the data imbalance with SMOTE-ENN. The final model accuracy of **94.03%** demonstrates the robustness of the approach taken. This model can be a valuable tool for the telecom company in proactively identifying at-risk customers and implementing retention strategies.
