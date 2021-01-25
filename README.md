# Principal Component Analysis

This isn't a full machine learning algorithm, but instead an unsupervised learning algorithm.

## PCA Review

PCA is just a transformation of your data and attempts to find out what features explain the most variance in your data. For example:

<img src='PCA.png' />

## PCA Visualization

As we've noticed before it is difficult to visualize high dimensional data, we can use PCA to find the first two principal components, and visualize the data in this new, two-dimensional space, with a single scatter-plot. 
Before we do this though, we'll need to scale our data so that each feature has a single unit variance.

PCA with Scikit Learn uses a very similar process to other preprocessing functions that come with SciKit Learn. 
We instantiate a PCA object, find the principal components using the fit method, then apply the rotation and dimensionality reduction by calling transform().

We can also specify how many components we want to keep when creating the PCA object.