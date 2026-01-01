# Project Overview: Titanic Survival Prediction
This project focuses on the end-to-end process of analyzing the Titanic dataset and developing machine learning models to predict passenger survival. The goal is to classify passengers as survivors (1) or victims (0) by leveraging data cleaning, exploratory analysis, and optimized classification algorithms.

# Part 1 – Data Analysis & Preprocessing (EDA)
Objectives:

Data Cleaning: Handled missing values in Age and Embarked and removed irrelevant or high-cardinality features such as PassengerId, Name, Ticket, and Cabin to reduce noise.

Feature Engineering: * Extracted Titles from names to capture social status.

Created AgeGroup and FareGroup bins to transform continuous numerical data into meaningful categories.

Engineered the IsAlone feature based on family size (SibSp + Parch) to identify social impact on survival.

Outlier Detection: Used boxplots and statistical analysis to detect and handle outliers in Fare and Age distributions.

Visual Exploration: Generated histograms, countplots, and correlation heatmaps to visualize the relationships between gender, class, and survival rates.

Data Encoding: Converted categorical features (Gender, Embarked, Titles) into numerical values using mapping and One-Hot encoding for model compatibility.

# Part 2 – Machine Learning Models
Objectives:

Baseline Establishment: Implemented a DummyClassifier as a baseline to evaluate whether the trained models provide a significant predictive lift.

Feature Scaling: Applied StandardScaler to ensure all numerical features are on the same scale, which is critical for distance-based models like KNN.

Model Implementation: Developed and trained two primary classification models:

Decision Tree Classifier

K-Nearest Neighbors (KNN)

Hyperparameter Tuning: * Investigated Decision Tree depth (max_depth) and splitting criteria to find the optimal balance between bias and variance.

Tested various values of k and distance metrics for the KNN model to maximize accuracy.

Performance Evaluation: Measured success using a comprehensive set of metrics:

Accuracy for overall correctness.

Precision, Recall, and F1-score to assess the model's reliability in identifying survivors.

Confusion Matrix to visualize and interpret the types of classification errors made by the models.
