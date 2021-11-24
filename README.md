# Charity Funding Predictor

## Overview
The purpose of this project is to evaluate whether machine learning and neural networks could be used to help predict whether applicants will successfully be funded by the non-profit foundation, Alphabet Soup.

## Preprocessing the data
The dataset used for the evaluation consists of 34,000 organizations that have received funding from Alphabet Soup over the years.
The following steps were taken to prepare the dataset:
* The 'EIN' and 'NAME' columns were dropped as they did not contain information that would be relevant features for the model.
* Application types with less than 500 counts were binned into an `Other` category to reduce potential variance.
* Classifications with less than 1,000 counts were binned into an `Other` category to reduce potential variance.
* All categorical data were converted to numeric values.
* The dataset was split into a training and testing subsets.

## Results
Our goal was to optimize our model to achieve a target predictive accuracy higher than 75%. Four attempts were made with the following parameters and results:
1. The first attempt was a neural network with the following hyperparameters:
    <ul>Number of hidden layers: 2</ul>
    <ul>Activation function: Relu (all 2 layers)</ul>
    <ul>Neurons: 8 units in 1st layer, 5 units in 2nd layer</ul>
    <ul>Output function: Sigmoid</ul>
    <ul>Epochs: 100</ul>

    This resulted in 72.8% of the model's predictions aligning to the true values.

2. The second attempt was also a neural network with the following hyperparameters:
    <ul>Number of hidden layers: 3</ul>
    <ul>Activation function: Relu (all 3 layers)</ul>
    <ul>Neurons: 16 units in 1st, 10 units in 2nd, 8 units in 3rd</ul>
    <ul>Output function: Sigmoid</ul>
    <ul>Epochs: 200</ul>
    
    This resulted in 72.5% of the model's predictions aligning to the true values.

3. The third attempt was also a neural network with the following hyperparameters:
    <ul>Number of hidden layers: 3</ul>
    <ul>Activation function: Relu (1st 2 layers), Tanh (3rd layer)</ul>
    <ul>Neurons: 16 units in 1st, 10 units in 2nd, 8 units in 3rd</ul>
    <ul>Output function: Sigmoid</ul>
    <ul>Epochs: 200</ul>
    
    This resulted in 72.4% of the model's predictions aligning to the true values.

## Summary