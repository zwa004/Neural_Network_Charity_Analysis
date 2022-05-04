# Neural_Network_Charity_Analysis

## Overview

## Results

### Data Preprocessing

* Target variables - IS_SUCCESSFUL contains data that is binary which indicates whether or not a donation for the charity was effectively used. 

* Features - AFFILIATION, CLASSIFCATION, ORGANIZATION, APPLICATION_TYPE, USE_CASE, ASK_AMT, SPECIAL_CONSIDERATIONS, INCOME_AMT, and STATUS are features for this model.

* Neither targets nor variables - columns NAME and EIN were removed because they are ID information and therefore not important.

### Compiling, Training, and Evaluating the Model

* Neural network specifics - The selected neural network contains two hidden layers with 80 and 30 neurons (respectively), with 43 features and 25,724 samples. ReLu was used as the activation function for the hidden layers while Sigmoid was used for the output layer. The optimizer was ada and binary_crossentropy was used for the loss function. 

* Performance - The initial model did not perform as desired since its accuracy was under 75%

* Attempting to increase performance - The ASK_AMT feature was bucketed and orgainized by intervals to improve the performance of the model. An additional layer of hidden neurons was also added. Tanh also was used as an activation function instead of the ReLu. However model performance remained under 75%. 

## Summary
This particular model underperformed with 72% accuracy for testing data. A nearest neighbor or random forest classifier supervised model may prove more effective. 
