# Bank Marketing Classification

This repository contains a Jupyter Notebook comparing **Logistic Regression** and **Decision Tree** on the Bank Marketing dataset from UCI.  

## Overview

This project reproduces a study based on the Bank Marketing dataset from the UCI Machine Learning Repository. The goal is to predict whether a bank client will subscribe to a term deposit after a marketing campaign. The original study is: Moro, Cortez, and Rita (2014), *A Data-Driven Approach to Predict the Success of Bank Telemarketing*, published in *Expert Systems with Applications*.  

Two classification algorithms covered in class, Logistic Regression and Decision Tree, are applied to replicate the methodology described in the study and evaluate their performance on the same dataset.

## Dataset

- File: `bank-full.csv`  
- Folder: `data/`  
- Source: [Bank Marketing Dataset - UCI ML Repository](https://archive-beta.ics.uci.edu/dataset/222/bank%2Bmarketing?utm_source=chatgpt.com)  
- Notes: The dataset contains client information, campaign features, and the target variable (`y`) indicating subscription.

## Notebook

The main notebook contains preprocessing, model training, evaluation, and visualizations.

- File: `notebooks/BankMarketing_Classification_Samantha_Moataz.ipynb`  
- Open directly in Google Colab: [Open in Colab](https://colab.research.google.com/github/SamanthaAValdez/bank-marketing-classification/blob/main/notebooks/BankMarketing_Classification_Samantha_Moataz.ipynb)

## How to Run

1. Open the notebook in **Google Colab** or **Jupyter Notebook**.  
2. Ensure the dataset file `bank-full.csv` is inside the `data/` folder.  
3. Run all cells sequentially to reproduce the results.

## Results

- Logistic Regression Accuracy: ~0.895  
- Decision Tree Accuracy: ~0.833  

The linear model performed better, suggesting that the relationship between the features and the target is mostly linear. The Decision Tree captured more complex patterns but may have slightly overfitted the data, resulting in lower generalization on the test set.  

Visualizations such as class distribution and model comparison charts are included in the notebook.
