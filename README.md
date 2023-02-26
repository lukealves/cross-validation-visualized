# About

This project focuses on showing the importance of cross-validation while building a model. We will use the `Stroke Prediction Data` dataset to train an `LGBMClassifier` model without any cross-validation technique and show how we might get a model with high accuracy and AUC on the training set but very low on the test set. We will then introduce different cross-validation techniques and show how they can help us achieve better results on unseen data.

# Requirements

* `pandas`
* `numpy`
* `matplotlib`
* `lightgbm`
* `scikit-learn`

# Dataset

The dataset used in this project is the `Stroke Prediction Data` which contains information about patients to predict whether they are likely to have a stroke. The data includes gender, marital status, smoking status, age, etc., and also has a "Doctor" feature added to represent the "group" within the data.

# Setup

To run the project, follow these steps:

1. Clone the repository
2. Install the required packages
3. Run the code

# Usage
The project consists of one main file `main.py`. Running this file will execute the code to train an `LGBMClassifier` model and apply different cross-validation techniques to it.

# The project is divided into several sections, as follows:

# Load and Prepare Data
This section loads and prepares the `Stroke Prediction Data` dataset for training.

# Train Without Cross-Validation
In this section, we train an `LGBMClassifier` model without using any cross-validation techniques.

# Cross-Validation Techniques
This section introduces several cross-validation techniques that can be applied to train a model.

# Time Series Split
`TimeSeriesSplit` is a cross-validation technique specifically designed for time-series data.

# K-Fold Cross-Validation
`K-Fold Cross-Validation` is a cross-validation technique where the data is divided into k-folds, and the model is trained on k-1 folds and validated on the remaining fold. This process is repeated k times, and the final result is the average of k iterations.

# Stratified K-Fold Cross-Validation
`Stratified K-Fold Cross-Validatio`n is a variation of `K-Fold Cross-Validation` designed to ensure that each fold's target variable's percentage is roughly the same as the whole dataset.

# Group K-Fold Cross-Validation
`Group K-Fold Cross-Validation` is a variation of `K-Fold Cross-Validation` where the data is divided into k-folds in such a way that each fold's groups are mutually exclusive.

# Stratified Group K-Fold Cross-Validation
`Stratified Group K-Fold Cross-Validation` is a combination of `Stratified K-Fold Cross-Validation` and `Group K-Fold Cross-Validation`, where the data is divided into k-folds in such a way that each fold's groups and target variable's percentage are roughly the same as the whole dataset.

# Train with Cross-Validation
This section applies the cross-validation techniques introduced in the previous section to train an `LGBMClassifier` model and evaluate its performance on a holdout set. We compare the results with the model trained without cross-validation.

# Conclusion

In this project, we learned the importance of cross-validation while building a model. We introduced several cross-validation techniques and showed how they can help us achieve better results on unseen data. We applied these techniques to the `Stroke Prediction Data dataset` and compared the results with the model trained without cross-validation. We saw that the model trained without cross-validation performed very poorly on the holdout set, whereas the models trained with cross-validation techniques achieved much better results.
