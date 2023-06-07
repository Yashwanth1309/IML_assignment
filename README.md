# IMLproject
Project on PCA(Principal Component Analysis)


This ML program is done for Introduction to Machine Learning assignment for CIE3

Problem statement : "How can we use PCA Dimensionality reduction to improve upon the model"

The above ML code implements a normal Logistic Regression algorithm to obtain result to classify Handwritten Numbering characters to respective results then we use PCA to do dimensionality reduction and to reduce the components/features that are being used to determine the result.

A preview of Images in the dataset, we know these images are spread over in pixels

![IMG_20181126_220308](https://github.com/Yashwanth1309/IMLproject/assets/108111611/ec9d73ac-b7f1-4c08-99d1-711ca9c58e6b)

AS we can see in the corners and in the borders they are just plain black spots which do not actually contribute as a component to compute our result so they are just waste to include as a component. So what PCA does is eliminate these kind of situations where we can save the resources and time. As we know in ML we always try to reduce dimensions and make the result depend on less and less features.

How PCA works:-

1. Standardize the data: PCA requires standardized data, so the first step is to standardize the data to ensure that all variables have a mean of 0 and a standard deviation of 1.

2. Calculate the covariance matrix: The next step is to calculate the covariance matrix of the standardized data. This matrix shows how each variable is related to every other variable in the dataset.

3. Calculate the eigenvectors and eigenvalues: The eigenvectors and eigenvalues of the covariance matrix are then calculated. The eigenvectors represent the directions in which the data varies the most, while the eigenvalues represent the amount of variation along each eigenvector.

4. Choose the principal components: The principal components are the eigenvectors with the highest eigenvalues. These components represent the directions in which the data varies the most and are used to transform the original data into a lower-dimensional space.

5. Transform the data: The final step is to transform the original data into the lower-dimensional space defined by the principal components.

Now before applying PCA we got a good Accuracy just by Logistic regression that is 97%

Then PCA finds out 29 components that are most effective,so we eliminate the other rows and then apply the Algorithm again.
We get the almost the same result.

Now we reduce that to just 5 and still get a accuracy of 85%.

In conclusion PCA dimensionality reduction comes in very handy while we are dealing with large datasets and we have redundant components that can be ignored,all in all helping build better models.
