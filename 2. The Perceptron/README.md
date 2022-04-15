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
 + Pre-Activation Function: Z = w<sub>1</sub>x<sub>1; + w<sub>2</sub>x<sub>2 + b
  
+ Post Activation function: a = &Phi;(z)

+Activation Function: &Phi;(z) = { 1    z > 0
                                   -1   z < 0
