## Week1 Topics:
* Linear Classifiers 
* Decision boundaries
* Logistic Regression：linear score with logistic link function
* Interpreting coefficients in logistic regression
* Class probability,scores
* Encoding categorical features: one-hot encoding, label encoding, BOW
* Multiclass classification 
  - one vs all
  - one vs one

## Algorithms: 
* Logistic Regression

## Implementation Details of Programming Assignment:
The goal of this notebook is to explore logistic regression and feature engineering with existing sklearn functions and use product review data from Amazon.com to predict whether the sentiments about a product (from its reviews) are positive or negative.

* Use pandas to do some feature engineering
* Train a logistic regression model to predict the sentiment of product reviews using **Bag of words(BOW)** features.
* Inspect the weights (coefficients) of a trained logistic regression model.
* Make a prediction (both class and probability) of sentiment for a new product review.
* Given the logistic regression weights, predictors and ground truth labels, write a function to compute the **accuracy** of the model.
* Inspect the coefficients of the logistic regression model and interpret their meanings.
* Train a simpler model with fewer words.
* Compare multiple logistic regression models.
