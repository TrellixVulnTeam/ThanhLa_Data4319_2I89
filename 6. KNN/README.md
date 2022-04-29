# K- Nearest Neighbors

![image](https://github.com/ThanhLa-IJ/ML-picture/blob/main/knn3.png)

K-nearest neighbor is one of the simplest supervised-learning algorithms (which works in some cases) in Machine Learning. When training, this algorithm does not learn anything from the training data, all calculations are performed when it needs to predict the outcome of new data. K-nearest neighbor can be applied to both types of Supervised learning problem, Classification and Regression.

With KNN, in the Classification problem, the label of a new data point (or the result of a question in the test) is directly inferred from the nearest K data points in the training set. The label of a test data can be decided by major voting between the nearest points, or it can be inferred by assigning a different weight to each of the nearest points and then deducing its label.

In a nutshell, KNN is an algorithm to find the output of a new data point by relying only on the information of K data points in the nearest training set (K-neighbors), regardless of whether some of the data points of these closest points are noise.

And For the distance measurement, we will use the *Euclidean Distance*:
$d_{(p, q)} = \sqrt{(p - q)^T(p - q)}$