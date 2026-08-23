# Telecom Customer Churn Prediction

A machine learning project that predicts which telecom customers are likely to churn, enabling proactive retention strategies.

## 📋 Overview

This project applies data preprocessing and classification modeling to a telecom customer dataset to identify customers at risk of canceling their subscription, before the company loses them.

## ✨ Features

- Data cleaning and preprocessing pipeline for raw customer data
- Applies SMOTE to the training data to account for class imbalance
- Feature engineering to improve model performance
- Multiple classification models trained and evaluated
- Performance comparison to select the best-performing model

## 🛠️ Tech Stack

- **Language:** Python
- **Libraries:** pandas, NumPy, scikit-learn, matplotlib

## 🚀 How to Run Locally

```bash
# Clone the repository
git clone https://github.com/israel7970/telecom-churn-prediction.git
cd telecom-churn-prediction

# Install dependencies
pip install -r requirements.txt

# Run the notebook or script
jupyter notebook churn_prediction.ipynb
# or
python churn_prediction.py
```

## 📊 Results

After cleaning, encoding, scaling, and applying SMOTE to address class imbalance, a Logistic Regression model was trained and evaluated:

| Metric | Score |
|-----------|--------|
| Accuracy | 72.6% |
| Precision | 49.1% |
| Recall | 76.2% |
| F1 Score | 59.6% |

The model is stronger at **identifying customers likely to churn (high recall)** than at **avoiding false alerts (lower precision)** — it catches most at-risk customers, but also flags some who wouldn't have actually churned.

For a customer retention use case, this tradeoff is generally favorable: failing to catch a customer who churns is typically more costly than sending an unnecessary retention offer to one who wouldn't have. Recall was prioritized accordingly.

## 📸 Screenshots

<img width="1206" height="736" alt="image" src="https://github.com/user-attachments/assets/d42c685c-cf8e-43e2-b6d8-5f3ae586a245" />


## 📌 Notes

Built to practice the full ML workflow: data cleaning, feature engineering, model training, and evaluation on a real-world-style business problem.
