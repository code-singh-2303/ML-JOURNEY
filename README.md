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
