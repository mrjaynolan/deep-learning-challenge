# Alphabet Soup Charity Model

This project creates and optimizes a neural network model to predict the success of organizations funded by Alphabet Soup. The model uses various organizational features to identify potential success, helping Alphabet Soup make data-driven funding decisions.

## Project Overview

The goal of this analysis is to build, train, and optimize a binary classification model using TensorFlow to predict whether an organization funded by Alphabet Soup will be successful. The project includes the following steps:
1. **Data Preprocessing**: Preparing and cleaning the data.
2. **Model Compilation, Training, and Evaluation**: Building the neural network model, training it on the preprocessed data, and evaluating its performance.
3. **Model Optimization**: Attempting various optimization techniques to reach a target accuracy of 75% or higher.
4. **Model Export and Report Writing**: Exporting the model to an HDF5 file and summarizing findings in a report.

## Table of Contents

- [Project Overview](#project-overview)
- [Technologies Used](#technologies-used)
- [File Descriptions](#file-descriptions)
- [Installation](#installation)
- [Usage](#usage)
- [Results](#results)
- [Contact](#contact)

## Technologies Used

- Python
- TensorFlow
- scikit-learn
- Pandas
- Google Colab (for model training)

## File Descriptions

- **charity_data.csv**: The dataset containing organizational details and success indicators.
- **Starter_Code.ipynb**: The initial notebook template for the project.
- **AlphabetSoupCharity.h5**: The saved neural network model file.
- **AlphabetSoupCharity_Optimization.h5**: The optimized version of the neural network model.

## Usage

### Data Preprocessing
- Load and clean the data, identify target and feature columns, and drop unnecessary columns.
- Convert categorical data into numerical values using one-hot encoding.
- Scale features using `StandardScaler` to prepare them for training.

### Model Compilation, Training, and Evaluation
- Define a neural network with two hidden layers using TensorFlow.
- Train the model on the training set and validate on the test set.
- Export the trained model to `AlphabetSoupCharity.h5`.

### Model Optimization
- Experiment with additional layers, different activation functions, and tuning the number of neurons and epochs to improve accuracy.
- Export the optimized model to `AlphabetSoupCharity_Optimization.h5`.

### Report Writing
- Summarize findings, including model structure, performance metrics, and optimization attempts.

## Results

- **Accuracy**: The initial model achieved approximately 73% accuracy. Optimization efforts, including additional layers and tuning parameters, aimed to reach a target accuracy of 75%.
- **Alternative Model Suggestions**: Based on the data characteristics, an ensemble model such as Random Forest or Gradient Boosting could be a suitable alternative, potentially yielding higher accuracy for this classification task.


