# Online Shopper's Purchasing Intention Classification

## Abstract

The project aims to predict online shoppers' purchasing intentions based on various session predictors. It involves classifying sessions into Positive (shopper ends up shopping) and Negative (shopper does not shop). Three models, including logistic regression, naive Bayes, and neural networks, are employed for classification.

## Introduction

The dataset contains information about each online shopper's session, and the goal is to predict whether a person will shop or not. Logistic regression, naive Bayes, and neural networks are utilized for classification.

## Data Description

The dataset consists of 18 columns and 12,330 rows, including 17 feature variables and 1 target variable ("Revenue"). The project aims to predict the "Revenue" variable using relevant features. The dataset is imbalanced, with around 84.5% negative class and 15.5% positive class.

### Predictor Type Description

- Administrative: Number of administrative pages visited during the session (Numerical)
- Administrative Duration: Total time spent on administrative pages (Numerical)
- Informational: Number of informational pages visited during the session (Numerical)
- Informational Duration: Total time spent on informational pages (Numerical)
- Product Related: Number of product-related pages visited during the session (Numerical)
- Product Related Duration: Total time spent on product-related pages (Numerical)
- Bounce Rate: Percentage of visitors who enter the website and exit without triggering additional tasks (Numerical)
- Exit Rate: Percentage of pageviews on the website that end at a specific page (Numerical)
- Page Value: Average value of the page (Numerical)
- Special Day: Closeness of the browsing date to special days or holidays (Numerical)
- Month: Month of the session (Categorical)
- Operating Systems: Operating system used (Categorical)
- Browser: Browser used (Categorical)
- Region: User's region (Categorical)
- Traffic Type: Type of traffic the user is categorized into (Categorical)
- Visitor Type: Type of visitor (Categorical)
- Weekend: Boolean indicating whether the session is on a weekend (Categorical)

## Data Exploration and Cleaning

Data cleaning involves handling raw data and presenting it in a usable format. The dataset contains no null values, eliminating the need for further modifications.

## Data Exploration and Visualization

Exploring and visualizing data are essential for understanding trends. A correlation plot reveals relationships between variables, and the dataset is visualized to identify patterns.

## Methods

### 1. Logistic Regression

Logistic regression is applied as a parametric classification model. Different hyperparameters are tested to optimize the F1-score for the validation set.

### 2. Naïve Bayes

Gaussian Naïve Bayes is applied for classification, considering the conditional independence of attribute values.

### 3. Neural Network

A neural network with input, output, and hidden layers is implemented. The model undergoes experimentation to find optimal parameters and avoid overfitting.

## Data Preprocessing and Feature Engineering

Categorical variables are encoded using `pd.get_dummies()`. Redundant columns are removed, and new features are created. SMOTE technique is used to balance the target class.

## Model Selection and Implementation

Logistic Regression, Naïve Bayes, and Neural Networks are chosen for classification. Hyperparameters are tuned based on validation scores, and the results are reported for the test set.

## Test Set Results

The test set results show accuracy, F1-score, precision, and recall for each model.

## Discussion

The project discusses feature engineering, dealing with imbalanced datasets, and model selection. Logistic regression and neural networks are identified as the best models for this classification task.
