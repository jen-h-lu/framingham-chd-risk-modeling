# Disease Risk Prediction (Framingham Dataset)

## Overview
This project builds a machine learning model to predict 10-year coronary heart disease (CHD) risk using the Framingham Heart Study dataset.

The goal is to demonstrate interpretable clinical risk modeling using logistic regression.

---

## Dataset
- Source: Framingham Heart Study
- Samples: 4,240 patients
- Features: 15 clinical and demographic variables
- Target: TenYearCHD (binary outcome)

---

## Methodology
- Data preprocessing: median imputation, standardization
- Model: Logistic Regression
- Evaluation: ROC-AUC, Accuracy, Confusion Matrix

---

## Results

- ROC-AUC: ~0.70
- Accuracy: ~0.84 (affected by class imbalance)

### ROC Curve
![ROC Curve](figures/roc_curve.png)

### Confusion Matrix
![Confusion Matrix](figures/confusion_matrix.png)

---

## Feature Importance
Top predictors include:
- Age
- Systolic Blood Pressure
- Smoking status
- Cholesterol

(See `figures/feature_importance.csv`)

---

## Interpretation
The model shows moderate predictive performance consistent with baseline clinical risk models. Results highlight the importance of traditional cardiovascular risk factors.

---

## Limitations
- Linear model assumption
- Class imbalance
- No external validation dataset

---

## Future Work
- LASSO regression for feature selection
- Calibration curves for clinical probability accuracy
- Gradient boosting models for comparison

---

## Author
Jenna Lu
University of Florida — Statistics
