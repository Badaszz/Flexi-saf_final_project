# FlexiSAF Final Project

## Overview
This repository contains the final project for the FlexiSAF internship program.  
The goal was to demonstrate the application of both **supervised** and **unsupervised** machine learning techniques to solve real-world problems.

- **Supervised Learning**: Microsoft Malware Classification – predicting malware family classes.
- **Unsupervised Learning**: Customer segmentation on the Online Retail II dataset.

---

## Supervised Learning

### Dataset
Microsoft Malware Classification dataset from Kaggle.

### Objective
Predict the malware class based on extracted features.

### Methodology
- Loaded and preprocessed the dataset.
- Separated features and target (`Class`).
- Split data into training and testing sets using stratified sampling.
- Standardized features using `StandardScaler`.
- Trained a **Random Forest Classifier** as a baseline.
- Tuned hyperparameters using **GridSearchCV**.
- Evaluated model using **classification report**, **confusion matrix**, and **log loss**.

---

## Unsupervised Learning

### Dataset
Online Retail II dataset from Kaggle.

### Objective
Segment customers into groups based on their purchasing behavior.

### Methodology
- Removed cancelled transactions and missing customer IDs.
- Converted invoice dates to datetime format.
- Engineered **Recency, Frequency, and Monetary (RFM)** features.
- Standardized features.
- Applied **K-Means clustering**.
- Evaluated clusters using **Silhouette Score** and **Davies–Bouldin Index**.
- Visualized clusters in **2D and 3D** using PCA and Plotly.
