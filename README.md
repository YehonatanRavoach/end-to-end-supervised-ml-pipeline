# End-to-End Supervised Machine Learning Pipeline

This project demonstrates a complete **supervised machine learning workflow** for a regression task on structured tabular data, implemented using **scikit-learn**.

The emphasis is on **correct ML methodology** rather than model complexity: Exploratory Data Analysis (EDA), preprocessing, model training, comparison, and evaluation with strict train/test separation to prevent data leakage.

---

## Project Overview

The objective is to predict a continuous target variable from a housing dataset using supervised learning techniques.

The notebook walks through a production-oriented ML flow:
- Data understanding via EDA
- Feature preprocessing and scaling
- Training and comparison of multiple regression models
- Evaluation on an unseen test set with appropriate metrics

This mirrors how real-world ML pipelines are designed and validated.

---

## Dataset

- Tabular housing dataset
- Separate CSV files for training and testing
- Numerical features
- Regression problem

---

## Methodology

### 1. Exploratory Data Analysis (EDA)
- Inspected feature distributions
- Analyzed correlations between variables
- Identified preprocessing requirements (e.g., scaling)

### 2. Preprocessing
- Applied feature scaling where appropriate
- Maintained clean separation between training and test data
- Avoided data leakage throughout the pipeline

### 3. Modeling
- Trained and compared multiple regression models using scikit-learn
- Evaluated trade-offs between performance, complexity, and efficiency

### 4. Evaluation
- Assessed final models on a held-out test set
- Focused on generalization rather than training performance

---

## Model Selection Summary

- **KNN** performed well on preprocessed data during training but showed weaker generalization at prediction time.
- **Linear Regression** provided more stable and consistent prediction performance and was selected as the final model.

Although **Random Forest** achieved the highest overall score (≈ **0.83**) without requiring preprocessing, it was not selected due to higher computational and resource requirements.

**Final decision rationale:**
- Faster and more predictable inference
- Lower computational and memory cost
- Higher interpretability and simpler deployment

**Key insight:** Proper data calibration and preprocessing had a greater impact on performance than increasing model complexity.

---

## Project Structure
```
ML-Flow-Project/
├── Assignment2_supervised_learning_flow.ipynb
├── housing_train.csv
├── housing_test.csv
└── README.md
```

---

## Technologies & Skills Demonstrated
- Python
- scikit-learn
- Supervised learning (regression)
- Exploratory Data Analysis (EDA)
- Feature scaling & preprocessing
- Model evaluation
- Reproducible ML workflow
