## Week5 Topics:
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
  

## Algorithms: 
* Adaboost
* Gradient Boost 

## Implementation Details of Programming Assignment 1:
Goal: Use the pre-implemented gradient boosted trees in scikit-learn. 

  * First to do some feature engineering.
  * Train a boosted ensemble of decision-trees (gradient boosted trees), predict whether a loan will default(on a validation set).
  * Evaluate the trained model and compare it with a baseline.
  * Explore how the number of trees influences classification performance
  * Visualize the classification performance with different number of trees
  
## Implementation Details of Programming Assignment 2:
Goal: Implement Adaboost decision tree from scratch

  * First to do some feature engineering.
  * Modify the decision trees to incorporate weights.
  * Implement Adaboost ensembling.
  * Use implementation of Adaboost to train a boosted decision stump ensemble.
  * Evaluate the effect of boosting (adding more decision stumps) on performance of the model.
  * Explore the robustness of Adaboost to overfitting.
