# Principle Component Analysis (PCA)

![image](https://github.com/ThanhLa-IJ/ML-picture/blob/main/fig_pca_principal_component_analysis.webp)

### Principle Component Analysis
Dimensionality Reduction is one of the important techniques in Unsupervised Machine Learning. Feature vectors in real-world problems can have very large dimensions, up to several thousand. In addition, the number of data points is often very large. If you perform storage and computation directly on data of this height, it will be difficult both in terms of storage and computation speed. Therefore, reducing the data dimension is an important step in many problems. This is also considered a data compression method.

One of the simplest Dimensionality Reduction algorithms is based on a linear model. This method is called Principal Component Analysis (PCA). something. PCA considers a special case where such special faces have linear form as subspaces.

### Machine Learning Principle Component Analysis Model
1. Stadardize (center and Scale) the Data
   1.  To set the center of the data, we calculate the average each row by replace value x by $x - \overline{x}$
   2. Because value may contain the vastly different range, so to ensure the PCA is not selecting wrong direction, we must divide the center data to standard deviation. Which mean we scale the data in each variable by finding the *z*_score: $z = \frac{x - \overline{x}}{standard deviation}$
   3. From here, we already formt he *m x n* matrix *A*
  
2. Compute the Covariance or correlation matrix
   + $S = \frac{1}{n-1}AA^T$
   + there will be two cases in this step:
     + If we only work on center data, then the *m x n* matrix is the covariance matrix
     + If we work with scaled data, then *S* is the correlation matrix.
  
3. Find the equivalent to the and the orthonormal eigenvectors of 
   + The eigenvectors are columns of the matrix *U* in the singular value decomposition of *A*, up to the factor n-1. We denote the eigenvalues by ${\sigma_i}^2$. 
   + Equivalent to the singular Value Decomposition of shifted training set matrix *A*: $A = U \Sigma V^T$

4. Find the Principle Components
   + After arrange in decrease order of the eigenvalues found in step 3. we notice the entries of each principle component ($PC_i$) are called loading scores and $PC_i$ is a linear combination of features.
  
5. Reduce the dimension of the data
   $$T = trace(S) = \frac{{\sigma_1}^2 + ... + {\sigma_m}^2}{n-1}$$
   And the i_th principle component $PC_i$ explained: $$\frac{{\sigma_1}^2/n-1}{T} = \frac{{\sigma_i}^2}{{\sigma_1}^2 + ... + {\sigma_m}^2}$$
   of the total variation.
6. 
