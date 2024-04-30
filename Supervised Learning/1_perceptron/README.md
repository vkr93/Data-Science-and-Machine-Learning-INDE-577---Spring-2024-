A [perceptron](https://en.wikipedia.org/wiki/Perceptron) is a fundamental building block of neural networks and a basic example of a linear classifier in the field of machine learning and artificial intelligence. It represents the simplest form of a neural network model, typically used for binary classification tasks. It was developed in the 1950s by **Frank Rosenblatt**, the perceptron is designed to mimic the behavior of a biological neuron, taking in inputs and producing an output based on a linear combination of those inputs.


![Image](https://dougenterprises.com/wp-content/uploads/2021/01/perceptron.png)

*   Linear classifier: Training data should be classified into corresponding categories (i.e. if there are two categories, all  the training data must lie in those two categories)

*   Binary classifier: defines that there should only be two categories

### Key Components of a Perceptron
1. **Inputs**: A perceptron receives a set of inputs, often represented as a vector of numbers.
2. **Weights**: Each input is multiplied by a corresponding weight. Weights determine the strength and direction of the influence each input has on the final output.
3. **Bias**: A constant term added to the weighted sum of inputs. It adjusts the threshold at which the perceptron activates.
4. **Activation Function**: The perceptron uses a step function (also known as a Heaviside function or sign function) to determine its output. If the weighted sum of inputs plus bias is greater than a threshold (usually zero), the output is one (activation), otherwise it's zero (no activation).

### Perceptrons are trained in three phases:

1. **Data Processing**

As a binary classifier, perceptrons are meant to classify input into two groups: yes/no, black/white, up/down, etc, corresponding to 1/0 or 1/-1 outputs (depending on the selected activation function). To prepare data, we must first determine the two output groups and classify data in numerical terms, at which point the data will be in a format that will allow the perceptron to be trained.

2. **Predict Results**

![image](https://camo.githubusercontent.com/89394bf7f9a189643712441698e39fc7648fbf25557be99a25bb983a5869a013/68747470733a2f2f63646e2e616e616c79746963737669646879612e636f6d2f77702d636f6e74656e742f75706c6f6164732f323032302f30322f3133557064796d51782d433174424b526e664437654f672e676966)

The perceptron learning rule states that the algorithm would automatically learn the optimal weight coefficients. The input features are then multiplied with these weights in a weighted sum to determine if the neuron "fires" or not (returns 1 if positive, 0 otherwise, or 1 and -1).

![image](https://miro.medium.com/v2/resize:fit:720/format:webp/1*zQlpVcYS-mxeW3z0sRHHdQ.png)

In the equation above:

w: vector of real valued weights
b: bias (an element that adjusts the boundary away from the origin without any dependence on the input value
x: vector of input values

3. **Update Weights**

The goal is to reduce the number of misclassified points, so by iterating through the algorithm, the separation line moves in space and after a few epochs, the algorithm classifies it correctly.

In the Perceptron learnning rule, predicted output is compared with known output; if they do not match, error is propagated backward to allow weight adjustment to happen

### Limitations of Perceptrons
While perceptrons are foundational, they have limitations:

- **Linearity**: Perceptrons are linear classifiers, which means they can't solve problems that aren't linearly separable. A classic example is the XOR problem, where no linear boundary can separate the two classes.
- **Single-Layer**: A perceptron on its own is a single-layer neural network. Multi-layer perceptrons (also known as feedforward neural networks) were developed to address this limitation, allowing for more complex problem-solving.

**Read more about Perceptron:**
1.  [Understanding the Perceptron Algorthim](https://medium.com/analytics-vidhya/understanding-the-perceptron-algorithm-4a368f493109)
2. [Guided tutorial](https://pabloinsente.github.io/the-perceptron)





