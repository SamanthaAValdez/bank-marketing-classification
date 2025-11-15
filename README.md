# Bank Marketing Classification

This repository contains a Jupyter Notebook comparing **Logistic Regression** and **Decision Tree** on the Bank Marketing dataset from UCI.

---

## Project Overview

The project reproduces the study by Moro, Cortez, and Rita (2014), *A Data-Driven Approach to Predict the Success of Bank Telemarketing*, published in *Expert Systems with Applications*.  
The goal is to predict whether a bank client will subscribe to a term deposit after a marketing campaign using the classification algorithms taught in class.

---

## Dataset

- File: 'bank-full.csv'  
- Folder: 'data/'  
- Source: [UCI ML Repository](https://archive-beta.ics.uci.edu/dataset/222/bank%2Bmarketing?utm_source=chatgpt.com)  
- Description: Client and campaign features; target variable 'y' (1 = yes, 0 = no)  
- Notes: Dataset is imbalanced (~88% no, ~12% yes). A binary feature 'pdays_never' indicates clients never contacted.

---

## Notebook

- File: 'notebooks/BankMarketing_Classification_Samantha.ipynb'  
- Open directly in Google Colab: [Open in Colab]https://colab.research.google.com/github/SamanthaAValdez/bank-marketing-classification/blob/main/notebooks/BankMarketing_Classification_Samantha.ipynb

---

## Project Structure

- 'README.md' — This file with instructions and summary  
- 'data/bank-full.csv' — Dataset file  
- 'notebooks/BankMarketing_Classification_Samantha.ipynb' — Main notebook

---

## Methodology & Steps

1. **Data Cleaning & Preparation**  
   - Drop 'duration' column to avoid target leakage  
   - Encode target 'y' as 0/1  
   - Create 'pdays_never' feature  
   - Separate numerical and categorical features

2. **Preprocessing**  
   - One-hot encode categorical variables  
   - Standardize numerical variables

3. **Train-Test Split**  
   - 75% training, 25% testing  
   - Stratify by target variable

4. **Modeling**  
   - Logistic Regression ('max_iter=1000')  
   - Decision Tree Classifier ('random_state=42')

5. **Evaluation**  
   - Accuracy on test set  
   - Comparison charts  
   - Simplified Decision Tree visualization (depth=3)

---

## Results

- Logistic Regression Accuracy: → 0.895  
- Decision Tree Accuracy: → 0.833  

The linear model performed better, suggesting the feature-target relationship is mostly linear. The Decision Tree captured more complex patterns but may slightly overfit.

Visualizations in the notebook:  
- Class distribution  
- Model accuracy comparison  
- Simplified Decision Tree

---

## References

- Moro, S., Cortez, P., & Rita, P. (2014). *A Data-Driven Approach to Predict the Success of Bank Telemarketing*. Expert Systems with Applications.  
- Dataset: [UCI ML Repository](https://archive-beta.ics.uci.edu/dataset/222/bank%2Bmarketing?utm_source=chatgpt.com)
