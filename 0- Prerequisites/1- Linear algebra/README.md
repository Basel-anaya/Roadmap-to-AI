# Linear Algebra - How it is used in AI ?

Well, Artificial Intelligence is not a single subject it has sub-fields like Learning (Machine Learning & Deep Learning), Communication using NLP, Knowledge Representation & Reasoning, Problem Solving, Uncertain Knowledge & Reasoning.


### Describing the sub-field concepts where LA Objects can be applied.

Going through each sub-field explain bit to the concerned topic and how applying it. The following diagram explain the areas where we apply Linear Algebra in AI.

---

![image](https://user-images.githubusercontent.com/81964452/168445056-638e5e87-b94f-44a9-a5bb-b55b2df2fe31.png)

#### Note: Please note that Data representation, Data Processing are not the sub areas of AI, these are using in ML,DL & NLP areas.

In the above diagram other sub-areas like Problem solving, Knowledge representation and knowledge reasoning LA objects are used but not as much in Learning(ML/DL) and NLP.

![image](https://user-images.githubusercontent.com/81964452/168445093-11d17954-c12d-42b2-93e0-fffcb44ebe47.png)

### Linear Algebra or Mathematical objects are Vectors, Matrices and Tensors. Depend upon the dimensions of your data you have to choose the right object to store and process, Title diagram describes this.

Before starting how to use Mathematical Objects in AI, it is better to refresh Linear Algebra.

- Data representation: Explained in terms of Mathematical Objects Vector, Matrix and Tensor.

- Data set: It is a collection of examples or data points or objects. Each example is a collection of features. Each example is a row and feature is a column.

- Design Matrix: A Data set can be described through Design Matrix. A Design Matrix is a matrix containing a different example in each row. For example:

![image](https://user-images.githubusercontent.com/81964452/168445126-471c7c64-36e1-4d1b-8232-e4f3a36c272f.png)

If the data is not in particular order, i.e., columns are not same for each example/row. In such cases we describe as set containing ‘m’ elements of which has different vector size.

In supervised learning, data set contains a Label or target as well as collection of features.

![image](https://user-images.githubusercontent.com/81964452/168445143-d943c1a6-d109-4d1b-bfc5-918f1bd60570.png)

### Data Processing: Before we use Data sets in our ML algorithms or in any sub-field of AI, it is necessary that the data set should be ready (cleansed & filtered).

- There are 3 forms of Data processing Mean subtraction, Normalization and PCA &whitening. These forms described in short in the below diagram.

![image](https://user-images.githubusercontent.com/81964452/168445161-12d79923-72c2-40a0-88e7-3aa321feb536.png)

- These 3 form access Matrix and produces the desired. The 3rd form PCA is used for dimensionality reduction and it is totally works in pure linear algebra, following algorithm describes it.

![image](https://user-images.githubusercontent.com/81964452/168445173-5344f8f2-2611-4de0-94a6-16a8d243f618.png)

Some of the operations used in Data selection, engineering, Data cleansing, etc., argmin and argmax are the operations in Data Processing. It works on Matrices and vectors and selecting the rows or columns of minimum or maximum respectively.

Here axis can be column or row. Axis 0 (zero) means Column, axis 1(one) means Row.

- argmin: Returns the indices of the minimum values along an axis.

- argmax: Returns the indices of the maximum values along an axis.

---

### [Machine Learning (ML)](https://github.com/Basel-anaya/Roadmap-to-AI/tree/main/1-%20Machine%20Learning)

#### How LA concepts applied in ML-Regression Algorithm?
Here describes how Linear Algebra applies to Regression analysis. Explaining the concepts through Linear Multiple Regression Algorithm. The following diagram describes LA concepts in ML and DL.

![image](https://user-images.githubusercontent.com/81964452/168445302-1739bc35-5b6d-4897-8602-9200726ad21a.png)

#### Regression Analysis explain in terms of Vectors, Matrices and their properties.

### What is Regression?
It is a statistical technique for estimating the relationships between a dependent and independent variables.

- The most common form of regression analysis is Linear Regression

#### In the following equations will describe Simple and Multiple Linear Regression.

![image](https://user-images.githubusercontent.com/81964452/168445324-bcc66357-e691-4995-9790-264b300facfb.png)

#### This technique predicts continuous responses — for example, forecasting stock prices, House Rent, etc.,.

- Residual: In Machine Learning/statistical terminology, it is a difference between the observed value and the estimated value of the target variable.

Notation is given below:

![image](https://user-images.githubusercontent.com/81964452/168445342-27482d1d-0060-415d-8ec9-b8748fb0fe69.png)

#### Sum of Squares of Residuals: Let’s define residual as ‘r’.

![image](https://user-images.githubusercontent.com/81964452/168445353-d71a896f-5595-47c8-b090-692e2dc62c87.png)

#### Least Square method: Least squares method is the standard approach and it minimizes the Sum of Squares of Residuals ‘S’.

- Ordinary Least Squares (OLS) or Linear Least Squares estimate the parameters in a regression model by minimizing the sum of the squares of residuals. It draws a line through the data points that minimize the SSE between observed and predicted (or fitted or estimated ) values.

---

![image](https://user-images.githubusercontent.com/81964452/168445364-33711ba6-3e5d-4ba0-b25b-846b5e361cbb.png)

The most important application is data fitting.

#### Data Fitting: It is the process of constructing a curve fitting or mathematical function, that has the best fit to a set of data points.

- Curve fitting can be linear or non-linear. The following describes both curves.

Linear Curves:

![image](https://user-images.githubusercontent.com/81964452/168445384-19cb4d3e-19ab-4a6c-95a1-0a54cbc3ec76.png)

After the introduction of Regression Analysis let us define the loss and cost function of it.

- Loss Function: The Loss function of Linear Regression is defined is as follows

![image](https://user-images.githubusercontent.com/81964452/168445397-86b39409-eb99-4075-b672-fbcdc6d0527e.png)

Finding out the parameters by differentiation w.r.to parameters.

![image](https://user-images.githubusercontent.com/81964452/168445409-3e25bb99-9587-42d4-9613-6182e0ac6e58.png)

#### What is Regularization?
- To avoid the over-fitting problem, the regularization technique is used to shrink the magnitude of Parameters. This can be achieved by adding a penalty (a function of the sum of parameters) into the cost function. L1, L2, Drop out and Max norm constraints used in DL, whereas L1, L2, L1+L2 used in ML.

#### If you are using neural networks for ML algorithms you can apply all of the above 4 regularization techniques.

- L2 Regularization: It is the most common form of Regularization. It can be implemented by penalizing the squared magnitude of all parameters directly in the objective.

- L1 Regularization: Each weight w we add the term param*|w| to the objective function, both L1, L2 is defined is as follows:

![image](https://user-images.githubusercontent.com/81964452/168445430-65cf39d7-d66a-4779-a6ac-fc8961c277f8.png)

#### Use of Vector Norms in Machine Learning for Regularization:

![image](https://user-images.githubusercontent.com/81964452/168445451-994ece61-37c2-424c-acb5-1e56861704f1.png)

