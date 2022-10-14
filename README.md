# Neural_Network_Charity_Analysis

## Overview of the analysis
This repository includes code to determine whether organiztions will be successfully funded or not by Alphabet Soup using Nerual Netowrk models. This machine learning model is designed using Tensorflow and Keras and written on Jupyter Notebook.

## Results

### Data Processing

- What variable(s) are considered the target(s) for your model?

Since the goal is to determine if an application is approved or not, the only target (y) variable is the "IS_SUCCESSFUL" column of our dataframe.

- What variable(s) are considered to be the features for your model?

Most of the columns are considered feature columns. These featured columns would have to be encoded prior to ruuning the machine learning model.

- What variable(s) are neither targets nor features, and should be removed from the input data?

The original "EIN" and "NAME" columns do not provide any meaningful insights to the output, therefore they should be removed.

### Compiling, Training, and Evaluating the Model

- How many neurons, layers, and activation functions did you select for your neural network model, and why?

The original designed Neural Network had 2 hidden layers (80 nodes for first layer and 30 for output layer) and obtained the following results:


- Were you able to achieve the target model performance?

The orginal and modified neural networks did acheive the desired 75% accuracy. 

- What steps did you take to try and increase model performance?

Adding layer, neurons, changing activation functions did not help much as the output accuracy was never able to pass 75%.

## Summary

