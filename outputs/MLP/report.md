# Multilayer Perceptron <b>(MLP)</b>

It is a feedforward neural network used for classification and regression tasks. It consists of multiple layers of nodes or neurons, where each neuron is connected to the neurons in the previous and next layers.

## Working and details

### Working of MLP

1. Input data is fed into the input layer.
1. The input is transformed by passing through one or more hidden layers with nonlinear activation functions.
1. The output is produced by the output layer, which can be a single node for regression or multiple nodes for classification.
1. The model is trained using backpropagation, where the weights of the connections between the neurons are adjusted to minimize the error between the predicted and actual outputs.

### Pros of using MLP

- MLP can handle non-linear relationships between features and target variables.
- It can perform well on a wide range of datasets, even when the data is noisy or complex.
- MLP can be used for both classification and regression tasks.
- It can learn complex decision boundaries and capture interactions between features.

### Cons of using MLP

- MLP can be sensitive to the choice of activation function, number of hidden layers, and number of neurons in each layer, requiring careful tuning.
- It can be prone to overfitting if the model is too complex or the dataset is small.
- MLP can be computationally expensive and slow to train, especially when dealing with large datasets.
- It can be difficult to interpret the learned model and understand the contribution of individual features to the classification or regression.

## Results

### Accuracy Plot

![](./Accuracy.png)

### Loss Plot

![](./Loss.png)

### Confusion Matrix

![](./Confusion%20Matrix.png)

### Classification Report

|              | precision | recall | f1-score | support |
| ------------ | --------- | ------ | -------- | ------- |
| 1            | 0.00      | 0.00   | 0.00     | 402     |
| 2            | 0.51      | 0.95   | 0.66     | 406     |
| 3            | 0.92      | 0.97   | 0.94     | 412     |
| 4            | 0.97      | 0.95   | 0.96     | 396     |
| 5            | 0.71      | 0.97   | 0.82     | 399     |
| 6            | 0.93      | 0.72   | 0.81     | 383     |
| 7            | 0.97      | 0.90   | 0.93     | 402     |
|              |           |        |          |         |
| accuracy     |           |        | 0.78     | 2800    |
| macro avg    | 0.72      | 0.78   | 0.73     | 2800    |
| weighted avg | 0.71      | 0.78   | 0.73     | 2800    |

### Code can be found [HERE](/main_1%20-%20MLP.ipynb)
