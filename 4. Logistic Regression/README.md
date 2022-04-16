# Logistic Regression Model

![image](https://github.com/ThanhLa-IJ/ML-picture/blob/main/logistic%20regression.png)

### The Logistic Regression 

Logistic regression is one of the supervise Learning algorithm in a series on deep learning, this is a simple but very effective algorithm in classification problems. Logistic regression is often used to compare with other classification algorithms. Logistic regression is a method of statistical analysis used to predict data values based on previous observations of a data set.

The purpose of logistic regression is to estimate the probability of events, including determining the relationship between features from which to predict the probabilities of the outcomes, so for logistic regression we will have:
+ Input: input data (we will consider there are two labels as 0 and 1).
+ Output : Probability of input data falling on label 0 or label 1.

### Machine Learning - Logistic Regression Model

Similar to the linear regression problem, we will have a set of weights w and two labels, label 0 and label 1, the learning of the model is to adjust the weight set w so that the prediction Accuracy of output as high as expect.

+ Pre-Activation Function: $Z = w_1 x_1 + w_2 x_2 + ... + w_n x_n$
+ Post Activation function: is the sigmoid Function: $a = \phi(z) = \frac{1}{1+e^{-z}}$
+ cost Function: $C_{(w, b)} = - \frac {1} {N} \displaystyle\sum_{i=1}^N P(y^{(i)}| x^{(i)})$ = $\frac {1} {N} \displaystyle\sum_{i=1}^N [-y^{(i)}log\hat{y}^{(i)} \text{ } - \text{ } (1 - y^{(i)})log(1-\hat{y}^{(i)})]$


