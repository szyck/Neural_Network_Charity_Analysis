# Neural_Network_Charity_Analysis
## Overview

Determine whether or not future funding from Alphabet Soup in numerous organizations will result in those organizations being successful. Data from ~34,000 organizations were used to create a binary classificaiton model using a neural network. 

## Results

### Initial Model
The data set was cleaned through the removal of the uneccessary 'EIN' and 'NAME' columns. All application types with <500 counts were placed into their own 'other' bin. These categories were encoded using OneHotEncoder. After these steps, the model was set up with 2 hidden layers. Both layers have 4 neurons with tanh and relu activation functions. The output layer has a sigmoid activation function. This resulted in a 72.9% accuracy.

### Optimization
In addition to our initial cleaning of the data, the 'STATUS' column was removed. The model has an additional hidden layer. The first layer has 8 neurons with a tanh activation function. The second and third layers also have 8 layers but with a relu activation function. This resulted in a accuracy of 73.2%, whicn improves on the initial model

## Summary

The model does not succeed in predicting success correctly above a 75% accuracy rate. Perhaps the large number of variables caused the model difficulty in its task to maximize accuracy.
