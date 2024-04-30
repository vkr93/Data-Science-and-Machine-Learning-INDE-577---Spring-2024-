# K-Means Clustering

![image](https://images.datacamp.com/image/upload/v1678462092/image7_a1777d39aa.png)
Source: [DataCamp](https://www.datacamp.com/tutorial/k-means-clustering-python)

K-means clustering is one of the most popular unsupervised machine learning algorithms. The objective of the algorithm is to group datapoints with certain similarities together into clusters to find underlying patterns. K-means clustering does this by looking for a pre-set number (k) of clusters in that dataset. Points are only able to be part of one cluster, and each cluster has a "centroid" that roughly averages the data and represents the center of the cluster. Data points are then allocated to each of the clusters by assigning them to clusters in such a way that minimizes each cluster's sum of squares (often using Euclidean distance).

At a high level, the algorithm starts with a set of k randomly selected centroids, then iteratively optimizes the locations of those centroids until there is effectively no change in the centroids between iterations or datapoints stop changing clusters (meaning the clustering was successful) or the algorithm has completed the defined number of iterations.

The algorithm outputs 1) the centroids of the k clusters, which can be used to label new data, and 2) labels for the training data.

## How it works?
1.  Input a dataset and choose the number of clusters, k There are two primary ways of selecting the number of clusters:
    *   Elbow criterion Run k-means clustering on the dataset for a range of values of k and calculate the sum of squared errors (SSE) for each k, then calculate the mean distance between data points and their cluster's centroid. As the number of clusters increeases, the number of datapoints per cluster will decrease and will decrease the SSE until the SSE equals zero when k equals the number of datapoints. The goal is to select a small value of k with a low SSE.

    In short: run the algorithm for different values of k and plot the k values against SSE, then select the value of k for the "elbow point" where the graph dips.

    * Silhouette coefficient: The silhouette coefficient is about finding a model with well-defined clusters. This value is calculated by taking the mean distance between a sample and all other points in the same cluster as well as its distance from all other points in the nearest cluster. The equation for a single sample is below:

    ![image](https://user-images.githubusercontent.com/89811204/146045653-2898b2fa-6f54-4a50-a617-f8efb3f07ef5.png)

 Using the equation above, calculate the silhouette coefficient for all the clusters. A higher value indicates the sample is well matched to its own cluster and poorly matched to neighboring clusters.

*   Other ways to choose k: cross-validation, information criteria, information theoretic jump method, G-means algorithm   

2.  Select k random points from the data as centroids.
3. Calculate the Eucledean Distance from each feature vector to each centroid and assign each datapoint to the closest cluster centroid.

[image](https://user-images.githubusercontent.com/89811204/132998845-37a6f436-47b4-4337-a030-72bd9212d59f.png)

The algorithm in the attached notebook uses the Euclidean Distance, but there are two other ways of calculating diatance that are used in machine learning algorithms:

    *   Cosine distance: determines the cosine of the angle between the point vectors of two points in n dimensional space. The closer the point vectors are by angle, the higher the Cosine Similarity. The equation is below:

![image](https://user-images.githubusercontent.com/89811204/146046597-0f8d9449-30d1-4bc7-9560-1b271cff737b.png)

4.  Update the centroid for each cluster by taking the mean of all the datapoints assigned to that centroid's cluster.

5.  Report previous steps 3-4 until the centroids converge (no change in cetnroids), datapoints stop moving between clusters, or the algorithm reaches the maximum number of iterations. Note that the algorithm may converge on a local optimum, so it is important to run the algorithm several times.

## Datset
Cluster mall customers based on their annual income and spending score using k-means clustering algorithm, and then interpret the resulting clusters to gain insights into the purchasing behavior.


## Reference
1. [Comprehensive guide K_means Custering](https://www.analyticsvidhya.com/blog/2019/08/comprehensive-guide-k-means-clustering/)
2. [K Means Explained](https://pub.towardsai.net/fully-explained-k-means-clustering-with-python-e7caa573176a)
