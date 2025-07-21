
# 🛒 Online Shoppers Purchasing Intention – ML & Tableau Dashboard

This project aims to predict whether a visitor will generate revenue (i.e., make a purchase) on an e-commerce website, using machine learning techniques, and visualize the insights through Tableau dashboards.


## 📊 Dataset

- **Source**: [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/online+shoppers+purchasing+intention+dataset)
- **Description**: This dataset contains information about online sessions on a retail website. It includes page types visited, session duration, bounce rates, etc.

---

## 🧠 Objective

To build a classification model that predicts whether a session will result in **revenue (purchase)** based on user behavior data.

---

## 🧹 Steps Performed

### 1. **Data Preprocessing**
- Converted categorical columns (e.g., `Month`, `VisitorType`) using One-Hot Encoding
- Scaled continuous features
- Handled class imbalance using `class_weight='balanced'`

### 2. **Modeling**
- **Model Used**: `RandomForestClassifier`
- Evaluation Metrics:
  - **Accuracy**: ~90%
  - **F1-Score (Class 1)**: ~60%
  - **ROC AUC**: ~0.91

### 3. **Prediction Output**
- Predicted labels (`Predicted Revenue`)
- Associated probabilities (`Revenue Probability`)
- Exported the final dataset for Tableau visualization

---

## 📉 Tableau Dashboard

The `predictions_for_tableau.csv` was imported into Tableau Public to build a dashboard with the following insights:
- Revenue prediction count (0 vs. 1)
- Revenue probability distribution
- Key user behaviors (like bounce rate, time spent, etc.) vs. predicted revenue

🖼️ *Dashboard Screenshot available in `/images` folder*

---

## 🚀 How to Run

### ✅ Model Notebook
1. Open `revenue_prediction.ipynb`
2. Run all cells – it will load data, train the model, and export the prediction CSV

### 📈 Tableau
1. Open Tableau Desktop/Public
2. Load `predictions_for_tableau.csv`
3. Use fields like `Predicted Revenue`, `Revenue Probability`, and session features to explore patterns

---

## 🧰 Tools & Libraries

- Python (Pandas, Scikit-learn, Matplotlib)
- Jupyter Notebook
- Tableau Public

---

## 📌 Key Learnings

- Handling imbalanced classification problems
- Interpreting model performance using classification report & ROC AUC
- Exporting model outputs for business visualization
- Creating actionable dashboards in Tableau

---

## 📎 Author

Aadersh Ramesh
Master’s in Data Analytics  
GitHub: Aadersh3569
LinkedIn:www.linkedin.com/in/aadersh356

