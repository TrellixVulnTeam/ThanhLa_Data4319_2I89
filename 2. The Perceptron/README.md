# Single Neuron Model

![image](https://www.marekrei.com/blog/wp-content/uploads/2014/01/neuron_cell-1680x1050.jpg)

### The Perceptron 

Perceptron is a simple model of biological neuron in artificial neural network. The perceptron algorithm is designed to classify visual input, classify objects into one of two categories, and separate groups by a straight line. Classification is an important part of machine learning and image processing.

In machine learning, a perceptron is an algorithm for supervised learning of binary classifiers. It is a type of linear classifier, i.e. a classification algorithm that makes its predictions based on a linear predictor function that combines a set of weights with a feature vector.

### Machine Learning - Perceptron Learning Algorithm (PLA)

Because it is a simple algorithm, PLA only works in a very specific case where the data can only be divided into 1 of 2 classes, moreover these 2 layers must be linearly separable. calculate or in other words can use straight lines, planes ... to divide the area)

PLA is an algorithm to find linear components to divide the regions of two data classes so that all data belonging to the class are in the same region. Depending on the number of dimensions of the data, the linear component to be found can be a straight line (2 dimensions), a plane (3 dimensions) or a hyperplane (multiple dimensions).

After determining the formula of y, we find the loss function and minimize it (Remind: the loss function is the function that determines the deviation between our predicted value and the actual value, and of course we want it to be as small as possible).

With the way is to test an initial straight line with any w, it is almost certain that we will have data points that are in the wrong area as shown in the image above, so the loss function we consider is the total number of lost points. wrong area. However, considering the sign function is quite difficult, we will consider the loss function as the total data value of the points in the wrong area. This new loss function still has the same minimum value as the old function (zero because we have to divide so that no data is in the wrong area).

And We can calculate the boundary is the linear that has the equation:
 + Pre-Activation Function: Z = w<sub>1</sub> x<sub>1</sub> + w<sub>2</sub> x<sub>2</sub> + b
 + Post Activation function: a = &Phi;(z)
 + Activation Function: &Phi;(z) = { (1 if z > 0) (-1 if z < 0)

After 
