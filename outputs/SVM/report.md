# Support Vector Machine (SVM)

It is a machine learning algorithm used for classification and regression tasks. It works by finding the hyperplane that maximally separates the data into different classes or predicts the target variable with the smallest possible error.

## Working and details

### Working of SVM

1. Transform the data into a higher-dimensional space using a kernel function.
1. Find the hyperplane that maximizes the margin, i.e., the distance between the hyperplane and the closest data points.
1. Assign a label or value to new data points based on which side of the hyperplane they fall.

### Pros of using SVM

- SVM is effective in high-dimensional spaces, making it suitable for complex classification problems.
- It performs well on a wide range of datasets, even when the data is noisy.
- SVM can handle both linear and non-linear classification problems through the use of different inbuilt kernel functions.
- It is less prone to overfitting than other classification algorithms.

### Cons of using SVM

- SVM can be slow and computationally expensive, especially when dealing with large datasets.
- It does not provide probabilistic outputs, only binary classifications or regression values.
- It is difficult to interpret the learned model and understand the contribution of individual features to the classification.

## Results

### Confusion Matrix

![](./Confusion%20Matrix.png)

### Classification Report

|              | precision | recall | f1-score | support |
| ------------ | --------- | ------ | -------- | ------- |
| 1            | 0.95      | 0.95   | 0.95     | 149     |
| 2            | 0.94      | 0.97   | 0.95     | 153     |
| 3            | 0.93      | 0.95   | 0.94     | 150     |
| 4            | 0.97      | 0.97   | 0.97     | 174     |
| 5            | 0.98      | 0.90   | 0.94     | 159     |
| 6            | 1.00      | 0.99   | 1.00     | 160     |
| 7            | 0.93      | 0.96   | 0.95     | 175     |
|              |           |        |          |         |
| accuracy     |           |        | 0.96     | 1120    |
| macro avg    | 0.96      | 0.96   | 0.96     | 1120    |
| weighted avg | 0.96      | 0.96   | 0.96     | 1120    |

### Code can be found [HERE](/main_1%20-%20SVM.ipynb)
