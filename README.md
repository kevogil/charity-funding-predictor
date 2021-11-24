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
Our goal was to optimize our model to achieve a target predictive accuracy higher than 75%. Three attempts were made with the following parameters and results:
* The first attempt 
<p>This resulted in 72.5% of the model's predictions aligning to the</p>

## Summary