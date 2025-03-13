# Mental-health-analytics
# Detecting Depression in University Students 🧠📊

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![License](https://img.shields.io/badge/License-MIT-green)
![ML](https://img.shields.io/badge/Machine%20Learning-Classification-orange)

A machine learning project to classify and predict depression in university students using psychological, academic, and lifestyle features.

---

## Table of Contents
- [Overview](#overview)
- [Dataset](#dataset)
- [Methodology](#methodology)
- [Installation](#installation)
- [Usage](#usage)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)
- [Acknowledgments](#acknowledgments)

---

## Overview 🔍

This project aims to identify university students at risk of depression using a classification model trained on demographic, academic, and lifestyle data. It serves as a **proof-of-concept tool** for educational institutions to prioritize mental health interventions.

**Key Features**:
- Preprocessing pipelines for handling categorical/numerical data.
- Comparison of Logistic Regression, Random Forest, and XGBoost models.
- Feature importance analysis to identify depression predictors.
- Ethical considerations for real-world deployment.

---

## Dataset 📂

The dataset contains anonymized student records with features like GPA, sleep patterns, social engagement, and academic stress. 

**Source**: [Depression Dataset](https://raw.githubusercontent.com/bilal265/Mental-health-analytics/refs/heads/main/Depression%20Dataset.csv)  
**Features**:
- `Gender`, `Age`, `Major` (demographic)
- `GPA`, `Academic_Stress` (academic)
- `Sleep_Duration`, `Social_Engagement` (lifestyle)
- `Depression` (target: binary classification)

---

## Methodology 🛠️

### Workflow
1. **Preprocessing**  
   - Handle missing values and encode categorical variables.
   - Convert ordinal data (e.g., `Sleep_Duration` ranges) to numerical values.
   - Normalize features using `StandardScaler`.

2. **Exploratory Data Analysis (EDA)**  
   - Visualize correlations between features and depression status.
   - Analyze distributions (e.g., sleep hours vs. depression).

3. **Model Building**  
   - Train and evaluate:
     - Logistic Regression (baseline)
     - Random Forest (feature importance)
     - XGBoost (optimized performance)
   - Hyperparameter tuning with `GridSearchCV`.

4. **Evaluation**  
   - Metrics: Recall, AUC-ROC, F1-score.
   - Confusion matrices and ROC curves.

---

## Installation 💻

1. Clone the repository:
   ```bash
   git clone https://github.com/bilal265/depression-detection.git
   cd depression-detection

2. Install dependencies:
  ```bash
  pip install pandas numpy scikit-learn xgboost matplotlib seaborn
    
