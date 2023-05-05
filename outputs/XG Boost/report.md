# Extreme Gradient Boost (XGBoost)

It is a gradient boosting algorithm used for classification and regression tasks. It works by building an ensemble of decision trees and sequentially adding trees to the ensemble to minimize the loss function.

### Working of XGBoost

1. Build an initial decision tree on the training data.
1. Compute the errors or residuals for the initial tree.
1. Build a new tree to predict the residuals from the previous tree.
1. Add the new tree to the ensemble and update the predictions.
1. Repeat steps 2-4 for a predetermined number of trees.

### Pros of using XGBoost

- XGBoost can handle missing values and maintain accuracy even if some features are correlated.
- It can handle a wide range of objective functions and can be used for both classification and regression tasks.
- XGBoost is computationally efficient and can handle large datasets with high dimensionality.

### Cons of using XGBoost

- XGBoost can be prone to overfitting if the model is too complex or the dataset is small.
- It can be difficult to interpret the learned model and understand the contribution of individual features to the classification or regression.
- XGBoost may not work well on datasets with imbalanced classes, requiring careful tuning of the model parameters.

## Results

### Confusion Matrix

![](./Confusion%20Matrix.png)

### Number of Decision Tree Estimator to Consider vs Accuracy

- We can see that as the number of DT Estimators are increased, the accuracy in general increases to a certain limit (95%) then diverges into noise

![](./Number%20of%20DT%20Estimators%20vs%20Accuracy.png)

|              | precision | recall | f1-score | support |
| ------------ | --------- | ------ | -------- | ------- |
| 1            | 0.94      | 0.93   | 0.93     | 148     |
| 2            | 0.97      | 0.95   | 0.96     | 156     |
| 3            | 0.93      | 0.89   | 0.91     | 160     |
| 4            | 0.93      | 0.95   | 0.94     | 164     |
| 5            | 0.92      | 0.95   | 0.94     | 154     |
| 6            | 0.99      | 0.98   | 0.99     | 163     |
| 7            | 0.96      | 0.99   | 0.97     | 175     |
|              |           |        |          |         |
| accuracy     |           |        | 0.95     | 1120    |
| macro avg    | 0.95      | 0.95   | 0.95     | 1120    |
| weighted avg | 0.95      | 0.95   | 0.95     | 1120    |

### Code can be found [HERE](/main_1%20-%20XG_Boost.ipynb)
