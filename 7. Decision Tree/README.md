# Decision Tree

![image](https://github.com/ThanhLa-IJ/ML-picture/blob/main/Create-Decision-Tree-1.png)

### Decision Tree

Decision Tree is a structured hierarchical tree used to classify objects based on sequences of rules. The properties of the object can be of different data types such as Binary , Identical (Nominal), Ordinal (Ordinal), Quantitative while the subclass property must have a data type of Binary or Ordinal. It gives data about objects including attributes with their classes, decision trees will generate rules to predict the class of the unknown data.

Decision tree is one of the models with high interpretability and can perform both classification and regression tasks. To do classical linear models we need to make sure that the data used to train the model does not have all anomalies like missing values, outliers that need to be handled, and multicollinearity that needs to be solved. The entire data preprocessing needs to be done before that. While in Decision Tree we don't need to do any kind of pre-processing of previous data. Decision Trees are powerful enough to handle all such kinds of problems to arrive at a decision. In addition, Decision Trees are capable of handling nonlinear data that cannot be handled by classical linear models. Therefore Decision Trees are diverse enough to perform both regression and classification tasks.

### Machine Learning - Decision Tree Model

1. Recursively partition the data into multiple subsets.
2. At each node, define the variable and the rule associated with the variable for the best separation.
3. Apply the split at that node using the best variable using the rule defined for the variable.
4. Repeat step 2 and step 3 on the child nodes.
5. Repeat this process until we reach the stopping condition.
6. Assign decisions at the leaf nodes based on the majority class label present at that node if performing the classification task or considering the average of the target variable values present at that leaf node if doing regression task.

In each construction algorithm, the criteria considered to select the best feature that provides the best possible decomposition are different as the CART algorithm uses the Gini Index impurity measure to determine the best feature providing best separation.
+ Gini: $\displaystyle I_{G}(i)=1-\sum _{j=1}^{m}f(i,j)^{2}$



