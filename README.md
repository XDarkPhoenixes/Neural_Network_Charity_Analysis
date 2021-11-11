# Neural_Network_Charity_Analysis

## Purpose
 Using machine learning and neural networks and the features in the provided dataset to create a binary classifier that is capable of predicting whether applicants will be successful if funded by a nonprofit philanthropic foundation Alphabet Soup. 

## Results

### Data Preprocessing.

- Variable that is considered the target for the model is the IS_SUCCESSFUL column, this column shows whether the fund is used effectively for each organization.

- Variables that are considered to be the features for the model include Alphabet Soup application type, affiliated sector of industry, government organization classification, the use case for funding, organization type, active status, income classification, Special consideration for application, and funding amount requested. 

- Variables such as EIN and NAME were used for identification purposes therefore neither targets nor features. They should be removed from the input data. 

### Compiling, Training, and Evaluating the Model
The initial model with two hidden layers had a predictive accuracy of 70% which is decent. 

In order to increase model performance, a few additional columns were removed including ASK_AMT(Funding amount requested) and INCOME_AMT(income classification). Those variables are suspected to be confusing the model. Furthermore, the activation functions in the hidden layer were changed to 'sigmoid'. Lastly, a third hidden layer was added to the model. 

The model that shows the most promising result had three hidden layers, adding more layers didn't improve the result. There are 150 neurons in the first layer, 90 neurons in the second layer, and 30 neurons in the third layer. The number of neurons was selected through trial and error, with the goal of improving the model's performance. 

Although multiple attempts were made, the target of 75% predictive accuracy is not achieved. 

## Summary
The improved model's accuracy ended up being 71% which is only slightly higher than the initial model.

One of the ways to increase the accuracy of the model is of course by having more solid features and data. Using the Random Forest classifiers could also be an option in this case since a random forest model with a sufficient number of estimators and tree depth should be able to perform at a similar capacity to most deep learning models. Also, the random forest model has the advantage of being faster than neural networks and is able to train on large datasets.
