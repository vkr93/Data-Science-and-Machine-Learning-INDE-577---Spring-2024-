# Density-Based Spatial Clustering of Applications with Noise (DBSCAN)

DBSCAN (Density-Based Spatial Clustering of Applications with Noise) is a clustering algorithm that groups together points that are closely packed together in high-density regions, while points in low-density regions are considered outliers or noise.

The algorithm works by defining a distance threshold (eps) and a minimum number of points (minPts) to form a dense region. Starting from an arbitrary point, the algorithm checks if there are enough neighboring points within the distance threshold to form a dense region. If there are, the region is expanded to include the neighboring points, and the process is repeated until no more points can be added. The process then continues with a new arbitrary point that has not yet been assigned to any cluster.

![Image](https://cdn-images-1.medium.com/max/640/1*MP0ZCqyW9vPYQCGfs8G-Cg.png)

The working of DBSCAN can be summarized in the following steps:

1.  DBSCAN requires two parameters to be set before running the lgorithm - epsilon (ε) and the minimum number of points required to form a dense region (minPts).
2.  The algorithm starts by randomly selecting a point from the dataset.
3.  It then checks if there are at least minPts points within a radius of ε around this point.
4.  If there are, it forms a dense region around the point, and all the points within the radius are marked as belonging to the same cluster.
5.  The algorithm repeats this process for all the points in the dense region until no more points can be added to the cluster.
6.  If there are not enough points within ε of the starting point to form a dense region, the point is marked as noise and the algorithm moves on to the next unvisited point.

DBSCAN can handle clusters of different shapes and sizes and can also identify noise points that do not belong to any cluster.


### Dataset

The **Mall Customer Segmentation** Data is a dataset that contains information about customers of a mall, and it is often used for customer segmentation or clustering analysis. This dataset can be useful for businesses, marketers, or analysts who are interested in understanding their customers' behavior and preferences to optimize their marketing strategies or product offerings.

1.  Explanation of each variable in the Dataset:

2.  CustomerID: unique identifier for each customer.

3.    Gender: the gender of the customer, either Male or Female.

4.  Age: the age of the customer.

5.  Annual Income (k$): the annual income of the customer in thousands of dollars.

6.  Spending Score (1-100): a score assigned by the mall based on customer behavior and spending nature.

### Refernces

1.  [DBSCAN Clustering in ML](https://www.geeksforgeeks.org/dbscan-clustering-in-ml-density-based-clustering/?ref=header_search)
2.  [DBSCAN: A Macroscopic Investigation in Python](https://www.datacamp.com/tutorial/dbscan-macroscopic-investigation-python)