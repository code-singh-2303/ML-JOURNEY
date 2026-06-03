# Heart Disease EDA

## Dataset
303 patients, 14 features, binary classification

## Target
1 = Heart Disease, 0 = No Disease
Note: original encoding was flipped, corrected during EDA

## Key Findings
1. Males have 55% disease rate vs 25% for females
2. Asymptomatic chest pain (cp=0) has highest disease rate (72%)
3. Older patients (55-65) more prone to disease
4. Removed 723 duplicate rows — significant data quality issue
5. Top features: exang, oldpeak, ca, cp, thalach, sex

## Features Selected for Model
exang, oldpeak, ca, cp, thalach, sex, age

## Tools Used
Python, Pandas, Seaborn, Matplotlib, NumPy

# Breast Cancer Classification

## Dataset
569 patients, 30 features, binary classification

## Target
0 = Malignant, 1 = Benign

## Models Compared
Logistic Regression → 97.37% accuracy, 2 missed cancers
Random Forest       → 96.49% accuracy, 3 missed cancers  
XGBoost             → 95.61% accuracy, 3 missed cancers

## Winner
Logistic Regression — simpler model won on clean linear data

## Key Finding
Simple models beat complex ones when data is clean and relationships are linear
Critical metric was FP (missed malignant) — LR had fewest at 2
