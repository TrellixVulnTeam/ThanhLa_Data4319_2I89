# Linear Regression Model

![image](https://github.com/ThanhLa-IJ/ML-picture/blob/main/Linear%20Regression.jpg)

### The Linear Regession 

Linear Regression is one of the most basic and popular algorithms of Supervised Learning, where the prediction output is continuous. Linear regression is used for analysing and predicting. This algorithm is a linear approach to modeling the relationship between a scalar criterion or response and multiple predictors or explanatory variables. Linear regression focuses on the conditional probability distribution of the response for the values of the predictors.

### Machine Learning - Linear Regression Algorithm 

Linear Regression or Linear Regression is an algorithm that aims to find the coefficients of an equation:

+ Pre-Activation Function: $Z = w_1 x_1 + w_2 x_2 + ... + w_n x_n$
+ Post Activation function: $a = \phi(z) = z$
+ Cost function: $C_{(w, b)} = \frac {1} {2N} \displaystyle\sum_{i=1}^N (\hat{y}^{(i)} - y^{(i)})^2$

  + and we know  $$\hat{y} = w_1 x_1 + w_2 x_2 + ... + w_n x_n$$ which is the pre_activation function

After the Loss Function is a function to finds new alphas that are more suitable for the equation as it goes through each row of data.

$w_n = w_o - \alpha \frac{\partial C_{(w, b; X, y)}}{\partial w_1}$

$b_n = b_o - \alpha \frac{\partial C_{(w, b; X, y)}}{\partial b}$

$\alpha$ is the learning rate. For ease of understanding, it can be visualized as the slope for each step when going downhill. If the $\alpha$ is large, it is easy for the foot to slip past the min point and into the region far from the center. If the $\alpha$ is too small, time to go to the end of downhill will take a long time.

After We run and train the model, we can predict how well the model work on the test data, and calling *plot decision regions* function to visualize the scatter datapoint ans show the region of space where the point is classified 



  



