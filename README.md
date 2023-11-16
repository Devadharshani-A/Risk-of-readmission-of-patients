# Risk-of-readmission-of-patients

# Project: Hospital Readmission Prediction

## Introduction

This project aims to predict the risk of hospital readmission for patients after they are discharged from a hospital. The project utilizes a dataset containing patient records with information such as demographics, medications, diagnoses, and other relevant clinical data.

## Dataset

The project uses a dataset named "diabetic_data.csv" which contains a variety of independent variables and a dependent variable "readmitted" with three categories: No readmission, readmission in less than 30 days, and readmission in more than 30 days. 

## Code Description

The project's code is written in Python and is organized into several sections. Here is a summary of the key components:

## Data Import and Preprocessing:

Imports necessary libraries
Loads the dataset
Performs initial data analysis
Feature Engineering:

Handles missing values and irrelevant columns
Creates new features like "service_utilization" and "numchange"
Replaces and categorizes values in various columns
Converts categorical variables to binary numeric values

## Data Visualization:

Visualizes data using matplotlib and seaborn
Handling Diagnosis Codes:

Consolidates diagnosis codes into nine disease categories
Assigns numeric values to primary diagnosis codes

## Data Reduction:

Handles cases where patients have multiple encounters
Deduplicates records
Consolidates multiple encounters into a single representation
Calculates average duration and medication changes

## Target Variable Encoding:

Encodes the dependent variable "readmitted" into three categories

## Model Architecture:

Utilizes a Sequential model, which is a linear sequence of neural network layers.
The first layer is a dense layer with 64 units and a ReLU activation function.
Subsequently, a second dense layer with 32 units and a ReLU activation function is added.
Finally, a dense layer with a single unit and a sigmoid activation function is used to produce binary classification results.

## Model Compilation:

Compiles the model using the Adam optimizer.
Employs the binary_crossentropy loss function, which is well-suited for binary classification tasks.
Selects accuracy as a metric to monitor during training.
## Model Training:

Trains the model on the training data for 30 epochs.
Uses a batch size of 32.
Monitors the model's performance on the validation data.

## Model Evaluation:

Evaluates the model using the test data.
Computes both the loss and accuracy.
Prints the accuracy of the model on the test data, which is obtained as 88%.

## Conclusion

The project successfully implements a machine learning model to predict hospital readmission risk with an accuracy of 88%. The code demonstrates the process of data preprocessing, feature engineering, model building, and evaluatio
