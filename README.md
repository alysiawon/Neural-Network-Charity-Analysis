# Neural-Network-Charity-Analysis

## Overview of Analysis

This analysis will focus on creating a deep learning neural network model to predict which foundations are worth donating to and which are too high risk. In this analysis, we will test and optimize our models to determine which charities to invest in.

### Results

## Data Preprocessing

**What variable(s) are considered the target(s) for your model?**

The variable that is considered the target for the model is the "IS_SUCCESSFUL" column.

**What variable(s) are considered to be the features for your model?**

Every column minus the "IS_SUCCESSFUL" column is a feature in the model. 

**What variable(s) are neither targets nor features, and should be removed from the input data?**

The varibales that are neither a target or feature is the "EIN" and "Name" columns which are dropped. They do not provide any signficiant value to the model.

### Compiling, Training, and Evaluating the Model

**How many neurons, layers, and activation functions did you select for your neural network model, and why?**

The neural network model has 2 hidden layers with the first layer having 80 neurons and the second layer is the outer layer having 30 neurons. The first and second hidden layer have the "RELU" activation function and the activation function for the output layer is "Sigmoid."

**Were you able to achieve the target model performance?**

The model was not able to reach the target 75%. This is the result of the three attempts:

First Model: 69.9%

Optimization Model:
- Attempt 1: 53.3%
- Attempt 2: 53.3%
- Attempt 3: 47.8%

**What steps did you take to try and increase model performance?**

Attempt 1: Removed the 'USE_CASE' column and kept therest of the model components the same.

Attempt 2: Adding additional neurons to hidden layers and additional hidden layers are added.

Attempt 3: Changing activation function of output layer from "Sigmoid" to "Tanh." 

## Summary

The initial neural network model had an accuracy score of 69.9%. After optimization, the accuracy score of the model dropped to 47.8%. After the test, we can recommend that additional optimization is required. This can include removingn features or adding additional data to the dataset to increase accuracy.
