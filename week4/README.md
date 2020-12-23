## Week4 Topics:
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


## Algorithms: 
* Build a decision tree with stopping conditions and erly stopping conditions


## Implementation Details of Programming Assignment:
Goal: Explore various techniques for preventing overfitting in decision trees.

* Implement binary decision trees with different early stopping methods.
  - Stopping condition:
    1. All examples have the same target value 
    2.  No more features to split on
  - Early stopping conditions:
    1. reached max_depth
    2. reached min error reduction
    3. reahced min node size
* Compare models with different stopping parameters.
* Visualize the concept of overfitting in decision trees.
 
