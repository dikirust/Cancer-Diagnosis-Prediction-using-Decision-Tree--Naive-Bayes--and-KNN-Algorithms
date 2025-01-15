# Cancer Diagnosis Prediction using Decision Tree, Naïve Bayes, and KNN

## Description

This repository contains an individual data mining project aimed at predicting the type of cancer (Malignant or Benign) using machine learning algorithms. The dataset used for the project is the Breast Cancer Data Set from Kaggle, which includes features such as tumor radius, texture, perimeter, and area to aid in diagnosis.

Algorithms used:

- Decision Tree
- Naïve Bayes
- K-Nearest Neighbors (KNN)

The models are trained and evaluated to predict cancer diagnosis based on visual characteristics of the tumors.

## Dataset

- The dataset consists of 569 rows and 30 features, including patient ID, cancer diagnosis, and tumor characteristics.
- The features used for prediction include `radius_mean`, `texture_mean`, `perimeter_mean`, `area_mean`, `smoothness_mean`, and more.
- The target variable is the `diagnosis`, which indicates whether the tumor is Malignant (M) or Benign (B).

Dataset Source: [Kaggle - Cancer Data](https://www.kaggle.com/datasets/erdemtaha/cancer-data)

## Features

- **id**: Unique patient ID (treated as a meta-variable and excluded from prediction)
- **diagnosis**: Cancer diagnosis (Malignant "M" or Benign "B")
- **radius_mean, texture_mean, perimeter_mean, area_mean**: Visual characteristics of the tumor.

## Workflow

![Workflow](https://github.com/dikirust/Cancer-Diagnosis-Prediction-using-Decision-Tree--Naive-Bayes--and-KNN-Algorithms/blob/main/knn%20nb%20dt%20ornge.png?raw=true)

1. **Data Preprocessing**:
   - The `id` variable is excluded as it does not impact the diagnosis.
   - Missing data check is performed, ensuring no missing values in the dataset.
2. **Feature Ranking**:

   - The correlation between features and target is evaluated using a ranking widget, revealing that `radius_worst`, `perimeter_worst`, and `area_worst` are most influential.

3. **Model Training and Evaluation**:
   - Three machine learning models are used to train the dataset:
     - **Decision Tree**
     - **Naïve Bayes**
     - **K-Nearest Neighbors (KNN)**
   - Evaluation metrics (using cross-validation with 20 folds):
     - **Decision Tree**:
       - AUC: 0.919
       - Accuracy: 92.6%
       - F1 Score: 92.6%
       - Precision: 92.6%
       - Recall: 92.6%
4. **Results**:
   - The Decision Tree model performed well with consistent results across metrics.
