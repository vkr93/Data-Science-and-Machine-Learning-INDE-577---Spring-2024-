# Logistic Regression

![Difference b/w linear/logistic Regression](https://editor.analyticsvidhya.com/uploads/711091.png)


Logistic regression is used for classification tasks where the goal is to predict the probability that an instance belongs to a given class or not. Logistic regression is a statistical algorithm which analyze the relationship between two data factors. The article explores the fundamentals of logistic regression, it’s types and implementations.

With this we carry out binary classification where we use [sigmoid function](https://www.geeksforgeeks.org/derivative-of-the-sigmoid-function/), that takes input as independent variables and produces a probability value between 0 and 1.

For example, we have two classes Class 0 and Class 1 if the value of the logistic function for an input is greater than 0.5 (threshold value) then it belongs to Class 1 otherwise it belongs to Class 0. It’s referred to as regression because it is the extension of linear regression but is mainly used for classification problems.

![sigmoid function](https://media.geeksforgeeks.org/wp-content/uploads/20190522162153/sigmoid-function-300x138.png)

### Key Points:

*   Logistic regression predicts the output of a categorical dependent variable. Therefore, the outcome must be a categorical or discrete value.
*   It can be either Yes or No, 0 or 1, true or False, etc. but instead of giving the exact value as 0 and 1, it gives the probabilistic values which lie between 0 and 1.
*   In Logistic regression, instead of fitting a regression line, we fit an “S” shaped logistic function, which predicts two maximum values (0 or 1).


### Types of Logistic Regression
O
n the basis of the categories, Logistic Regression can be classified into three types:

1.  Binomial: In binomial Logistic regression, there can be only two possible types of the dependent variables, such as 0 or 1, Pass or Fail, etc.
2.  Multinomial: In multinomial Logistic regression, there can be 3 or more possible unordered types of the dependent variable, such as “cat”, “dogs”, or “sheep”
3.  Ordinal: In ordinal Logistic regression, there can be 3 or more possible ordered types of dependent variables, such as “low”, “Medium”, or “High”.

## Summary

In summary, logistic regression can be implemented using a single output neuron with a sigmoid activation function. The neuron takes a set of input features, applies a weighted sum to them, adds a bias term, and then passes the result through the sigmoid function to obtain the predicted probability of the binary outcome. The neuron can be trained using the cross-entropy loss and gradient descent to find the values of the weights and bias that minimize the cost function. Once the parameters have been learned, the neuron can be used to predict the probability of the binary outcome for a new input vector.

## Dataset

[Breast Cancer Datset](https://scikit-learn.org/stable/modules/generated/sklearn.datasets.load_breast_cancer.html) was used in the notebook.


Resources

1. [Logistic Regression in ML](https://scikit-learn.org/stable/modules/generated/sklearn.datasets.load_breast_cancer.html)
2. [A beginners guide to LR](https://www.analyticsvidhya.com/blog/2021/08/conceptual-understanding-of-logistic-regression-for-data-science-beginners/)