# Breast-Cancer-Prediction
This repository contains a machine learning model built to predict whether a breast tumor is benign or malignant. The model is based on the [Breast Cancer Wisconsin dataset](https://archive.ics.uci.edu/ml/datasets/Breast+Cancer+Wisconsin+(Diagnostic)) and uses a Naive Bayes classifier to make predictions based on various tumor features.

## Table of Contents

1. [Overview](#overview)
2. [Data Preprocessing](#data-preprocessing)
3. [Model Training](#model-training)
4. [Model Evaluation](#model-evaluation)
5. [Using the Model](#using-the-model)
6. [Installation](#installation)
7. [Future Work](#future-work)

## Overview

This project uses machine learning to predict whether a breast tumor is malignant or benign using a set of 30 features like mean radius, texture, smoothness, and others, which are extracted from digitized images of fine needle aspirates (FNA) of breast tumors.

### Key features:
- **Mean Radius**: Average distance from the center of the tumor to the perimeter.
- **Mean Texture**: Standard deviation of grayscale values.
- **Mean Perimeter**: Average perimeter length of the tumor.
- **Worst Radius, Worst Perimeter, etc.**: The worst (largest) values of the above features.

The dataset contains both benign (labeled as 1) and malignant (labeled as 0) tumors.

## Data Preprocessing

The data was loaded from a publicly available dataset, which includes multiple features related to cell nuclei characteristics. Preprocessing steps included:
1. **Normalization**: Normalizing the data for better performance.
2. **Splitting the data**: 70% of the data was used for training, and 30% for testing.
3. **Label encoding**: Labels were encoded into 0 (malignant) and 1 (benign).

## Model Training

The model was trained using a Gaussian Naive Bayes classifier, which is a probabilistic model based on Bayes' Theorem. This model was chosen due to its simplicity and effectiveness in classification problems.

Steps involved:
1. Split the dataset into training and testing sets.
2. Train the Naive Bayes model on the training data.
3. Evaluate the model's performance on the test data.

## Model Evaluation

The performance of the model was evaluated using metrics such as:
- Accuracy
- Precision
- Recall
- F1-score
- ROC Curve and AUC
