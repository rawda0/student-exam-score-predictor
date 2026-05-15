# 🎓 Student Performance Factors — ML Regression Project

Predicting student exam scores using machine learning based on various academic, social, and personal factors.

---

## 📌 Project Overview

This project builds a regression model to predict **Exam Scores** from 19 features covering study habits, parental involvement, access to resources, and more.

The dataset contains **~6,600 student records** with features like hours studied, attendance, sleep hours, tutoring sessions, family income, school type, and others.

---

## 📁 Repository Structure

```
├── Final_Project.ipynb               # Main notebook (EDA + modeling)
├── StudentPerformanceFactors.csv     # Dataset
├── ML_Project_Template.docx         # Project documentation
├── Project_Proposal_Form.docx        # Original project proposal
├── Student_Performance_Factors.pptx  # Presentation slides
├── requirements.txt                  # Python dependencies
└── README.md                         # This file
```

---

## 🔍 Dataset

| Property | Value |
|----------|-------|
| Source | StudentPerformanceFactors.csv |
| Rows | ~6,607 |
| Features | 19 (numerical + categorical) |
| Target | `Exam_Score` (continuous) |

**Key Features:** `Hours_Studied`, `Attendance`, `Previous_Scores`, `Sleep_Hours`, `Tutoring_Sessions`, `Parental_Involvement`, `Access_to_Resources`, `Motivation_Level`, `Family_Income`, and more.

---

## ⚙️ Methodology

1. **Data Cleaning** — Handling missing values (mode imputation for `Parental_Education_Level`, `Distance_from_Home`, `Teacher_Quality`)
2. **EDA** — Distribution analysis, correlation heatmap, outlier detection via IQR
3. **Feature Engineering** — One-hot encoding for categorical variables
4. **Feature Selection** — Top features by correlation with target
5. **Modeling** — SVR (RBF kernel) with GridSearchCV hyperparameter tuning
6. **Evaluation** — MSE, RMSE, MAE on test set

---

## 📊 Model Performance

| Model | RMSE | MAE |
|-------|------|-----|
| SVR (baseline) | — | — |
| SVR (tuned) | *run notebook to see* | *run notebook to see* |

---

## 🚀 How to Run

```bash
# 1. Clone the repo
git clone https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git
cd YOUR_REPO_NAME

# 2. Install dependencies
pip install -r requirements.txt

# 3. Open the notebook
jupyter notebook Final_Project.ipynb
```

> ⚠️ Make sure `StudentPerformanceFactors.csv` is in the **same folder** as the notebook before running.

---

## 🛠️ Technologies Used

- Python 3.x
- pandas, numpy
- scikit-learn (SVR, GridSearchCV, Pipeline)
- matplotlib, seaborn
- Jupyter Notebook

---

## 👤 Author

*Add your name here*

---
