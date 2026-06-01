# InternSpark-Internship
This repository is made for my submission of task/projects under InternSpark Internship

# Task 1 : Iris Classification


## Project Description
This project classifies Iris flowers into three species:
- Setosa
- Versicolor
- Virginica

The dataset used is the Iris Classification Dataset from Kaggle.

## Algorithms Used
1. Logistic Regression
2. K-Nearest Neighbors (KNN)
3. Decision Tree

The best-performing model was saved as 'iris_model.pkl'.

## Running the Notebook

open and run:

Iris_Classification.ipynb

## Inference Example
### python:
import pandas as pd

import joblib

model = joblib.load('iris_model.pkl')

scaler = joblib.load('scaler.pkl')

sample = [[5.1,3.5,1.4,0.2]]

sample = scaler.transform(sample)

prediction = model.predict(sample)

print("Predicted Species: ", encoder.inverse_transform(prediction)[0])

## Expected Output:

Iris-setosa.
