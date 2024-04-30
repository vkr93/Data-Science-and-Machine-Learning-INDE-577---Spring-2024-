# Linear Regression

![medium](https://miro.medium.com/v2/resize:fit:1100/format:webp/1*N1-K-A43_98pYZ27fnupDA.jpeg)
**Source:** [Towards Data Science](https://towardsdatascience.com/linear-regression-explained-1b36f97b7572)



[Linear regression](https://en.wikipedia.org/wiki/Linear_regression) is a type of regression analysis that is used to predict a continuous target variable y based on one or more input features X. The model assumes a linear relationship between the input features and the target variable, and tries to fit a linear function to the data. In single neuron linear regression, a single neuron is used to model the relationship between the input variables and the output variable.

![image](https://analyticsindiamag.com/wp-content/uploads/2019/12/aim-2019-1.png) 
Source: [ANN with Linear Regression](https://analyticsindiamag.com/ann-with-linear-regression/)

Linear regression has been around for over 200 years and has been studied from every possible. Often different angles have been given different names:

*   **linear model:** a model that assumes a linear relationship between input variables (x) and a single output variable (y), with the goal of calculating y from a linear combination of the input variables (x)
*   **simple linear regression:** when there is a single input variable (x)
*   **Multiple linear regression:** when there are multiple input variables

### There are some assumptions underlying linear models:

1.  **Linearity:** The independent and dependent variables have a linear relationship with one another. This implies that changes in the dependent variable follow those in the independent variable(s) in a linear fashion. This means that there should be a straight line that can be drawn through the data points. If the relationship is not linear, then linear regression will not be an accurate model.

![image](https://media.geeksforgeeks.org/wp-content/uploads/20231123113044/python-linear-regression-4.png)

2. **Independence:** The observations in the dataset are independent of each other. This means that the value of the dependent variable for one observation does not depend on the value of the dependent variable for another observation. If the observations are not independent, then linear regression will not be an accurate model.

3.  **Homoscedasticity:** Across all levels of the independent variable(s), the variance of the errors is constant. This indicates that the amount of the independent variable(s) has no impact on the variance of the errors. If the variance of the residuals is not constant, then linear regression will not be an accurate model. 
![image](https://media.geeksforgeeks.org/wp-content/uploads/20231123113103/python-linear-regression-5.png)

4.  **Normality:** The residuals should be normally distributed. This means that the residuals should follow a bell-shaped curve. If the residuals are not normally distributed, then linear regression will not be an accurate model.


### Dataset

The [Concrete Compressive Strength Dataset](https://archive.ics.uci.edu/dataset/165/concrete+compressive+strength) is a collection of measurements of the compressive strength of concrete. It is available on the UCI Machine Learning Repository and contains data from 1030 samples of concrete, with eight input features such as cement, water, and coarse aggregate, and a single output variable, the compressive strength.


References/Resorces
1. [Linear Regression](https://www.geeksforgeeks.org/ml-linear-regression/?ref=header_search)
2. [Understanding ANN with LR](https://analyticsindiamag.com/ann-with-linear-regression/)