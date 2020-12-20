## Week2 Topics:
* Maximum Likelihood estimation
* Implement MLE via gradient ascent
* Control Overfitting in logistic regression using L2 regularization

## Algorithms: 
* Build Logistic Regression from scratch

## Implementation Details of Programming Assignment 1:
Goal: implement ogistic regression classifier from scratch.

 * Extract features from Amazon product reviews, perform text cleaning
 * Convert an dataframe into multi-dimensional array.
 * Implement gradient ascent:
   - predict probability
   - derivative 
   - log-likelihood
   - stopping condition: max iteration reached/log-likelihood decrease
 * Predict sentiment using trained model, Compute classification accuracy
 
 ## Implementation Details of Programming Assignment 2:
 Goal: implement logistic regression classifier with L2 regularization from scratch
 
 * Extract features from Amazon product reviews, perform text cleaning
 * Convert an dataframe into multi-dimensional array.
 * Implement gradient ascent with L2 regularization
   - no penalization on constant
   - choose appropriate step size
 * Train LR classifiers with different level of penalties
 * Visualize effect of regularization on logistic regression
   - coefficient path for most positive words 
   - coefficient path for most negative words
 * Compute classification accuracy for different classifiers on training and validation set
 
