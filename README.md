# 🏥 Healthcare Appointment No-Show Prediction Dashboard

[![Python](https://img.shields.io/badge/Python-3.9+-blue?logo=python)](https://www.python.org/)
[![Power BI](https://img.shields.io/badge/Power--BI-Dashboard-yellow?logo=powerbi)](https://powerbi.microsoft.com/)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

---

## 🚀 Project Overview

**Predict and reduce missed medical appointments (no-shows) using Python machine learning and Power BI dashboards!**  
This project takes you step-by-step from raw clinical data ➡️ automated cleaning ➡️ feature engineering ➡️ predictive modeling ➡️ interactive reporting.

---

## 📂 Table of Contents

- [Features](#features)
- [Dataset](#dataset)
- [Project Workflow](#project-workflow)
- [Python Pipeline](#python-pipeline)
- [Power BI Dashboard](#power-bi-dashboard)
- [Key Insights](#key-insights)
- [How to Use](#how-to-use)
- [Contribution](#contribution)

---

## ✨ Features

- ⚙️ **Automated Data Cleaning & Preprocessing**
- 🏷️ **Feature Engineering**: Age groups, time gaps, same-day flags
- 🤖 **ML Models**: Decision Tree, Random Forest, Gradient Boosting (with class balancing)
- 🔎 **Model Evaluation**: Confusion Matrix, ROC AUC, precision/recall
- 📈 **Power BI Dashboard**: KPIs, demographic slicers, confusion matrix, operational breakdowns
- 📤 **CSV Export**: Ready for business reporting or further analytics

---

## 🗂️ Dataset

- Patient demographics (Age, Gender, Scholarship)
- Medical history (Hypertension, Diabetes, Alcoholism, Handicap)
- Appointment meta-data (Days to appointment, Same-day booking, SMS reminders)
- Target: **No-show** (Yes/No)

---

## 🔄 Project Workflow



graph TD
A[📄 Raw Data] --> B[🔬 Clean & Explore]
B --> C[🛠️ Feature Engineering]
C --> D[🧠 Model Training]
D --> E[📊 Power BI Dashboard]



---

## 🐍 Python Pipeline

1. **Data Cleaning**
   - `pandas` for handling nulls, duplicates, type conversion.
2. **Exploratory Data Analysis**
   - `matplotlib` / `seaborn` for visualizations (age, gender, SMS, weekday trends)
3. **Feature Engineering**
   - Computes age groups, time gaps, flags for same-day booking.
4. **Modeling**
   - Train/test split using `stratify` for balance.
   - Tried `DecisionTreeClassifier`, `RandomForestClassifier`, and `GradientBoostingClassifier` (best).
   - Used `class_weight='balanced'` for all trees.
5. **Model Evaluation**
   - Calls `classification_report`, confusion matrix, and ROC/AUC
6. **Probability Threshold Optimization**
   - Custom `predict_proba` threshold for fairer no-show detection!
7. **Export for Power BI**
   - Outputs test set with `Actual_NoShow`, `Predicted_NoShow`, and probability scores.

---

## 📊 Power BI Dashboard

- 🟢 **KPI Cards**: Total appointments, no-show %, target, same-day, SMS
- 📊 **Confusion Matrix**: Actual vs predicted no-shows (visual and table)
- 📇 **Demographic/Operational Slicers**: Age, days to appointment
- 📉 **Rate by Age/Gender**: Pinpoints high-risk groups
- 📈 **SMS Timing Line**: When reminders are sent (and if they matter!)
- 🧮 **Calibrated Probabilities Table**: How risk scores match up to real attendance

---

## 🔍 Key Insights

- **20% no-show rate**: Major impact on efficiency and patient care
- **Same-day bookings & youth**: Highest risk, need targeted outreach
- **Model captures both obvious and subtle patterns** (recall improved via thresholding)
- **Dashboard fuels both strategic and operational conversations with real-time KPIs**

---

## 🛠️ How to Use

1. 🐍 **Run `model_pipeline.py` or Jupyter notebook for cleaning, modeling, and export**
2. ⬆️ **Import the result CSV into Power BI**
3. 🖱️ **Explore, filter, and learn directly from the interactive dashboard**
4. 📈 **Share witih stakeholders, iterate on interventions, and improve over time**

---

## 🤝 Contribution

Fork, star ⭐, or submit a PR to improve model, visuals, or documentation! For issues, open a ticket or reach out.

---

## 📬 Contact

👤 Priyanshu Bagri
✉️ scholarpriyanshu@gmail.com  
🔗 https://capstonedata.my.canva.site/healthcare-dashboard

---

> Made with ❤️, Python, and Power BI for patient-centered impact!

