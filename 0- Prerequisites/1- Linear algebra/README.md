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

