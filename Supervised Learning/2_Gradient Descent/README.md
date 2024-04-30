# Gradient Descent 

Gradient Descent is defined as one of the most commonly used iterative optimization algorithms of machine learning to train the machine learning and deep learning models. It helps in finding the local minimum of a function.

The best way to define the local minimum or local maximum of a function using gradient descent is as follows:

*   If we move towards a negative gradient or away from the gradient of the function at the current point, it will give the     local minimum of that function.

*   Whenever we move towards a positive gradient or towards the gradient of the function at the current point, we will get the local maximum of that function.

![image](https://static.javatpoint.com/tutorial/machine-learning/images/gradient-descent-in-machine-learning1.png)

source: [Javapoint](https://www.javatpoint.com/gradient-descent-in-machine-learning)

The algorithm can be expressed mathematically as follows:

1.  Initialize the weights of the model with random values.

2.  Compute the gradient of the MSE loss function with respect to the weights:
![image](Images/Gradient_descent.png)



4. Repeat steps 2-3 until the cost function converges to a minimum or a maximum number of iterations is reached.


The main objective of using a gradient descent algorithm is to minimize the cost function using iteration. To achieve this goal, it performs two steps iteratively:

*   Calculates the first-order derivative of the function to compute the gradient or slope of that function.

*    Move away from the direction of the gradient, which means slope increased from the current point by alpha times, where Alpha is defined as Learning Rate. It is a tuning parameter in the optimization process which helps to decide the length of the steps.

There are two main types of gradient descent, both of which are programmed from scratch in the accompanying notebook:

*   **Batch Gradient Descent (aka vanilla gradient descent):**

*   calculates the error for each example within the training dataset, but the model is only updated after all training examples have been updated 
*   the whole process is called a "training epoch"
*   Advantages: model is computationally efficient, produces stable error gradient, and a stable convergence
*   Disadvantages: stable error gradient can sometimes result in sub-optimal convergence. It also requires the entire training  set to be in memory and available to the algorithm

*   **Stochastic Gradient Descent:**

*   updates the parameters for each training example one by one
*   depending on the problem, this can make it faster than batch gradient descent
*   Advantage: frequent updates allow for a detailed rate of improvement
*   Disadvantage: frequent updates are more computationally expensive and can result in noisy gradients, which can result in an error graph with spikes rather than steady decrease

When there are one or more inputs you can use a process of optimizing the values of the coefficients by iteratively minimizing the error of the model on your training data.


To learn more about GD watch this [vidoe](https://www.youtube.com/watch?v=IHZwWFHWa-w&t=416s&ab_channel=3Blue1Brown)

### Dataset

The breast cancer [dataset](https://archive.ics.uci.edu/dataset/17/breast+cancer+wisconsin+diagnostic) is part of the datasets provided by Scikit-learn. The dataset reports weather a given tumor is benign or malignant based on its characteristics (represented by the various features in the dataset). The goal is to classify whether a given case is malignant (cancerous) or benign (not cancerous) based on these features.

