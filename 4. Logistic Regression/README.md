# Logistic Regression Model

![image](https://github.com/ThanhLa-IJ/ML-picture/blob/main/logistic%20regression.png)

### The Logistic Regression 

Logistic regression is one of the supervise Learning algorithm in a series on deep learning, this is a simple but very effective algorithm in classification problems. Logistic regression is often used to compare with other classification algorithms. Logistic regression is a method of statistical analysis used to predict data values based on previous observations of a data set.

The purpose of logistic regression is to estimate the probability of events, including determining the relationship between features from which to predict the probabilities of the outcomes, so for logistic regression we will have:
+ Input: input data (we will consider there are two labels as 0 and 1).
+ Output : Probability of input data falling on label 0 or label 1.

### Machine Learning - Logistic Regression Model

Similar to the linear regression problem, we will have a set of weights w and two labels, label 0 and label 1, the learning of the model is to adjust the weight set w so that the prediction Accuracy of output as high as expect.

+ Post Activation function: is the sigmoid Function: $a = \phi(z) = \frac{1}{1+e^{-z}}$

  + Is a continuous function and takes values in the interval (0;1): $\exists x with \forall we have \lim_{x \to c} f(x) = f(c))$
  + Because it is a continuous function, the sigmoid function will have a derivative at every point.

    Derivative: $\frac{\partial \sigma(x)}{\partial x} = \frac{e^{-x}}{(1+e^{-x})^2}$

After go over Perceptron and Linear Regression, I know that all real regressions share the same pre-Activation Function equation to help show how the objective variable y (the dependent variable) will change based on the relationship between the its relationship with all independent variables x regardless of whether the relationship is nonlinear or linear:
+ Pre-Activation Function: $Z = w_1 x_1 + w_2 x_2 + ... + w_n x_n = w^Tx+w_0$

+ Apply the sigmoid function to convert the value $w^T + w_o$ into a probability to conclude the value of the variable y from which to determine the label of input x: $P = \frac{1}{1 + e^{-(w^Tx+w_0)}}$

    => Finish build the logistic Regression Model
  
+ cost Function: $C_{(w, b)} = - \frac {1} {N} \displaystyle\sum_{i=1}^N P(y^{(i)}| x^{(i)})$ = $\frac {1} {N} \displaystyle\sum_{i=1}^N [-y^{(i)}log\hat{y}^{(i)} \text{ } - \text{ } (1 - y^{(i)})log(1-\hat{y}^{(i)})]$

The cost function in a supervised learning algorithm is a function to measure the difference between the actual value and the predicted model value, the difference can be different from the true value (as in the linear regression model) or difference in labels (as in the classification problem) how to define the difference depends on each specific problem from which to build the loss function.

After We run and train the model, we can predict how well the model work on the test data, and calling *plot decision regions* function to visualize the scatter datapoint ans show the region of space where the point is classified 