# 📧 Email Marketing Campaign – Click Prediction Case Study

## 🚀 Overview

This case study focuses on optimizing an email marketing campaign using machine learning. The objective is to predict which users are likely to click on a link in the email, enabling the marketing team to send targeted emails and improve the overall Click-Through Rate (CTR).

---

## 🧠 Problem Statement

The marketing team of an e-commerce platform sent emails to users about a new feature. The goal is:
- Analyze open and click behavior.
- Build a predictive model to target users likely to click.
- Simulate improved CTR using the model’s predictions.

---

## 📊 Data Description

There are 3 datasets:

1. `email_table.csv` – details of each sent email.
2. `email_opened_table.csv` – email IDs that were opened.
3. `link_clicked_table.csv` – email IDs where the internal link was clicked.

---

## 🛠️ Tech Stack

- Python (Jupyter / Colab)
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn
- XGBoost, CatBoost
- Imbalanced-learn (`SMOTE`)
- Category Encoders (`TargetEncoder`)

---

## 🧪 Model Development

We explored various models:
- Logistic Regression
- Gaussian Naive Bayes
- XGBoost ✅
- CatBoost ✅

XGBoost and CatBoost gave the best results, especially in detecting rare click events with higher precision and recall.

---

## 📈 CTR Optimization Strategy

We used the trained model to score users by their likelihood to click. The approach:

- Predict click probabilities for all users.
- Target top 5,000 users with the highest predicted probabilities.
- Calculate CTR improvement in this segment.

**📌 Baseline CTR (Random):** ~2.1%  
**📌 CTR in Top 5,000 Scored Users:** ~8.38%

🎯 **Result:** ~4x improvement in CTR by leveraging model-based targeting.

---

## 📘 How to Run

1. Clone the repo:
```bash
git clone https://github.com/your-username/email-campaign-case-study.git
```

2. Install dependencies:
```bash
pip install -r requirements.txt
```

3. Launch the notebook: Open notebooks/email_campaign_analysis.ipynb in Jupyter or Google Colab:





Refer to report to understand :
```bash
Business understanding
EDA insights
Feature engineering
Model building
CTR simulation and results
Strategic recommendations
```
