# Decision Tree

Decision Tree is a machine learning algorithm used for classification and regression tasks. It works by recursively splitting the data into subsets based on the most informative features until each subset is pure or the stopping criterion is met.

## Working and details

### Working of Decision Tree

1. Select a feature that best splits the data based on a certain criterion, such as information gain or Gini index.
1. Split the data into subsets based on the selected feature.
1. Repeat the process for each subset until a stopping criterion is met, such as a maximum depth or minimum number of samples in each leaf node.
1. Assign a label or value to new data points based on the path they take through the tree.

### Pros of using Decision Tree

- Decision Tree is easy to understand and interpret, making it suitable for exploratory data analysis.
- It can handle both categorical and numerical features and can perform well even with missing data.
- Decision Tree can handle both classification and regression tasks.

### Cons of using Decision Tree

- Decision Trees can be sensitive to small variations in the data, leading to different trees for the same data.
- It can be biased towards features with many levels or high cardinality.
- Decision trees can be prone to overfitting if the tree is not pruned correctly.
- It can be difficult to handle continuous features that have many possible values.

## Results

### Confusion Matrix

![](./Confusion%20Matrix.png)

### Classification Report

|              | precision | recall | f1-score | support |
| ------------ | --------- | ------ | -------- | ------- |
| 1            | 0.96      | 0.94   | 0.95     | 175     |
| 2            | 0.95      | 0.95   | 0.95     | 167     |
| 3            | 0.89      | 0.96   | 0.92     | 138     |
| 4            | 0.98      | 0.95   | 0.96     | 182     |
| 5            | 0.98      | 0.92   | 0.95     | 143     |
| 6            | 0.97      | 0.99   | 0.98     | 148     |
| 7            | 0.94      | 0.96   | 0.95     | 167     |
|              |           |        |          |         |
| accuracy     |           |        | 0.95     | 1120    |
| macro avg    | 0.95      | 0.95   | 0.95     | 1120    |
| weighted avg | 0.95      | 0.95   | 0.95     | 1120    |

### Code can be found [HERE](/main_1%20-%20Decision%20Tree.ipynb)
