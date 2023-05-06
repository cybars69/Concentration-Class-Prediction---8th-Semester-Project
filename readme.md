# Concentration Class Prediction

## Data Acquisition and Data Format

### Introduction

- The goal is to track the concentration of Troponin-I in blood. Troponin-I, or Troponins in general are a good indicator of cardiovascular diseases and myocardial infarctions.
- The main goal of this procedure was to detect and diagnose early instances of patients who might go through Acute Myocardial Infarction (AMI).

### Data Format and Acquisition

- While testing in the lab, we measure the ΔR/R value for 8-10 devices over a series of voltage values.
- The above process is repeated for 7 concentrations of Troponin-I in total with concentrations being constant for each iteration.
- At the end of this step, we have a 3-dimensional dataset that we need to process further.

## Data Pre-Processing

### Reading the Data from Disk

- We start with reading the data from the Excel Sheet which was generated in the above steps.
- The data is returned as a python dictionary which we will process further.

### Inferring the Statistics

- For each corresponding Voltage and Troponin concentration, we have a set of 8-10 devices which give us the ΔR/R values.
- Since the ΔR/R values are not sequential or dependent on other similar values for the same voltage and Troponin concentration, replacing the 8-10 generated data points with their corresponding statistical measures seems a better option.
- We have generated, for each set of devices under the same measures - median, mean and standard deviation - and excluded all the direct device measurements from the final data over which we will be training our models.

## Results

- The Algorithms and ML Models used in this project have all been linked below with their corresponding overall accuracies and within them are Precision, Recall and F1 Score included as well.

| Training Algorithm | Accuracy | Deployment Accuracy | Detailed Accuracy Reports                           |
| ------------------ | -------- | ------------------- | --------------------------------------------------- |
| KNN                | 92.6 %   | 88.6 %              | [More Details](./outputs/KNN/report.md)             |
| SVM                | 95.4 %   | 88.5 %              | [More Details](./outputs/SVM/report.md)             |
| Decision Tree      | 94.6 %   | 82.4 %              | [More Details](./outputs/Decision%20Tree/report.md) |
| Random Forest      | 97.2 %   | 89.6 %              | [More Details](./outputs/Random%20Forest/report.md) |
| XG Boost           | 94.9 %   | 85.3 %              | [More Details](./outputs/XG%20Boost/report.md)      |
| MLP                | 78.1 %   | NA                  | [More Details](./outputs/MLP/report.md)             |
