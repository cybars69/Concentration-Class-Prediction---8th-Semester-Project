# Random Forest (RF)

It is an ensemble learning algorithm used for classification and regression tasks. It works by building multiple Decision Trees on random subsets of the training data and then combining their predictions to produce a final prediction.

## Working and details

### Working of Random Forest

1. Randomly select a subset of the training data.
1. Build a Decision Tree on the selected subset.
1. Repeat the process for a predetermined number of trees.
1. Assign a label or value to new data points based on the majority vote or average value of the predictions of all trees.

### Pros of using Random Forest

- Random Forest can handle high-dimensional data and non-linear relationships between features and target variables.
- It is less prone to overfitting than single Decision Trees due to the use of multiple trees and the randomness introduced in the process.
- It can handle missing values and maintain accuracy even if some features are correlated.

### Cons of using Random Forest

- Random Forest can be slow and computationally expensive, especially when dealing with large datasets.
- It can be difficult to interpret the learned model and understand the contribution of individual features to the classification or regression.
- Random Forest may not work well on small datasets or datasets with imbalanced classes.

## Results

### Confusion Matrix

![](./Confusion%20Matrix.png)

### Number of Decision Tree Estimator to Consider vs Accuracy

- We can see that as the number of DT Estimators are increased, the accuracy in general increases to a certain point (96.7%)

![](./Number%20of%20DT%20Estimators%20vs%20Accuracy.png)

### Classification Report

|              | precision | recall | f1-score | support |
| ------------ | --------- | ------ | -------- | ------- |
| 1            | 0.98      | 0.98   | 0.98     | 168     |
| 2            | 0.97      | 0.99   | 0.98     | 140     |
| 3            | 0.96      | 0.96   | 0.96     | 164     |
| 4            | 0.96      | 0.96   | 0.96     | 160     |
| 5            | 0.97      | 0.97   | 0.97     | 156     |
| 6            | 0.99      | 0.98   | 0.99     | 166     |
| 7            | 0.97      | 0.96   | 0.97     | 166     |
|              |           |        |          |         |
| accuracy     |           |        | 0.97     | 1120    |
| macro avg    | 0.97      | 0.97   | 0.97     | 1120    |
| weighted avg | 0.97      | 0.97   | 0.97     | 1120    |

### Code can be found [HERE](/main_1%20-%20Random%20Forest.ipynb)
