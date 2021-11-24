# Neural_Network_Charity_Analysis
Neural Network and Deep Learning Models


## Overview 
•	Create a binary classifier that can predict weather applicants will be successful if funded by Alphabet Soup based on the features in the dataset. 
•	Compile, train, and evaluate the binary classification model to calculate the model’s loss and accuracy.
•	By Using our knowledge of TensorFlow, optimize my model in order to achieve a target predictive accuracy higher than 75%. 

## Results: Using bulleted lists and images to support your answers, address the following questions.

###	Data Preprocessing
*	What variable(s) are considered the target(s) for your model?
column IS_SUCCESSFUL is the target of the model because it contains binary data referring to weather or not the charity donation was used effectively. 
* What variable(s) are considered to be the features for your model?
The following columns APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, ASK_AMT are the features for the model
* What variable(s) are neither targets nor features, and should be removed from the input data?
Columns EIN and NAME were identification information and were removed from the input data.

### Compiling, Training, and Evaluating the Model
* How many neurons, layers, and activation functions did you select for your neural network model, and why?
The model was made of two hidden layers with 80 and 30 neurons.
The input data has 43 features and 25,724 samples.
The output layer was made of a unique neuron 
To speed up the training process, we are using the activation function ReLU for the hidden layers. As our output is a binary classification, Sigmoid is used on the output layer.
For the compilation, the optimizer is adam and the loss function is binary_crossentropy.

* Were you able to achieve the target model performance?
The model accuracy is under 75%. Then it is not a good performance to predict the result of the charity donations.

*What steps did you take to try and increase model performance?
To increase the performance of the model, bucketing was applied to the feature ASK_AMT and organized the different values by intervals.
The number of neurons on one of the hidden layers, then a model with three hidden layers was used

## Summary
The learning neural network model did not reach the target of 75% accuracy. Then considering the accuracy of the model, it could be said that its performance is not significant. Therefore we can use a supervised learning model that help us combine different decisions such as Random Forest to  generate a classified output and evaluate the model's performance

