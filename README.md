## Implementation of Random Forest Classifier Algorithm from Scratch

### Overview:

This implementation builds the random forest classifier from scratch without using scikit-learn or other ML libraries, relying only on NumPy. It Develops a random forest classifier from the ground up without relying on external machine learning libraries. The goal is to build a robust ensemble learning model and gain a deeper understanding of the algorithm.

#### Key steps:

1. DecisionTree class defines a single tree that can be fit and used to make predictions. It implements functions for growing the tree, finding the best split, making predictions, etc. 

2. Bootstrap_sample function randomly samples the training data with replacement to create a sample set for each tree.

3. The RandomForest class initializes the number of trees, the minimum of the sample size, etc. It contains a list to hold each tree.

4. The Fit method grows each tree on a bootstrapped sample and stores it in the list of trees. 

5. The Predict method aggregates the predictions of individual trees and returns the most common prediction via a majority vote.


### Implementation:

- Created DecisionTree class to construct single decision trees using information gain criteria for node splitting. In addition, methods for predicting, and fitting were included.

- BootstrapSampling function randomly draws samples with replacement to create training data for individual trees. 

- RandomForest class initializes hyperparameters, and stores fitted (trained) trees in a list.

- Fit method grows each tree on a bootstrapped sample to completion using the DecisionTree class. 

- Predict aggregates predictions from all trees and returns the majority vote via a plurality calculation.


### Evaluation:  

Evaluation is done by calculating prediction accuracy on the test set. It is worth mentioning that this algorithm is:

  - Tested on breast cancer dataset from scikit-learn with 10-fold cross-validation.

  - Achieved well above 90% accuracy demonstrating the efficacy of the random forest approach.

  - Parameters tuning of max_depth and n_estimators (number of trees) were utilized to optimize performance.

### Skills: 

Algorithm design, NumPy, Classification, Ensemble methods, Scikit-learn datasets. 

#### Outcome: 
Successful implementation of Random Forest from scratch establishing the core understanding of the algorithm. The thorough evaluation showed the viability of the approach for real-world problems. 

On the whole, this project provides an example of my skills in algorithm design and implementation, classification modeling, and hands-on experience with standard ML techniques and datasets. It is indeed worth mentioning that the from-scratch approach strengthened conceptual understanding.
