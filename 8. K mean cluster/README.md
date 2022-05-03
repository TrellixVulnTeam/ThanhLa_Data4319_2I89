# K Mean Clustering

![image](https://github.com/ThanhLa-IJ/ML-picture/blob/main/k%20mena%20clustering.jpg)

### K mean Clustering

K_mean_clustering 

K mean clustering is one of the most basic algorithms of Unsupervised learning. In this algorithm, we do not know the label of each data point. The goal is how to divide data into different clusters so that the data in the same cluster has the same properties.

The simplest idea of a cluster is a collection of points that are close to each other in some space (this space can have many dimensions in case the information about a data point is very large).

Each cluster has a representative point (center), and the points around each center belong to the same group as that center. In the simplest way, considering any point, we consider which point is closest to the center, then it belongs to the same group as that center.

### Machine Learing K Mean Clustering Model
The ultimate goal of this clustering algorithm is: from the input data and the number of groups we want to find, specify the center of each group and assign the data points to the corresponding groups.

1. $X = [x_1, x_2,..., x_N] \epsilon R^{d*N}$ and $k < N$ is the number of clusters we want to split. We need to find the centers $m_1, m_2,...m_k$  $\epsilon R^{d*1}$ and label of each datapoint
2. With each $x_i$ that $y_i = [y_{i1}, y_{i2},..., y_{ik}]$ 
   where $x_i$ is assigned to cluster k, we have: $$y_{ik} \epsilon \{0, 1\}, \sum_{k=1}^{k} y_{ik} = 1$$
3. After find the k cluster for each point, and assign the datapoint to each cluster. Keep Update the center for each cluster by averaging all the data points assigned to the cluster