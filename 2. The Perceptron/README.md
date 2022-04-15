# Single Neuron Model

### The Perceptron

In this section, I will introduce the first algorithm in Classification called Perceptron Learning Algorithm (PLA) or also known as Perceptron.

Perceptron is a Classification algorithm for the simplest case: there are only two classes (problems with only two classes are called binary classification) and also only works in a very specific case. However, it is the foundation for an important part of Machine Learning, Neural Networks and later Deep Learning. (Why is it called Neural Networks - ie neural networks).

![image](https://www.marekrei.com/blog/wp-content/uploads/2014/01/neuron_cell-1680x1050.jpg)

### The Perceptron problem

The Perceptron problem is stated as follows: Given two labeled classes, find a plane such that all points in class 1 lie on one side, all points in class 2 lie on the other side of the line. there. Assuming that such a plane exists.

If there exists a plane line separating two classes, we call the two classes linearly separable. Classification algorithms that create boundaries that are flat lines are collectively known as Linear Classifiers.

### The Perceptron Algorithm (PLA)

The basic idea of PLA is that starting from a certain predictive solution, through each iteration, the solution will be updated to a better position. This update is based on decreasing the value of some loss function.

From the data, assume X as the predictor which is a matrix of data points where each column is a data point in the space of each *d* dimension. and y are the labels corresponding to each data point stored in a vector

And We can calculate the boundary is the linear that has the equation:
$$
\min_{w\in \mathbb{R}} f(w) \:\:\:\:\:\:\:\:\:\: (\text{PROBLEM 1})
$$
 with $\bar{x}$ is the extended data point by adding the element $x_0 = 1$ in front of the vector x similar to in Linear Regression.

 So if w is a solution of the Perceptron problem, with a new data point x unlabelled, we can determine its class by simple math as follows:
 $$lable(X) = 1 if w^TX >= 0, other wise: -1$$

 Or we can rewrite: 
 $$label(X) = sgn(w^TX)$$