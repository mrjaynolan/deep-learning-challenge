# Report on Neural Network Model for Alphabet Soup

## Overview of the Analysis
The purpose of this analysis was to build and optimize a neural network model to predict the success of organizations funded by Alphabet Soup. By identifying key predictors and processing the data accordingly, the model aims to accurately classify organizations that are likely to succeed.

## Results

### Data Preprocessing
- **Target Variable(s):**  
  - `IS_SUCCESSFUL`: This binary variable indicates whether an organization was successful (1) or not (0).
  
- **Feature Variable(s):**  
  - Variables related to the organization’s type, classification, use case, affiliation, income amount, and special considerations.
  
- **Removed Variables:**  
  - `EIN` and `NAME`: These columns were removed as they are identifiers and do not provide meaningful information for predicting success.

### Compiling, Training, and Evaluating the Model
- **Neurons, Layers, and Activation Functions:**
  - **Input Layer**: The model’s input layer received all the features after one-hot encoding and scaling.
  - **First Hidden Layer**: 80 neurons with ReLU activation function.
  - **Second Hidden Layer**: 30 neurons with ReLU activation function.
  - **Output Layer**: 1 neuron with Sigmoid activation function for binary classification.
  
- **Model Performance:**
  - The model achieved an accuracy of approximately **73%** on the test set, which is slightly below the target threshold of 75% accuracy.

- **Optimization Steps Taken:**
  - Adjusted the number of neurons in each hidden layer.
  - Experimented with adding and removing hidden layers.
  - Tried different activation functions in the hidden layers and adjusted the number of epochs.
  - Processed categorical variables to group rare occurrences into an "Other" category to reduce noise.

### Summary
The neural network model provided a reasonable level of accuracy in predicting the success of organizations, reaching a final accuracy of 73%. Although this falls short of the target 75%, the model still offers valuable insights. Further accuracy improvement could be challenging with this architecture. As an alternative, I recommend exploring a **Random Forest** or **Gradient Boosting Classifier**. These ensemble models handle categorical data well, can highlight feature importance, and might yield higher accuracy given the nature of the dataset.
