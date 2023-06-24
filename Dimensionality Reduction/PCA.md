Suppose we have a dataset with two variables, X1 and X2, and we want to reduce the dimensionality of the data from 2 to 1 using PCA.

Step 1: Standardization
First, we need to standardize the data by subtracting the mean and dividing by the standard deviation of each variable. This is done to ensure that all variables have the same scale.

Step 2: Covariance Matrix
Next, we calculate the covariance matrix of the standardized data. The covariance matrix provides information about the relationships between the variables.

Step 3: Eigendecomposition
We perform an eigendecomposition on the covariance matrix to obtain the eigenvectors and eigenvalues. The eigenvectors represent the directions of the principal components, and the eigenvalues represent the amount of variance explained by each principal component.

Step 4: Selecting Principal Components
We select the principal components based on the eigenvalues. The principal component with the highest eigenvalue explains the most variation in the data, and so on. In our example, since we want to reduce the dimensionality to 1, we select the principal component with the highest eigenvalue.

Step 5: Projection
Finally, we project the standardized data onto the selected principal component. This projection is done by taking the dot product of the standardized data and the selected eigenvector.

Let's say the eigenvector corresponding to the highest eigenvalue is [0.6, 0.8]. We can calculate the projected values by multiplying each standardized data point by this eigenvector. This will give us the reduced-dimensional representation of the data.

By applying PCA, we have transformed our original dataset from two dimensions (X1 and X2) to one dimension (the projected values on the selected principal component).