#  The K-Nearest Neighbors Algorithm

K-Nearest Neighbor (KNN) is a non-parametric and supervised machine learning algorithm that is used for both classification and regression problems. It works by finding the k-nearest neighbors of a given query data point from the training dataset and then uses the majority vote (in classification) or the average value (in regression) of the k neighbors to predict the label or value of the query data point.


![KNN](https://intuitivetutorial.com/wp-content/uploads/2023/04/knn-1.png)


## How KNN Works

1.  Data Preparation: Start by cleaning and preprocessing the data by removing missing values and scaling the features to ensure they are on the same scale.

2.  Choose the Value of K: Select the value of k (the number of neighbors) based on the size of the dataset and the problem at hand. A small k value will lead to more flexible decision boundaries, while a large k value will lead to more rigid decision boundaries.

3.  Calculate Distances: Calculate the distance between the query data point and all the training data points using a distance metric such as Euclidean, Manhattan, or Minkowski distance.

4.  Find K-Nearest Neighbors: Select the k-nearest neighbors of the query data point based on the calculated distances.

5.  Majority Vote (Classification) or Average (Regression): For classification problems, the label of the query data point is predicted based on the majority vote of the k-nearest neighbors. For regression problems, the value of the query data point is predicted based on the average value of the k-nearest neighbors.

6.  Evaluate the Model: Finally, evaluate the performance of the model by using metrics such as accuracy, precision, recall, or mean squared error, depending on the problem at hand.

**Calculating distance** between the point and each point in the dataset (Euclidean, Manhattan, and Minkowski istance methods are common metrics for this). Note that all of these algorithms are only valid for continuous variables; Hamming distance must be used for categorical variables

![distance](https://miro.medium.com/v2/resize:fit:640/format:webp/1*10Ax3s9vQzPPYeTTVhlQKg.png)


