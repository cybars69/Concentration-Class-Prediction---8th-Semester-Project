# K Nearest Neighbours (KNN)

It is a simple, non-parametric algorithm that works by finding the k closest neighbors to a given query point and then using those neighbors to predict the label or value of the query point

## Working and details

### Working of KNN

1. Select a value for k, which determines the number of neighbors to consider.
1. For each query point, find the k training examples that are closest to it in the feature space.
1. Assign a label or value to the query point based on the majority label or average value of its k nearest neighbors.

### Pros of using KNN

- Easy to understand and implement
- It is a non-parametric algorithm, which means it does not make any assumptions about the underlying distribution of the data.
- Can be used for both classification and regression tasks.
- It is a lazy learning algorithm, meaning it does not require any training phase. The model simply stores the training data for later use.

### Cons of using KNN

- KNN can be slow and computationally expensive, especially when dealing with large datasets.
- Highly susceptible to the curse of dimensionality, which occurs when the feature space becomes too high-dimensional.
- Very sensitive to noisy data and outliers, which can lead to poor performance.

## Results

### Confusion Matrix

![](./Confusion%20Matrix.png)

### Number of Neighbors to Consider vs Accuracy

- We can see that as the number of neighbors to be considered for prediction increases, the combined predicted group value deviates from the real value.

![](./Number%20of%20Neighbours%20vs%20Accuracy.png)

### Classification Report

|              | precision | recall | f1-score | support |
| ------------ | --------- | ------ | -------- | ------- |
| 1            | 0.89      | 0.91   | 0.90     | 158     |
| 2            | 0.94      | 0.89   | 0.91     | 157     |
| 3            | 0.91      | 0.95   | 0.93     | 164     |
| 4            | 0.93      | 0.93   | 0.93     | 160     |
| 5            | 0.94      | 0.89   | 0.91     | 150     |
| 6            | 1.00      | 0.98   | 0.99     | 164     |
| 7            | 0.87      | 0.92   | 0.89     | 167     |
|              |           |        |          |         |
| accuracy     |           |        | 0.92     | 1120    |
| macro avg    | 0.93      | 0.92   | 0.92     | 1120    |
| weighted avg | 0.93      | 0.92   | 0.92     | 1120    |

### Code can be found [HERE](/main_1%20-%20K%20Nearest%20Neighbours.ipynb)
