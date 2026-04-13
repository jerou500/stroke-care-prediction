# Stroke Care Quality Prediction — NHS Data

**Student:** Jerald John Bosco  
**Module:** 7150CEM — Data Science Project  
**Institution:** Coventry University, 2025/26  
**Ethics Reference:** P192998 (Low Risk, approved 23 Feb 2026)

## Overview

This project applies machine learning to predict whether an NHS Primary Care Trust (PCT) is at risk of poor stroke care quality using publicly available NHS England IPMR Stroke data (Q1-Q4, 2012-13).

## Models

- Logistic Regression
- Random Forest
- XGBoost + SHAP interpretability

## Results

| Model | Test AUC | CV AUC |
|-------|----------|--------|
| Logistic Regression | 0.7805 | 0.7726 |
| Random Forest | 0.7698 | 0.7036 |
| XGBoost | 0.7921 | 0.8012 |

## Data

Download the 4 quarterly .xls files from NHS England and place in a data/raw/ folder.
Source: https://www.england.nhs.uk/statistics/statistical-work-areas/stroke-care/

## Setup

```bash
pip install pandas numpy==1.26.4 matplotlib seaborn scikit-learn xgboost shap openpyxl xlrd==1.2.0 jupyter
```

## Run

Open stroke_care_prediction.ipynb in Jupyter and run all cells.

## Ethics

All data is fully anonymised at organisational level. No patient records accessed. Ethics approval: P192998, Coventry University, 23 Feb 2026, Low Risk.
