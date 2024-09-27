# Churn Analysis Using Machine Learning

## Overview

The objective of this project is to predict customer churn for a subscription-based service using various machine learning models. Churn prediction helps businesses identify customers at risk of leaving, allowing them to take action to retain these customers. This project walks through the process of data preprocessing, model training, evaluation, and comparison across multiple algorithms.

The project involves:
- Data loading, exploration, and preprocessing
- Feature engineering for better model performance
- Training machine learning models
- Evaluating model performance using various metrics
- Handling imbalanced data using **SMOTE**
- Interpreting key features influencing churn

## Dataset

This project uses a customer churn dataset with features such as:
- **AccountAge**: The number of months the customer has been with the service.
- **MonthlyCharges**: The monthly fee paid by the customer.
- **SubscriptionType**: Subscription tier selected by the customer (e.g., Basic, Premium).
- **PaymentMethod**: Method used for payment (e.g., Credit Card, Electronic Check).
- **WatchlistSize**: The number of items in the customer’s watchlist.
- **Churn**: The target variable, where 1 indicates the customer churned, and 0 indicates they stayed.

## Handling Imbalanced Data with SMOTE

In churn prediction, it is common for the dataset to be imbalanced, with fewer customers churning (1) compared to those who do not churn (0). To address this, we used **SMOTE (Synthetic Minority Over-sampling Technique)** to artificially increase the number of churn cases by generating synthetic samples. This helps balance the dataset and ensures that machine learning models do not become biased towards the majority class (non-churn).

SMOTE works by:
- Creating new synthetic data points for the minority class (churn cases).
- Ensuring that models have more balanced data to learn from, improving classification performance.

## Models and Performance

The following machine learning models are trained and evaluated in this project:

1. **Machine Learning Models:**
   - Decision Tree
   - Random Forest
   - LightGBM

Each model is evaluated based on the following metrics:
- **Accuracy**: The overall correctness of the model's predictions.
- **Precision**: The proportion of positive predictions that are actually correct.
- **Recall**: The proportion of actual positives that are correctly identified.
- **F1-Score**: The harmonic mean of precision and recall.
- **AU-ROC Curve**: AUC score that helps understand the tradeoff between sensitivity and specificity.

## Results

The notebook provides a detailed comparison of all models. After applying **SMOTE**, the **Random Forest** and **LightGBM** models perform the best, achieving accuracy scores as high as **85%**. Key features influencing churn are identified, such as account age, monthly charges, and the subscription type.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

## Contact

For any questions or inquiries, feel free to reach out to:
- **Ariharasudhan A** - [Email](mailto:ariadaikalam1234@gmail.com)
