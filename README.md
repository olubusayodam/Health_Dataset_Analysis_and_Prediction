# Health Dataset Analysis and Prediction

## Introduction
This project delves into the analysis of a comprehensive health dataset to uncover insights into the factors influencing heart disease. The initial dataset consisted of 319,834 rows and 18 columns. The analysis encompasses exploratory data analysis (EDA), data cleaning, preprocessing, and model training.

## Exploratory Data Analysis (EDA)

### Dataset Overview:
The dataset comprises a mix of numerical and categorical variables. Initial examination revealed BMI, PhysicalHealth, MentalHealth, and SleepTime as numerical, while others are categorical. Class imbalance was observed, particularly in the target variable (HeartDisease).

### Data Distribution and Outliers:
Numerical data exhibited non-normalized distributions. Outliers were discerned using boxplots, with PhysicalHealth and MentalHealth showing a significant number.

### Several issues were identified:
1. Non-normalized distribution
2. Presence of outliers, particularly in PhysicalHealth and MentalHealth
3. Disparate treatment of categorical and numerical variables
4. Class imbalance in the target variable (HeartDisease)
5. Presence of missing values
6. Identification and removal of duplicate values

## Data Cleaning

### Duplicate Removal:
18,114 duplicate values were identified and removed.

### Missing Values:
Rows with missing values were discarded, resulting in 301,684 rows.

### Outlier Treatment:
Addressed outliers in BMI, PhysicalHealth, MentalHealth, and SleepTime using various methods, including log transformation.

## Data Preprocessing and Transformation:

### Categorical Labels:
Categorical labels were categorized as ordinal (AgeCategory and GenHealth) and nominal (other categorical variables).

### Encoding:
Ordinal encoding was applied to GenHealth and AgeCategory. Nominal variables underwent one-hot encoding.

### Feature Selection:
Recursive Feature Elimination (RFE) was utilized to pinpoint the most influential features for predicting heart disease. The top 5 features identified were:
- Stroke_No
- Race_Asian
- Diabetic_No
- Diabetic_Yes (during pregnancy)
- KidneyDisease_No

## Model Training and Testing:
The dataset was bifurcated into training and testing sets. A machine learning model was trained using the top 5 features, and the model's performance was subsequently evaluated.

## Conclusion:
This analysis unearthed crucial insights into the health dataset, effectively addressing issues such as outliers, missing values, and class imbalance. The trained model, utilizing selected features, lays a robust foundation for predicting heart disease. Further refinement and exploration are recommended for a more exhaustive understanding.
