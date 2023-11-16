# Smoker Status Prediction
## Overview
This repository contains code for a binary classification task: predicting a patient's smoking status based on various health indicators. The goal is to build a robust predictive model that can accurately classify individuals as smokers or non-smokers.

## Dataset
The dataset used in this project is generated from the Smoker Status Prediction using Bio-Signals dataset. It includes information about various health indicators such as age, weight, cholesterol levels, and more. The task is to predict the 'smoking' status of individuals.

## Exploratory Data Analysis (EDA)
The initial analysis includes exploring the dataset, understanding the data types, handling missing values, and visualizing the distribution of key features. Exploratory visualizations include pie charts and count plots for variables like dental caries and smoking.

## Feature Relationships
Correlation matrices and visualizations are used to identify interesting relationships between different features. Notable relationships include correlations between weight, waist, and triglycerides, as well as positive correlations between smoking and dental caries.

## Model Selection and Hyperparameter Tuning
Three different models (LightGBM, CatBoost, XGBoost) are considered for the binary classification task. Hyperparameter tuning is performed using Optuna to find the optimal set of hyperparameters for each model, maximizing the area under the ROC curve.

## Model Evaluation
The final models (LightGBM, CatBoost, XGBoost) are trained on the training dataset with the best hyperparameters. The models are then evaluated on the test set, and their predictions are combined using a weighted ensemble approach to maximize performance.

## Ensemble Approach
The ensemble approach combines predictions from LightGBM, CatBoost, and XGBoost using weights determined through optimization. This weighted ensemble aims to leverage the strengths of each individual model for a more robust and accurate prediction.

## Submission
The final ensemble predictions are submitted to Kaggle for evaluation. The submission file includes individual predictions from each model as well as the weighted ensemble prediction. At the end of the competition I classified as 663/1910
