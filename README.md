# Neural_Network_Charity_Analysis
## Overview

The purpose of this project is to use deep-learning neural networks with the TensorFlow platform in Python, to analyze and classify the success of charitable donations.
The following methods were used for the analysis:
1. preprocessing the data for the neural network model
2. compile, train and evaluate the model
3. optimize the model.

## Results
### Data Preprocessing

The columns EIN and NAME are identification information and have been removed from the input data.
The column IS_SUCCESSFUL contains binary data refering to weither or not the charity donation was used effectively. This variable is then considered as the target for our deep learning neural network.
The following columns APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, and SPECIAL_CONSIDERATIONS are the features for our model.
Encoding of the categorical variables, spliting into training and testing datasets and standardization have been applied to the features.

### Compiling, Training, and Evaluating the Model

This deep-learning neural network model is made of two hidden layers with 80 and 30 neurons respectively. The input data has 43 features and 25,724 samples.
The output layer is made of a unique neuron as it is a binary classification. To speed up the training process, we are using the activation function ReLU for the hidden layers. As our output is a binary classification, Sigmoid is used on the output layer. 
The model accuracy is under 75%. This is not a satisfying performance to help predict the outcome of the charity donations.
An attempt was made to modify neurons, layers, and activation features but all were unsuccesful as accuraacy remained under 75%

## Summary
The Target level of 75% is not extreme or strenuous, thus we can assume that the model is not effective at achieving it's stated goal. Perhapsa migrating the current model over to a supervised machine learning framework would yield a greater result. If this model is to remain in an unsupervised format it has become obvious that the work done here requires a substantial reimagining. 
