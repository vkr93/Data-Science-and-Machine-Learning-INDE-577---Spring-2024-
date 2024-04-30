# The Random Forest Algorithm

Random Forest is an ensemble learning method that combines multiple decision trees to improve the accuracy and stability of predictions. It can be used for both regression and classification tasks.

The key idea behind Random Forest is to build a large number of decision trees and then combine their predictions through voting. Each decision tree is trained on a random subset of the training data and a random subset of the features. This introduces randomness into the model and helps to reduce overfitting.
![Image](https://media.geeksforgeeks.org/wp-content/uploads/20240219150749/Random-Forest-Algortihm.png)


Source: [GG](https://www.geeksforgeeks.org/random-forest-algorithm-in-machine-learning/?ref=header_search)

The two most popular ensemble methods are:

*   **Bootstrapping:** Training a bunch of individual models in a parallel way. Each model is trained by a random subset of the data
*   **Bagging:** Training a bunch of individual models in a sequential way. Each individual model learns from mistakes made by the previous model.


## Working of Random Forest

The Random Forest algorithm works in the following steps:

1.  Random Sampling: Randomly select "m" samples from the dataset with replacement. This forms the training data for one decision tree.
2.  Random Feature Selection: Randomly select "p" features from the total "n" features. This is done to reduce the correlation among the trees.
3.  Build Decision Tree: Build a decision tree using the selected features and samples.
4.  Repeat: Repeat steps 1 to 3 "k" times to create "k" decision trees.
5.  Prediction: For a new data point, make predictions using all the "k" decision trees and take a majority vote to get the final prediction.

The fundamental principle of ensemble methods is based on randomization. There are three main decisions to make when constructing a tree:

*   method for splitting the leaves
*   type of predictor used in each leaf
*   method for injecting randomness into the tree (bagging or bootstrapping)

There are a few stopping criteria:

*   minimum number of samples in a terminal node to allow it to split
*   minimum number of samples in a leaf node when the terminal node is split
*   maximum tree depth, i.e. the maximum number of levels a tree can grow
*   Tree accuracy (defined by the Gini Index) is less than a fixed threshold



## Dataset:
The [Concrete Compressive Strength](https://archive.ics.uci.edu/dataset/165/concrete+compressive+strength) Dataset is a collection of measurements of the compressive strength of concrete. It is available on the UCI Machine Learning Repository and contains data from 1030 samples of concrete, with eight input features such as cement, water, and coarse aggregate, and a single output variable, the compressive strength.

Explanation of each variable in the Concrete Compressive Strength Dataset:

Cement (kg/m3): The amount of cement used in the concrete mixture, measured in kilograms per cubic meter.

Blast Furnace Slag (kg/m3): The amount of blast furnace slag used in the concrete mixture, measured in kilograms per cubic meter.

Fly Ash (kg/m3): The amount of fly ash used in the concrete mixture, measured in kilograms per cubic meter.

Water (kg/m3): The amount of water used in the concrete mixture, measured in kilograms per cubic meter.

Superplasticizer (kg/m3): The amount of superplasticizer used in the concrete mixture, measured in kilograms per cubic meter.

Coarse Aggregate (kg/m3): The amount of coarse aggregate (such as gravel or crushed stone) used in the concrete mixture, measured in kilograms per cubic meter.

Fine Aggregate (kg/m3): The amount of fine aggregate (such as sand) used in the concrete mixture, measured in kilograms per cubic meter.

Age (days): The age of the concrete sample at the time of testing, measured in days.

Concrete Compressive Strength (MPa): The compressive strength of the concrete sample, measured in megapascals (MPa). This is the target variable that we are trying to predict.

## Resources:

1.  [Random Forest](https://www.datacamp.com/tutorial/random-forests-classifier-python)
2.  [RF Algoithm](https://www.geeksforgeeks.org/random-forest-algorithm-in-machine-learning/?ref=header_search)
 