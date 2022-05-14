# Linear Algebra - How it is used in AI ?

#### Well, Artificial Intelligence is not a single subject it has sub-fields like Learning (Machine Learning & Deep Learning), Communication using NLP, Knowledge Representation & Reasoning, Problem Solving, Uncertain Knowledge & Reasoning.

#### In this repository you will find 2 Linear algebra notebooks from [Jon Krohn's Machine Learning Foundations series](https://www.jonkrohn.com/) that will assist you in the foundations of LA, then you will have an idea and a concept to continue learning about the usage of LA in different AI fields.

- [Introduction to Linear Algebra](https://github.com/Basel-anaya/Roadmap-to-AI/blob/main/0-%20Prerequisites/1-%20Linear%20algebra/intro-to-linear-algebra.ipynb)
- [Linear Algebra II](https://github.com/Basel-anaya/Roadmap-to-AI/blob/main/0-%20Prerequisites/1-%20Linear%20algebra/linear-algebra-ii.ipynb)

---
### Describing the sub-field concepts where LA Objects can be applied.

Going through each sub-field explain bit to the concerned topic and how applying it. The following diagram explain the areas where we apply Linear Algebra in AI.

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
## Now to learn about the usage of linear algebra in ML
#### Note: This section may be too advanced, hence you have to learn about [Machine learning](https://github.com/Basel-anaya/Roadmap-to-AI/tree/main/1-%20Machine%20Learning) concept first.

### Machine Learning (ML)

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

---

## Now to learn the usage of linear algebra in DL.
#### Note: To better understand this section learn about the [Deep learning](https://github.com/Basel-anaya/Roadmap-to-AI/tree/main/2-%20Deep%20Learning) concept.

### Deep Learning (DL)

- DL is inspired by Neurons. One neuron gets connected with multiple neurons and applies activation function at the neuron.

Vectors, Matrices and Tensors are objects used in DL area. The Following diagram is the sample of a Neural Network and describes Input, Neurons, Layers, Feed Forward Propagation, Back-propagation, etc.,

There are many Mathematical Subjects involved in Deep Learning, in this article Linear Algebra is considered. Describing how Mathematical objects are being used in each stage.

![image](https://user-images.githubusercontent.com/81964452/168445688-fc6ab3c2-eaa6-45d8-b663-2ec1af2fce61.png)

#### Input: Input is in the form of Vectors, Matrices or Tensors to the Neural Network. Finally each data object/sample will be in Vectors. Here Input is a vector of n - dimensions. It is an example or data point in the data set.

#### Neurons or Nodes: Here we apply activation function for the input of previous layer and weights or connections. It is an interconnected group of natural or Artificial Neurons that uses mathematical or computational model for information processing based on a connectionistic approach to computation.

#### Connections: Connections of the biological neuron are modeled as weights.

![image](https://user-images.githubusercontent.com/81964452/168445715-908c6ead-8db6-4a53-8ec3-bf427da1579e.png)

#### Layer: Each layer contains set of neurons the following picture depicts.

![image](https://user-images.githubusercontent.com/81964452/168445724-f46146ce-f425-4bea-af68-9835433957d7.png)

#### Feedforward Propagation: These are called Deep feedforward networks or feedforward neural networks or Multilayer perceptrons (MLPs). These are called feedforward because information flows through the function being evaluated from x, through the intermediate computations used to define f, and finally to the output y.

Feedforward neural networks are called networks because they are typically represented by composing together many different functions.

- Let us say for an example our network has 3 functions connected in a chain, to form:

![image](https://user-images.githubusercontent.com/81964452/168445736-e442d8b2-8baf-4367-8012-9aa1bc02a911.png)

These chain structures are used structure of neural networks.

![image](https://user-images.githubusercontent.com/81964452/168445743-6ceecc32-f95e-43ab-892f-7ff7d17c03fd.png)

#### Let us see how we are applying using vectors and matrices in Feed forward Networks.

1. Vectorizing Inputs, Weights and Bias : x: input vector of n-dimensions; w-weight matrix of n rows and m neurons in the next layer, and bias of m neurons in the next layer.

![image](https://user-images.githubusercontent.com/81964452/168445758-0670e254-a209-4575-a007-2c36ad1d1364.png)

From this it is concluded that

![image](https://user-images.githubusercontent.com/81964452/168445765-4dab631b-27f8-4cb4-a436-c0fb8942ce07.png)

2. Apply intermediate Variable Z into activation function

![image](https://user-images.githubusercontent.com/81964452/168445772-1bac0d8c-3e78-4b1c-b546-30cbeed6c309.png)

3. The above steps repeated and results getting feed to next layer in the forward way.

At each neuron Intermediate calculation & activation function will be is as follows:

- Consider an example of Neural Network of Input 2-Features, 3-Hidden Layers and 1-Output Layers with dimensions 3,5,4,2,1 hidden units.

![image](https://user-images.githubusercontent.com/81964452/168445778-07c642e7-effc-43a1-90cf-a4ad78adf3e6.png)

Know your Matrix dimensions:

![image](https://user-images.githubusercontent.com/81964452/168445784-f80374d4-e15d-47d9-919f-c58ea8ca2169.png)

- Feedforward Propagation = Matrix-Vector product rule, addition of matrices along with activation functions.

- Back Propagation = Matrix Calculus + Linear Algebra Product Rules.

---
# Lastly we will know the usage of linear algebra in NLP.
#### Note: This is the last section, If you're having any issues understanding the ideas I advice you to learn [Natural Language Processing](https://github.com/Basel-anaya/Roadmap-to-AI/tree/main/3-%20Natural%20Language%20Processing) Concept first. 

### Natural Language Processing (NLP):

Here we describe Word2Vector (W2V)technique that is for NLP. In Word2Vec represents each distinct word with a particular list of numbers called a Vector. Based on W2V we can apply vector properties for checking the similarity and semantic similarity between vectors.

- In NLP we use Vectors and Matrices is as follows:

![image](https://user-images.githubusercontent.com/81964452/168445897-5fb2e671-21b0-41ec-bc93-b0978b8202b9.png)

#### W2V used in many of the tasks in NLP and it is the base of capturing word in to vector. Natural Language Text = Sequence of discrete symbols

![image](https://user-images.githubusercontent.com/81964452/168445906-e583c683-6778-4762-beb1-1f635e636304.png)

Produce Dense vector representation based on the context /use of words.

**What is Target & Context words:** Consider a text instance with context window size =2. Following describes

![image](https://user-images.githubusercontent.com/81964452/168445919-4f4b9ddc-98b1-482e-85d4-2bcc89eef510.png)

How to represent One-hot representation?

**Vocabulary:** The set of words encoded in to the feature vector is called the Vocabulary, so the dimension of vector is equal to the size of the Vocabulary. In short, |V| = size of the Vocabulary.

- Let us say our text data set contains the following lines

1. “And the Cute kitten purred and then …
2. “ Cute furry cat purred and miaowed…”
3. “ That the small kitten miaowed and she ..”
4. “ the loud furry dog ran and bit… ”

- From these 4 sentences basis vocabulary : { bit, cute, furry, loud, miaowed, purred, ran, small} — 8 is the vocabulary length. Let us define target and context words.

Target Word: **Kitten**, Context words: { Cute, purred, small, miaowed}

Target Word: **Cat**, Context words: { Cute, Furry, miaowed}

Target Word: **Dog**, Context words: { Loud, Furry, ran, bit }.

- Now we represent as a vector of vocabulary length 8.

![image](https://user-images.githubusercontent.com/81964452/168445964-38f96953-e7a4-45f9-a9ca-9a5a76d27ff8.png)

We defined the vectors as when context words appears then specify ‘1’, otherwise ‘0’ at the dimension of vector.

**Checking the similarity between vectors:** To check the similarity we can use the Inner product (or) cosine as similarity kernel.

Sim(Kitten,Cat)=Cosine(Kitten,Cat)~0.58; Sim(Kitten, Dog)= Cosine(Kitten, Dog) ~ 0.00; Sim(Cat,Dog)=Cosine(Cat,Dog)~0.29

![image](https://user-images.githubusercontent.com/81964452/168445981-1cf74b8c-43b8-4077-b861-354723a88a29.png)

**Embedding Matrix:** Embedding Matrix can be defined as Rows -> Target words and Columns -> Number of Context words are length of context window

![image](https://user-images.githubusercontent.com/81964452/168445988-491e63d0-7e26-4fdd-8115-2edbd3c01fe2.png)

Rows are word vectors, so we can retrieve them with one hot vectors

![image](https://user-images.githubusercontent.com/81964452/168445995-de72e08c-2a4c-4548-8aa5-0c5929013a8a.png)

#### Algorithm for constructing Embedding Matrix:

![image](https://user-images.githubusercontent.com/81964452/168446005-b461dae2-9187-4c0a-98a3-d1d93deab290.png)

- A Vector that captures the meaning of a Word. It can also be known as Word2Vec, Word Emebedding. Following are the algorithms

1. Skip-gram (SG) : Predicting Context words given by the target word
2. Continuous bag of words (CBOW): Predicts target word given by the context words
3. Glove: It makes use of global co-occurrence statistics. Glove consists of a weighted least squares model that trains on global word-word co-occurrence counts.

The above 3 algorithms explained in the usage of Linear Algebra .

**Step-1: Skip-gram (SG):** The objective of the skip-gram (SG) model is to maximize the average log probability

![image](https://user-images.githubusercontent.com/81964452/168446028-fe7ea2d5-5e00-4f26-86ad-2be1244817bf.png)

**Step-2:** Project into Vocabulary Softmax.

![image](https://user-images.githubusercontent.com/81964452/168446041-a8835cde-607c-4ff7-9a3a-0a00b6be6abb.png)

**Step 3:** Learn to estimate likelihood of Context words.

![image](https://user-images.githubusercontent.com/81964452/168446056-bde331f1-cf0e-4d57-9855-bedd702c115b.png)

**Continuous bag of words (CBOW):** It predicts target or current word based on its context words. Its possibility distribution would be

![image](https://user-images.githubusercontent.com/81964452/168446083-b035f72e-b53c-47e0-bee1-090f0ebe9c28.png)

- Project back to vocabulary size / softmax

![image](https://user-images.githubusercontent.com/81964452/168446101-ce8b4c2d-d16f-4e2d-a7da-3860eb2b53c8.png)

- Embed context words, add them.

![image](https://user-images.githubusercontent.com/81964452/168446105-6300f0a9-3dd5-491d-9e2a-4c41270437f7.png)

![image](https://user-images.githubusercontent.com/81964452/168446113-226312d1-d479-4b5a-954a-4b77eef1bc8e.png)

**GLOVE:** Like word2vec, Glove is a set of vectors that capture the semantic information (i.e., meaning about words. It consists of a weighted least squares model that trains on global word-word co-occurrence counts.

Glove makes use of Global-occurrence statistics.

**Co-occurrence matrix:** We define the this matrix using the following corpus.

"I like deep learning; I like NLP; I enjoy flying."

![image](https://user-images.githubusercontent.com/81964452/168446138-798ccca0-3571-4388-b169-e8d564b81edc.png)

Let X be the word-word co-occurrence counts matrix.

![image](https://user-images.githubusercontent.com/81964452/168446149-20502f86-6455-4000-afd6-340f72a0b26c.png)

Conclusion: Described how Linear Algebra applied in various fields of AI, it is better to be keen in Linear Algebra stuff before you move into ML, DL or NLP. I tried to cover how to apply Linear Algebra stuff in algorithmic perspective, I hope it may give strength to be involve more into Linear Algebra.

Linear Algebra promotes to other subjects like Matrix Calculus which is heavily used in Back propagation in DL.

References :

- Artificial Intelligence: A Modern Approach by Stuart Russell, Peter Norvig,
- Deep Learning Book by Ian Goodfellow and Yoshua Bengio and Aaron Courville
- https://en.wikipedia.org/wiki/Regression_analysis
- http://web.stanford.edu/class/cs224n/
- Efficient Estimation of Word Representations in vector space
- https://nlp.stanford.edu/projects/glove/
