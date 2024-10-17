# Satisfaction Analysis using Random Forest and Feature Sampling

This repository contains a Jupyter notebook analyzing satisfaction data from the ADVANCE Survey. The dataset consists of Likert scale responses, and the analysis focuses on identifying the factors contributing to high satisfaction levels using Random Forest classification.

## Project Overview

### Objective:
The primary objective of this analysis is to calculate the overall satisfaction score using weighted averages, and then use Random Forest to identify the key factors contributing to higher satisfaction. To address the issue of class imbalance, we applied Random Over-Sampling and SMOTE techniques.

### Key Steps:
1. **Data Preparation:**
   - The survey responses were divided into 5 broad sections. Each question and section was assigned a weight to calculate an overall satisfaction score.
   - Satisfaction scores were classified into **high** and **low** categories by setting a threshold of **0.5**.

2. **Data Preprocessing:**
   - **Mean Imputation** was used to handle missing data.
   - **MinMaxScaler** was applied to normalize the data and bring all the features to the same scale.

3. **Random Forest Classification:**
   - A Random Forest classifier was trained to identify the key features contributing to high satisfaction.
   - Class imbalance was addressed using the following techniques:
     - **Random Over-Sampling:** To duplicate instances of the minority class.
     - **SMOTE (Synthetic Minority Over-sampling Technique):** To generate synthetic samples for the minority class.

### Results:
This analysis identifies the most important factors influencing high satisfaction, and compares the effectiveness of different class balancing techniques.

## Technologies Used:
- **Python** for data analysis
- **Jupyter Notebook** for running the analysis
- **Pandas** for data manipulation
- **scikit-learn** for Random Forest and data preprocessing
- **imblearn** for handling class imbalance with RandomOverSampler and SMOTE

## How to Run:
1. Clone the repository:  
   ```bash
   git clone https://github.com/payalbhattad/Predictive-Modelling-RF-Features.git
