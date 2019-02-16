# Predicting-Bike-Sharing-Patterns
Neural Network Project [Udacity Deep Learning Nanodegree]

## Project Overview
Build a neural network from scratch and use it to predict daily bike rental ridership. 


## Project Overview
### Project Description
Evaluate 10 supervised learning algorithms that are currently available in scikit-learn on data collected for the U.S. census to help CharityML (a fictitious charity organization) identify people most likely to donate to their cause. 

### Project Procedure
- Explore the data
- Preprocesse the data
  - Transfered skewed continous features
  - One-hot encoding
- Evaluate performance of several supervised learning algorithms
  - Gaussian Naive Bayes (GaussianNB)
  - Decision Trees
  - Ensemble Methods (Bagging, AdaBoost, Random Forest, Gradient Boosting)
  - K-Nearest Neighbors (KNeighbors)
  - Stochastic Gradient Descent Classifier (SGDC)
  - Support Vector Machines (SVM)
  - Logistic Regression
- Choose the best model
- Tune model parameters using grid search
- Evaluate feature importance to optimize the model's performance
  - feature_importances_  attribute 
  - recursive feature elimination(RFE)

### Project Results
  - Gradient Boosting algorithm performed best in f-score and accuracy on the testing dataset
  - Improve model performance after tuning model using grid search
  
    | Metric | Unoptimized Model | Optimized Model |
    | :---:   | :-: | :-: |
    | Accuracy | 0.8630 | 0.8705 |
    | F-score | 0.7395 | 0.7513 |
    
  - Both accuracy score and f-score are slightly declined on the reduced data(top 5 important features) than the scores on the full data.     However, it decreases substantial training time. 
  
    | Metric | Final Model trained on full data |  Final Model trained on reduced data  |
    | :---:   | :-: | :-: |
    | Accuracy | 0.8705 | 0.8590 |
    | F-score | 0.7513 | 0.7252 |
    | Train time | 5.7013 | 54.9721|

## Getting Started
### Prerequisites

### Run
In a terminal or command window, run one of the following commands:

```bash
ipython notebook finding_donors.ipynb
```  
or
```bash
jupyter notebook finding_donors.ipynb
```

This will open the iPython Notebook software and project file in your browser.

### Data
Download data from the [UCI Machine Learning Database](https://archive.ics.uci.edu/ml/datasets/Bike+Sharing+Dataset)
