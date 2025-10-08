# Heart Disease Prediction Using Decision Tree and Random Forest

## Project Overview

This project aims to predict the presence of heart disease using a publicly available heart disease dataset. We build, evaluate, and interpret machine learning models, specifically Decision Tree and Random Forest classifiers. The notebook includes data preprocessing, model training, overfitting analysis, visualization, and feature importance interpretation.

## Dataset

The dataset contains 1025 patient records with 14 attributes, including demographic and medical features such as age, sex, cholesterol levels, resting blood pressure, and others.

The target variable is target, indicating the presence (1) or absence (0) of heart disease.

## Key Steps

Data Loading & Exploration

Load dataset from CSV.

Explore initial data with .head() and .info().

Data Preprocessing

Apply one-hot encoding (dummy variables) to categorical features.

Convert boolean columns to integer type for model compatibility.

## Model Training and Evaluation

Split the dataset into training and testing sets with stratification.

Train a Decision Tree Classifier and visualize the tree.

Analyze overfitting by varying tree depth and plotting train/test accuracy.

Train a Random Forest Classifier.

Evaluate models using accuracy, classification report, confusion matrix, and cross-validation.

## Interpretation

Visualize feature importance from the Random Forest model to identify key predictors.

Tools & Libraries

Python (pandas, numpy)

Scikit-learn (DecisionTreeClassifier, RandomForestClassifier, model_selection, metrics)

Matplotlib & Seaborn (for visualizations)

## Results

Achieved high accuracy on test data with both Decision Tree and Random Forest models.

Controlled model complexity to avoid overfitting with depth tuning.

Identified important features contributing to heart disease prediction through feature importance analysis.
