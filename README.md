# Credit Card Fraud Detection

## Overview

This project implements a machine learning pipeline to detect fraudulent credit card transactions. The model leverages transaction features—such as amount, time, and principal component analysis (PCA) transformed variables—to classify transactions as authentic or fraudulent. Addressing the challenge of severe class imbalance, the project applies advanced resampling and multiple classification algorithms to maximize fraud detection performance.

## Features

- **Exploratory Data Analysis (EDA):**  
  Detailed analysis of transaction data to understand feature distributions, correlations, and class imbalance.

- **Imbalanced Data Handling:**  
  Utilizes both undersampling and oversampling techniques (including SMOTE) to address the rarity of fraudulent transactions.

- **Feature Engineering & Scaling:**  
  Applies PCA-transformed features and modified min-max normalization for optimal model performance.

- **Modeling:**  
  Compares several classifiers:
  - Logistic Regression
  - K-Nearest Neighbors
  - Decision Tree
  - Support Vector Machine (linear kernel)
  - Naive Bayes
  - Random Forest
  - Linear Discriminant Analysis
  - Stochastic Gradient Descent
  - Ridge Classifier

- **Evaluation Metrics:**  
  Focuses on the $F_2$-score to prioritize recall (catching fraud) over precision, alongside accuracy, precision, recall, and ROC-AUC.

## Results

- The **Random Forest** classifier, trained on SMOTE-oversampled data, achieved the best test $F_2$-score of **0.880783**.
- This result demonstrates strong performance in identifying fraudulent transactions with minimal false negatives.

## Usage

1. **Clone the Repository**
   ```
   git clone https://github.com/Vcode2407/creditcard_prevention.git
   cd creditcard_prevention
   ```

2. **Install Dependencies**
   ```
   pip install -r requirements.txt
   ```

3. **Run the Code**
   - Follow the instructions in the main Python scripts or Jupyter notebooks to preprocess data, train models, and evaluate results.

4. **Customize**
   - Update data paths, parameters, or experiment with additional classifiers as needed.

---

**Author:** Vinay Kumar  
**License:** MIT License (c) 2025 Vinay Kumar

*This repository is a personalized adaptation of open-source work for educational and portfolio purposes.*
```
