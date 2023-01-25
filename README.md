# Neural_Network_Charity_Analysis

## Overview of the analysis
This repository includes code to determine whether organiztions will be successfully funded or not by Alphabet Soup using Nerual Netowrk models. This machine learning model is designed using Tensorflow and Keras and written on Python using Jupyter Notebook.

## Results

### Data Processing

- What variable(s) are considered the target(s) for your model?

Since the goal is to determine if an application is approved or not, the only target (y) variable is the "IS_SUCCESSFUL" column of our dataframe.

- What variable(s) are considered to be the features for your model?

Most of the columns are considered feature columns. Among the feature columns we can find the following:

![image](https://user-images.githubusercontent.com/20058842/195754605-7d16680c-65f5-4701-b86a-88fa79d003c9.png)


These featured columns are encoded prior to ruuning the machine learning model.

- What variable(s) are neither targets nor features, and should be removed from the input data?

The original "EIN" and "NAME" columns do not provide any meaningful insights to the output, therefore they should be removed.

### Compiling, Training, and Evaluating the Model

- How many neurons, layers, and activation functions did you select for your neural network model, and why?

The original designed Neural Network had 2 hidden layers (80 nodes for first layer and 30 for output layer) and obtained the following results:

![image](https://user-images.githubusercontent.com/20058842/195754796-f5d625dc-c51f-4069-bdc7-1345f81dd734.png)

![image](https://user-images.githubusercontent.com/20058842/195754842-e172f8bf-cacb-4ff6-a82f-d82cea2b8196.png)

After running this initial model, the following neural network structures were tested:

**Attempt 1:**

![image](https://user-images.githubusercontent.com/20058842/195755139-f47d53e5-ab90-49e9-aa13-60b1021834f1.png)

![image](https://user-images.githubusercontent.com/20058842/195755182-c9ad7816-f653-4b87-b0e2-3eba61e83d81.png)

**Attempt 2:**

![image](https://user-images.githubusercontent.com/20058842/195755270-e491a388-a943-4f02-a5a3-1da322cc0a5c.png)

![image](https://user-images.githubusercontent.com/20058842/195755311-15752b63-eae7-48ff-a7ee-43f6358b374f.png)

**Attempt 3:**

![image](https://user-images.githubusercontent.com/20058842/195755391-d5c0fa97-9961-4eca-93c4-bf27697d1a4d.png)

![image](https://user-images.githubusercontent.com/20058842/195755426-9f076d26-4392-40e8-8ce5-fed3a7323b8c.png)

- Were you able to achieve the target model performance?

The orginal and modified neural networks did acheive the desired 75% accuracy. 

- What steps did you take to try and increase model performance?

Adding layer, neurons, changing activation functions did not help much as the output accuracy was never able to pass 75%.

## Summary

Since changing the network structure did not help (hidden layers, neurons, activation functions, and training epochs) it is to note that data being used might not be the best suited to achieve the accuarcy goal. It is recommended to try modifying this data, whether it's incrementing or decreseaing testing points, or modyfing the input features. It is also recommended to try other supervised learning algorithms such as logistic regression or SVM and compare the results to see what can work better.
