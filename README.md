# Credit Card Fraud Detection System

## Project Overview

The goal of this project is to detect fraudulent credit card transactions using machine learning techniques.  
Since fraudulent transactions are very rare compared to normal ones, the main challenge is handling highly imbalanced data.

This project focuses on building a reliable classification model by carefully preprocessing data and balancing the dataset.

---

## Dataset

- Total transactions: 284,807  
- Number of features: 30 (numerical)  
- Target column: Class  

Class labels:
- 0 → Normal transaction  
- 1 → Fraudulent transaction  

The dataset is highly imbalanced:
- Normal transactions: 284,315  
- Fraudulent transactions: 492  

All features (V1 to V28) are anonymized for security purposes.

---

## Data Exploration and Preprocessing

- Checked dataset shape, data types, and missing values  
- No missing values were found  
- Analyzed class distribution to understand imbalance  
- Compared transaction amount statistics for normal and fraudulent transactions  

---

## Handling Imbalanced Data

To handle class imbalance, under-sampling was applied:

- Randomly selected 492 normal transactions  
- Combined them with all 492 fraudulent transactions  
- Created a balanced dataset with equal class distribution  

This approach helps the model learn patterns from both classes effectively.

---

## Feature and Target Selection

- Features (X): All columns except Class  
- Target (Y): Class  

The dataset was split into:
- Training set: 80%  
- Testing set: 20%  

Stratified sampling was used to preserve class balance.

---

## Model Used

Logistic Regression was used for binary classification due to its simplicity and effectiveness.

- Model trained on the balanced dataset  
- No complex hyperparameter tuning was applied  

---

## Model Performance

Accuracy was used as the evaluation metric:

- Training accuracy: ~94.15%  
- Testing accuracy: ~93.90%  

The similar performance on training and testing data indicates good generalization and minimal overfitting.

---

## Key Learnings

- Handling imbalanced datasets is critical in fraud detection problems  
- Data preprocessing plays a major role in model performance  
- Logistic Regression can perform well when data is properly prepared  
- Real-world financial data requires careful analysis before modeling  

---

## Technologies Used

- Python  
- NumPy  
- Pandas  
- Scikit-learn  
- Google Colab  

---

## Project Link

Open the notebook in Google Colab:  
https://colab.research.google.com/github/mohitsaini65/-Credit-Card-Fraud-Detection-System

