# Decision Tree Classifier from Scratch (Python)

## Overview

This projects implements a **Decision Tree classifier from scratch using pure Python**, without relying on machine learning 
libraries such as scikit-learn.
The goal is to demonstrate a deep, working understanding of how decision trees actually operate under the hood - including
split selection, recursion, and prediction logic.

This is **not a wrapper project**. Every step of the algorith is explicitly coded.

## Key Features
* Custom implementation of
- * Entropy
  * Best split selection
  * Recursive tree construction
    
* Clear separation of concerns:
  * **Model logic** (tree building and prediction)
  * **Training / execution script

* Importable and reusable model class

* Easily extensible to:
  * Pruning
  * Feature importance
  * Regression trees
 
## How the Model Works
1. Calculates the impurity for each possible split
2. Selects the split that minimizes impurity
3. Recursively builds left and right subtrees
4. Stops splitting based on:
   * Node purity
   * Maximum depth
   * Minimum samples per split
5. Uses majority voting at leaf nodes for prediction


## Example usage
```python
from decision_tree import DecisionTree

tree = DecisionTree(max_depth = 5)
tree.fit(x_train, y_train)

predictions = tree.predict(X_test)
```

## Why This Project Matters
Most machine learning projects rely heavily on high-level libraries. This project demonstrates:
* Algorithmic thinking
* Recursive problem solving
* Mathematical understanding of ML models
* Ability to build production-ready code instead of notebooks

This kind of implementation is especially relevant for **ML Engineering, Research, and Backend-heavy Data Science roles.**

## Future Improvements
* Tree pruning
* Feature Importance calculation
* Visualizationof tree structure
* Support for regression trees
* Performance optimizations


## Author
**Stephanie**
Data Science | ML Engineering




