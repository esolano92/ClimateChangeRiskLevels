# 🌍 Climate Risk Classification with Machine Learning

This project uses historical global temperature data to classify cities into **Low**, **Moderate**, or **High Climate Risk** categories. We applied three machine learning models—**Logistic Regression**, **Support Vector Machine (SVM)**, and **Random Forest**—to analyze trends and predict risk levels based on long-term climate behavior.

---

## 📊 Project Overview

- **Dataset**: Subset from the Berkeley Earth Global Land Temperatures dataset  
- **Scope**: 3,448 cities worldwide, covering the years **1900–2012**
- **Goal**: Use machine learning to identify cities at risk due to rising temperatures
- **Focus**: Prioritize **recall** to avoid missing at-risk locations

---

## 🛠 Features Engineered

- Average temperature (`AvgTemp`)
- Maximum temperature (`MaxTemp`)
- Temperature standard deviation (`TempStdDev`)
- Temperature trend (`TempTrendPerYear`)
- Years until +1.5°C warming (`YearsUntil1.5C`)

---

## 🧠 Models Used

- **Logistic Regression** (with GridSearchCV)
- **Support Vector Machine** (RBF kernel with parameter tuning)
- **Random Forest** (tuned for depth, splits, and estimators)

Each model was evaluated using **recall**, **F1-score**, and **classification reports** on both training and testing sets.

---

## 📈 Results

- **Random Forest** achieved the best performance with near-perfect recall.
- **SVM** also performed strongly with minimal overfitting.
- **Logistic Regression** was interpretable but less effective for Moderate Risk.

> See `/figures` for all tuning plots and classification reports.

---



