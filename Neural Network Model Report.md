# Neural Network Model Report

1. Overview 

The purpose of this analysis was to create a tool that can help the Alphabet Soup foundation to select applicants for funding that have the best chance of success in their ventures. Machine learning and neural networks were used to create a binary classifier that can predict whether applicants will be successful or not if funded by Alphabet Soup.

2. Results

Data Processing

- Target variable
    - IS_SUCCESSFUL
- Feature variables
    - APPLICATION_TYPE
    - CLASSIFICATION
    - USE_CASE
    - ORGANIZATION
    - INCOME_AMT
    - ASK_AMT
- Variables that were removed
    - EIN
    - NAME

Compiling, Training, and Evaluating the Model

Three attempts at optimizing the model were made in order to achieve a target predictive accuracy higher than 75%.

1st Attempt - an extra hidden layer was added
- 3 hidden layers
    - 1st hidden layer - 80 nodes, activation - relu
    - 2nd hidden layer - 30 nodes, activation - relu
    - 3rd hidden layer - 10 nodes, activation - relu
    - 100 epochs
- this attempt achieved a predictive accuracy of 72.84%

2nd Attempt - a different activation function was used 
- 3 hidden layers
    - 1st hidden layer - 80 nodes, activation - tanh
    - 2nd hidden layer - 30 nodes, activation - tanh
    - 3rd hidden layer - 10 nodes, activation - tanh
    - 100 epochs
- this attempt achieved a predictive accuracy of 72.93%

3rd Attempt - more epochs were added to the training regimen
- 3 hidden layers
    - 1st hidden layer - 80 nodes, activation - relu
    - 2nd hidden layer - 30 nodes, activation - tanh
    - 3rd hidden layer - 10 nodes, activation - tanh
    - 200 epochs
- this attempt achieved a predictive accuracy of 73%

3. Summary
   
Overall this neural network model achieved a predictive accuracy of 73% which is lower than the desired 75%. Even with adding more layers and changing the activation functions and increasing epochs the model did not achieve higher accuracy. A different model where the feature variables have been changed and more data added might result in a higher accuracy.








