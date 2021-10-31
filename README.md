# Overview

In this analysis we used a neural network to determine which partner companies are worthy candidates for recieving donations from our non profit organization. We did this by taking many forms of data that was gathered from the partner comapnies, and processed it for our neural network. We then compiled and trained our model, and finally optomized it to give us the best accuracy possible.

# Results

### Q) What variable(s) are considered the target(s) for your model?

* The column "IS_SUCCESSFUL" is the target for this model as it defines whether or not the company is a candidate for donations

### Q) What variable(s) are considered to be the features for your model?

* APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, ASK_AMT are the features for our model.

### Q) What variable(s) are neither targets nor features, and should be removed from the input data?

* Identification columns such as EIN and NAME are not needed for the neural network

### Q) How many neurons, layers, and activation functions did you select for your neural network model, and why?

* This neural network model is made of two hidden layers with around 80 and 30 neurons. The input data has 43 features and 25,724 samples. To speed up the training process, we are using the activation function ReLU for the hidden layers. As our output is a binary classification, Sigmoid is used on the output layer.

### Q) Were you able to achieve the target model performance?

* Unfortunately the model could only achieve a 72-73% accuracy

### Q) What steps did you take to try and increase model performance?

* We applied bucketing to the feature ASK_AMT and organized the different values by intervals. We increased the number of neurons on one of the hidden layers, as well as used a model with 3 hidden layers. We also tried the activation function tanh, but none of these steps helped improve the model's performance.

# Summary

Overall our neural network model was not accurate enough to predict if a company was a good candidate to get a donation. Based on the project a recommendation I would have is using a supervised machine learning model since we are in a classification situation where we know the input and can generate a classified output. We could then evaluate the results and compare it to our model.
