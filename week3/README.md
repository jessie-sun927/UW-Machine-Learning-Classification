## Week3 Topics:
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
## Algorithms: 
* Build a decision tree using DecisionTreeClassifier
* Build a binary decision tree from scratch(with binary features)

## Implementation Details of Programming Assignment 1:
Goal: Build a decision tree using data from the LendingClub to predict whether a loan will be paid off in full or the loan will be and possibly go into default.

* Data cleaning: imbalanced data, one-hot encoding
* Train a decision-tree on the LendingClub dataset.
* Predict whether a loan will default along with prediction probabilities (on a validation set).
* Train a complex tree model and compare it to simple tree model.
* Visualize decision tree, plot confusion matrix
 
 ## Implementation Details of Programming Assignment 2:
 Goal: implement  binary decision tree classifier from scratch.
    
* Transform categorical variables into binary variables.
* Write a function to compute the number of misclassified examples in an intermediate node.
* Write a function to find the best feature to split on.
* Build a binary decision tree from scratch.
* Make predictions using the decision tree.
* Evaluate the accuracy of the decision tree.
* Visualize the decision at the root node.
