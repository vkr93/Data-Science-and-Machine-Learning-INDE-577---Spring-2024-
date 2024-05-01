# Principal Component Analysis (PCA)

Principal Component Analysis is basically a statistical procedure to convert a set of observations of possibly correlated variables into a set of values of linearly uncorrelated variables. 

Each of the principal components is chosen in such a way that it would describe most of them still available variance and all these principal components are orthogonal to each other. In all principal components, first principal component has a maximum variance.

![Image](https://camo.githubusercontent.com/f8c57d591f7f5cba8d6c3af40f50b3a05c2d31ae3c7f87a19532e60d862bf6be/68747470733a2f2f6d69726f2e6d656469756d2e636f6d2f6d61782f323135382f302a354961773934776c594354703047754b2e706e67)


**Uses of PCA:** 

1.  It is used to find interrelations between variables in the data.
2.  It is used to interpret and visualize data.
3.  The number of variables is decreasing which makes further analysis simpler.
4.  It’s often used to visualize genetic distance and relatedness between populations.

These are basically performed on a square symmetric matrix. It can be a pure sums of squares and cross-products matrix Covariance matrix or Correlation matrix. A correlation matrix is used if the individual variance differs much.

## Objectives of PCA: 

1.  It is basically a non-dependent procedure in which it reduces attribute space from a large number of variables to a smaller number of factors.
2.  PCA is basically a dimension reduction process but there is no guarantee that the dimension is interpretable.
3.  The main task in this PCA is to select a subset of variables from a larger set, based on which original variables have the highest correlation with the principal amount.
4.  Identifying patterns: PCA can help identify patterns or relationships between variables that may not be apparent in the original data. By reducing the dimensionality of the data, PCA can reveal underlying structures that can be useful in understanding and interpreting the data.
5.  Feature extraction: PCA can be used to extract features from a set of variables that are more informative or relevant than the original variables. These features can then be used in modeling or other analysis tasks.
6.  Data compression: PCA can be used to compress large datasets by reducing the number of variables needed to represent the data, while retaining as much information as possible.
7.  Noise reduction: PCA can be used to reduce the noise in a dataset by identifying and removing the principal components that correspond to the noisy parts of the data.
8.  Visualization: PCA can be used to visualize high-dimensional data in a lower-dimensional space, making it easier to interpret and understand. By projecting the data onto the principal components, patterns and relationships between variables can be more easily visualized.


![image](https://miro.medium.com/v2/resize:fit:1400/0*PZk89dEQZubeWz4-)
Source: [Medium](https://medium.com/@yashj302/principal-component-analysis-pca-nlp-python-ce9caa58bd7a)


### Dataset

**Iris** dataset was used.

### References:
1. [PCA](https://www.geeksforgeeks.org/principal-component-analysis-with-python/?ref=header_search)
2. [Principal Component Analysis (PCA) in Python Tutorial](https://www.datacamp.com/tutorial/principal-component-analysis-in-python) 

