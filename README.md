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

These results indicate moderate discriminative ability consistent with baseline clinical risk models such as logistic regression-based cardiovascular risk scores.

---

## Feature Importance (Odds Ratios)

The logistic regression coefficients were exponentiated to compute odds ratios, allowing clinical interpretability.

Key findings:
- Age and systolic blood pressure show the strongest positive association with CHD risk
- Smoking status is a significant behavioral risk factor
- Cholesterol contributes moderately to risk prediction

---

## Interpretation
The model shows moderate predictive performance consistent with baseline clinical risk models. Results highlight the importance of traditional cardiovascular risk factors.

---

## Clinical Relevance

This project demonstrates how classical statistical learning models can support interpretable clinical decision-making. Unlike black-box models, logistic regression provides transparent risk factors that align with established cardiovascular epidemiology.

---

## Limitations
- Logistic regression assumes linear relationships between features and log-odds
- Dataset is moderately imbalanced (low CHD incidence)
- No external validation cohort
- No temporal modeling of longitudinal risk changes

---

## Future Work
- LASSO regression for feature selection
- Calibration curves for clinical probability accuracy
- Gradient boosting models for comparison

---

## Author
Jenna Lu
University of Florida — Statistics
