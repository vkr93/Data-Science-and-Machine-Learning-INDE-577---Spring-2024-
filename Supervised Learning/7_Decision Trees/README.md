#The Decision Tree Algorithm

![Image](https://miro.medium.com/v2/resize:fit:720/format:webp/1*OLJWt9hD2zTS-x3gRhYuqg.png)

Image source: [Medium](https://pub.towardsai.net/fully-explained-decision-tree-classification-with-python-d90d3bd16836)

Decision tree is a supervised learning algorithm used for classification and regression tasks. It is a type of model that learns simple decision rules from the data and builds a tree-like structure to represent the decision-making process.

The idea behind decision tree is to recursively split the data into subsets based on the values of the input features such that the target variable is more homogeneous within each subset. This is done by choosing the feature that maximizes the information gain, which is a measure of the reduction in uncertainty about the target variable after the split. The split is continued until a stopping criterion is met, such as a maximum depth of the tree or a minimum number of samples required to split a node.

The decision tree can be represented as a flowchart-like structure where each internal node represents a test on an input feature, each branch represents the outcome of the test, and each leaf node represents a class label or a regression value. The decision rule at each internal node is simply a threshold on the input feature, and the decision boundary between two classes is a hyperplane perpendicular to the feature axis.

**Algorithm:**

1.  Place the best attribute of the dataset at the root of the tree.
*   Compare the values of the root attribute with the record's attribute, then follow the branch corresponding to that value and jump to the next node using the Sum of Product representation (or Disjunctive Normal Form). For a class, every branch from the root of the tree to a leaf node having the same class is a conjunction (product) of values, different branches ending in that class form disjunction (sum).
2.  Split training set into subsets in such a way that each subset contains data with the same value for an attribute.
3.  Repeat 1-2 on each subset until you find leaf nodes in all the branches of the tree.
*   Compare the record's attribute values with other internal nodes of the tree until we reach a leaf node with the predicted class value
*   The primary challenge is to determine which attributes should be considered at each level. There are a couple popular attribute selection measures:
    *   Entropy (Information gain)
        *   Assume attributes are categorical and try to estimate the information contained by each attribute
        *   Entropy is the measure of randomness or uncertainty of a random variable X. In a binary classification problem, if all examples are positive or all are negative, entropy will be 0 (i.e. low). If half the records are of positive class and half are of negative class, entropy is 1 (i.e. high). The equation for the entropy measure is below:

        ![image](https://user-images.githubusercontent.com/89811204/146313029-48b75b32-2fc3-4376-8f82-898d03642e6d.png)

    *   Gini index
        *   Assume attributes are continuous, the index is a metric that measures how often a randomly chosen element would be inorrectly identified. Thus, we prefer a low gini index

There are a few assumptions with the training set:

*   At the beginning, the root is the whole training set
*   Feature values are preferred to be categorical. If the values are continuous, they are discretized prior to building the model.
*   Records are distributed recursively on the basis of attribute values
*   Order to placing attributes as root or internal node of the tree is done using some statistical approach

Overfitting is a common issue with decision trees. There are two approaches to avoid this:

*   Pre-Pruning
    *   Stops the tree construction early. It is preferred not to split a node it its goodness measure is below a threshhold, but it's difficult to choose a stopping point
*   Post-pruning
    *   Build a complete tree. If the tree demonstrates overfitting, then prune using cross-validation data to check the effect. The cross validation data tests whether expanding a node will make an improvement (increase in accuracy) or not


### Dataset:
[Diabete](https://www.kaggle.com/datasets/akshaydattatraykhare/diabetes-dataset) datset was used for Decision trees.

### Resources:
1.  [Decision Trees Classification](https://pub.towardsai.net/fully-explained-decision-tree-classification-with-python-d90d3bd16836)
2.  [All about Decision trees](https://www.geeksforgeeks.org/decision-tree/?ref=header_search)
3.  [DT in python](https://www.datacamp.com/tutorial/decision-tree-classification-python)

