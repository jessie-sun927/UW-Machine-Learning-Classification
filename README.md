# UW-Machine-Learning-Classification 
This is the third course in ML specialization and it focus on classification algroithms.

### [Week1](https://github.com/jessie-sun927/UW-Machine-Learning-Classification/tree/main/week1):
* Linear Classifiers 
* Decision boundaries
* Logistic Regression：linear score with logistic link function
* Interpreting coefficients in logistic regression
* Class probability,scores
* Encoding categorical features: one-hot encoding, label encoding, BOW
* Multiclass classification 
  - one vs all
  - one vs one
  
  
### [Week2](https://github.com/jessie-sun927/UW-Machine-Learning-Classification/tree/main/week2):
* Maximum Likelihood estimation
* Implement MLE via gradient ascent
* Control Overfitting in logistic regression using L2 regularization


### [Week3](https://github.com/jessie-sun927/UW-Machine-Learning-Classification/tree/main/week3):
* Dealing  with imbalanced data, categorical features
* Greedy decision tree learning Algorithm
  - select best feature to split on 
    * classification error
    * Gini impurity
    * infomation gain
  - stopping condition:
    * all data in the nodes fall into the same class
    * used up all possible features
    * reached maximum depth
* Visualize decision tree, plot confusion matrix
* Dealing with continuous numerical features, multi-choice
  - Try on thresholds
  - Try on single features and its combinations
  
  
### [Week4](https://github.com/jessie-sun927/UW-Machine-Learning-Classification/tree/main/week4):
* Overfitting in decision trees
* Principal of Occam's razor
  - when two trees have similar classification error on the validation set, pick the simpler one
* Prevent overfitting:
  - Early stopping: stop learning algorith before tree become too complex
    * Stop if the depth of tree reached max_depth
    * Stop if error doesn’t decrease by more than ε 
    * Stop if number of data points contained in a node is too small 
    * Potential Problem in early stopping: stop too early, miss out on "good" splits
  - Tree Pruning: simplify tree after learning alogrithm finished
    * Cost function: balance how well tree fits data and the complexity of tree
    * Total cost = measure of fit + measure of complexity, prune if the total cost is lower after pruning
    
    
### [Week5](https://github.com/jessie-sun927/UW-Machine-Learning-Classification/tree/main/week5):
* AdaBoost: an adaptive learning algroithm 
  - step1: initialize with same weight for all points
  - step2: learn decision stump
    - pick the decision stump with lowest weighted training error(or Gini impurity）according to the weights
    - compute amount of say of the stump(i.e. stump weights)
    - Compute updated weights 
    - normalize weights
  - step3: use updated weights of observations to build another decision stump
  - step4: make final prediction by model ensembling
  - summary: 
    - Adaboost is an adaptive learning algorithm which combines and weights weak learners 
    - Stump weights and data point weights are two different concepts. Stump weights tell how important each stump is while making predictions with the entire boosted ensemble. Data point weights tell how important each data point is while training a decision stump
    - Adaboost gives lower weights for correctly classified observations in the next decision stump learning, gives higher weights for incorrectly classified observations. Adaboost gives higher weights for decision stumps which has lower classification error in final prediction, lower weights for decision stumps which has higher classification error
  - Disadvatage of adaboost: Very sensitive to outliers, outliers will be given high weights in stump learning
  
* Gradient Boost: Another adaptive learning algorithm under boosting family
  - loss function: squared loss
  - step1: initialize the prediction
  - step2: fit a regression tree to residuals 
    - fit the regression tree by minimizing MSE
    - compute output value for ech leaf
    - update the predictions with learning rate
  - step3: keep doing stpe2 until maximum number of tree reached, make final prediction with the most updated prediction
  - Difference with Adaboost:
    - different adpative pattern: adaboost learn adaptive model by giving higher weights for misclassified samples, gradient boost learn adaptive model by learning residuals
  

### [Week6](https://github.com/jessie-sun927/UW-Machine-Learning-Classification/tree/main/week6):
* Evaluation metrics for classifiers
* Precision: Fraction of positive predictions that are actually positive
* Recall: Fraction of positive data predicted to be positive 
* Trade-off precision and recall by setting probability threshold
  - Pessimistic model: high precision, low recall
  - Optimistic model: low precision, high recall
* Choosing evaluation metric:
  - F1 measure, area-under-curve(AUC)
  - precision at k
  
### [week7](https://github.com/jessie-sun927/UW-Machine-Learning-Classification/tree/main/week7):
* Stochastic gradient ascent
  - adapt for new data
  - very sensitive to parameters, noisy convergence
* Mini-batch gradient ascent 
