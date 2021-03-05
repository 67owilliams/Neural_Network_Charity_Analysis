# Neural_Network_Charity_Analysis

## Overview of Analysis:

The purpose of this analysis was to help AlphabetSoup find out if which donation recipients are worth investment and which are too high risk, by creating a neural network that will evaulate inputs and determine which organization should recieve donations.

## Results:

#### Data Preprocessing
* The variable considered to be the target in this situation is "IS_SUCCESSFUL". 
* Variables considered to be features include "APPLICATION_TYPE", "AFFILAIATION", "CLASSIFICATION", "USE_CASE", "ORGANIZATION", "INCOME_AMT", "SPECIAL_CONSIDERATIONS".
* Variables considered to be neither and should be removed are "EIN", "NAME", "STATUS", and "ASK_AMT".

#### Compiling, Training, and Evaluating the Model
* The structure of the model I chose had three hidden layers. The first hidden layer had thirteen nodes and had the "ReLu" activation method. The second layer had five nodes and used the "ReLu" activation method. The third layer had a single node and also used the "ReLu" activation method. The final output layer used the "Sigmoid" activation method.
* I was not able to achieve the desired target performance of 75%. THe closest I was able to achieve was 61%
![Accuracy.png](https://github.com/67owilliams/Neural_Network_Charity_Analysis/blob/main/accuracy.png)
* To attempt to optimise the model perforamnce the "IS_SUCCESSFUL", "EIN", "NAME", "STATUS", and "ASK_AMT" columns were dropped. I also added a third hidden layer.

## Summary:
My model after optimization was able to predict if a potential recpient would be sucessful with 61% accuracy. A model to include that would help classification would be one that determined how likely a busniess would be to "disappear" next actually being successful.
