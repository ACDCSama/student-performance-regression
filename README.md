# 🎓 Student Performance Prediction

This project builds regression models to predict students' academic test scores based on their demographics and preparation levels. The dataset includes math, reading, and writing scores, and the goal is to train models that can accurately predict these scores using various features.

## 📂 Dataset

- **Source**: [Kaggle - Students Performance Data](https://www.kaggle.com/datasets/spscientist/students-performance-in-exams)
- **Format**: CSV, 1000 samples × 8 columns
- **Features**:
  - Categorical: `gender`, `race/ethnicity`, `parental level of education`, `lunch`, `test preparation course`
  - Numerical: `math score`, `reading score`, `writing score`

## 🎯 Objective

To predict each of the three test scores (math, reading, writing) using:
- Linear Regression (baseline model)
- Random Forest Regression (ensemble model)

## 🧠 Models Used

- **Linear Regression**: Simple interpretable model for baseline performance.
- **Random Forest Regression**: Ensemble tree-based model to capture non-linear patterns.

## 📊 Evaluation Results

| Target Score     | Model              | MAE   | MSE    | R² Score |
|------------------|--------------------|-------|--------|----------|
| Math Score       | Linear Regression  | 4.21  | 29.10  | 0.880    |
|                  | Random Forest      | 4.71  | 36.48  | 0.850    |
| Reading Score    | Linear Regression  | 3.49  | 18.57  | 0.918    |
|                  | Random Forest      | 3.72  | 20.56  | 0.909    |
| Writing Score    | Linear Regression  | 3.20  | 14.91  | 0.938    |
|                  | Random Forest      | 3.69  | 20.53  | 0.915    |

> ✅ The **Linear Regression model** achieved the best performance when predicting **writing score** (R² = 0.938).

## 🔍 Exploratory Data Analysis (EDA)

Key insights include:
- Students who completed a test preparation course performed better.
- Higher parental education levels are generally associated with better scores.
- Reading and writing scores are highly correlated.
- Gender and lunch type had moderate effects on performance.

Visualization tools used:
- Histograms, boxplots, heatmaps, pairplots
- Libraries: `seaborn`, `matplotlib`



