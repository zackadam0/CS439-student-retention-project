# CS439 Final Project: Student Retention and Academic Success Prediction

This repository contains the code, data, figures, and report materials for my CS439 final project.

## Project Overview

This project investigates whether unsupervised student segmentation can improve the interpretability and predictive modeling of academic outcomes in higher education. Using a student retention dataset, I compare baseline supervised learning models with cluster-augmented models.

The target variable has three classes:

- Dropout
- Enrolled
- Graduate

## Methods

The project includes:

- Data preprocessing
- Binary feature handling
- One-hot encoding of categorical variables
- Standard scaling of numerical variables
- K-Means clustering
- PCA visualization
- Logistic Regression
- Random Forest
- Extra Trees
- Cluster-augmented classification
- Confusion matrices
- ROC curves
- Feature importance analysis

## Main Results

The baseline Random Forest model achieved the strongest overall predictive performance, with 0.7605 accuracy and 0.8902 macro ROC-AUC. Logistic Regression achieved the highest macro F1-score of 0.6852. K-Means clustering produced interpretable student-risk profiles but did not consistently improve classifier performance when added as a model feature.

## Repository Structure

- `student_retention_project.ipynb`: main notebook containing all preprocessing, modeling, and evaluation code
- `dataset.csv`: dataset used for the project
- `figures/`: saved plots used in the final report
- `results/`: exported model results and tables
- `report/`: LaTeX report files and final PDF

## How to Run

Install the required packages:

```bash
pip install -r requirements.txt