# Deep Learning Challenge

## Overview
The purpose of this model is to determine is the charity, Alphabet Soup utilizes their funding in an efficient manner.

## Results

### Pre-Processing

- The target variable for the model is IS_SUCCESSFUL,"which indicates if Alphabet Soup uses their funding efficiently.
- The feature variables are the columns that capture metadata about each organization.
- EIN and NAME can be removed from the input data as they add predictive capability to the model.

### Compiling, Training, and Evaluating the Model

- Layer 1: 80 neurons, relu activation
 Layer 2: 30 neurons, relu activation
Output Layer: sigmoid activation

- The model was only able to reach 69% accuracy, missing the target of 75%. 

- Attempts to improve performance:

1. Removed additional feature ('USE_CASE' column). The accuracy decreased to 63%.
2. Adding neurons to hidden layers and added hidden layers. The accuracy decreased to 53%.
3. Updateing activation function of output layer from "sigmoid" to "tanh." The accuracy decreased to 50%.

## Summary
Overall the initial model had the best results in terms of accuracy. One issue that may have affected the accuracy of the models is overfitting. In order to mitigate this issue, I would conside using a random forest model.
