📶 5G Network Call Drop Prediction using Machine Learning

This project applies machine learning techniques to predict call drops in 5G networks using a combination of network resource data and Call Detail Records (CDR).
It focuses on feature engineering, data balancing, and Random Forest optimization to identify key network performance indicators contributing to call drop events.

🚀 Project Overview

With the rapid expansion of 5G technology, maintaining consistent call quality is critical.
This project aims to predict potential call drops before they occur by analyzing parameters such as signal strength, bandwidth allocation, network load, and user behavior patterns.

By integrating advanced feature engineering techniques and hyperparameter tuning, this model improves reliability and provides actionable insights for telecom operators.

📊 Key Features

Feature Engineering:

Bandwidth_Satisfaction = Allocated_Bandwidth / Required_Bandwidth

Network_Load_Index = Active_Users / Total_Capacity

Data Balancing: Ensures equal representation of samples across datasets.

Hyperparameter Tuning: Uses RandomizedSearchCV for optimizing Random Forest parameters.

Feature Importance Visualization: Identifies most impactful network features affecting call drop probability.

Cross Validation: 5-fold CV to ensure model robustness and generalization.

🧠 Tech Stack

Language: Python

Libraries:

pandas, numpy

scikit-learn

matplotlib, seaborn

Model: Random Forest Classifier

Evaluation Metrics: Accuracy, Precision, Recall, F1 Score, Confusion Matrix

🗂️ Dataset Description

The project uses two preprocessed datasets:

5G Resource Dataset (5g_dataset_cleaned.csv):
Contains network parameters such as bandwidth, active users, and total capacity.

5G Call Detail Record Dataset (5g_cdr_cleaned.csv):
Includes call activity, duration, and call drop labels.

These datasets are balanced and merged to form the combined feature set used for training.

⚙️ Model Workflow

Load and Merge Datasets

Preprocessing & Label Encoding

Feature Engineering (custom metrics)

Scaling & Normalization

Train-Test Split (80-20)

Random Forest Training + Hyperparameter Optimization

Evaluation and Cross Validation

Feature Importance Analysis

📈 Results Summary

High accuracy and F1 score achieved through balanced data and optimized Random Forest.

Key contributors identified:

Signal Strength

Bandwidth Satisfaction

Network Load Index

These parameters strongly influence 5G call stability and drop prediction.
