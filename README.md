# Heart Disease Prediction Using Machine Learning

## Project Overview

This project uses machine learning to predict whether a patient is likely to have heart disease based on clinical features.

Two classification algorithms were implemented and compared:

- Logistic Regression
- Decision Tree

The models were evaluated using accuracy, precision, recall, confusion matrices, and ROC-AUC analysis.

> **Note:** This project is for educational purposes only and is not a medical diagnostic system.

## Dataset

The project uses the **UCI Heart Disease dataset**.

- Number of instances: 303
- Number of features: 13
- Target variable: Heart disease presence

The original target contains multiple values. For this project, it was converted into a binary classification:

- `0` → No heart disease
- `1` → Heart disease present

## Features

The dataset contains the following features:

- Age
- Sex
- Chest pain type
- Resting blood pressure
- Cholesterol
- Fasting blood sugar
- Resting ECG
- Maximum heart rate
- Exercise-induced angina
- ST depression
- Slope
- Number of major vessels
- Thalassemia

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- UCI ML Repository

## Machine Learning Workflow

1. Load the Heart Disease dataset
2. Inspect the dataset
3. Check for missing values
4. Convert the target into binary classification
5. Split the dataset into training and testing sets
6. Handle missing values using median imputation
7. Scale features for Logistic Regression
8. Train Logistic Regression
9. Train Decision Tree
10. Evaluate both models
11. Compare model performance
12. Generate confusion matrices
13. Generate ROC curves and calculate AUC

## Model Performance

### Logistic Regression

| Metric | Score |
|---|---:|
| Accuracy | 86.89% |
| Precision | 81.25% |
| Recall | 92.86% |
| F1-score | 0.87 |

### Decision Tree

| Metric | Score |
|---|---:|
| Accuracy | 78.69% |
| Precision | 74.19% |
| Recall | 82.14% |
| F1-score | 0.78 |

## Results

Logistic Regression performed better than the Decision Tree on the test split.

It achieved:

- Higher accuracy
- Higher precision
- Higher recall
- Higher F1-score

The ROC curve and AUC analysis were also used to compare the classification performance of both models.

## Project Structure

```text
Heart-Disease-Prediction/
│
├── Heart_Disease_Prediction.ipynb
├── README.md
└── requirements.txt
