# Iris-Flower-Classification---ANN-Model

## Overview

This project uses the classic Iris dataset and applies a neural network to predict flower species from four numerical features:

- Sepal length
- Sepal width
- Petal length
- Petal width

The workflow includes data loading, preprocessing, model training, evaluation, and saving the trained model for future use [file:11].

## Objectives

- Build an ANN-based multiclass classification model.
- Preprocess and standardize the input features.
- Train and evaluate the model on the Iris dataset.
- Save the trained model and scaler for reuse.
- Predict the species of unseen Iris samples [file:11].

## Dataset

The project uses the Iris dataset from `sklearn.datasets.load_iris`, which contains 150 samples and 4 input features across 3 classes [file:11].

### Classes
- Setosa
- Versicolor
- Virginica

## Project Workflow

1. Load the Iris dataset.
2. Create a pandas DataFrame.
3. Check for missing values and duplicates.
4. Separate input features and target labels.
5. Encode the target labels.
6. Standardize the feature values.
7. Split the dataset into training and testing sets.
8. Build an ANN model using TensorFlow/Keras.
9. Train the model.
10. Evaluate performance on the test set.
11. Generate predictions for unseen samples.
12. Save the model and scaler [file:11].

## Model Architecture

The ANN model is built using a simple feedforward architecture with:

- Input layer for 4 features.
- Hidden layer with 10 neurons and ReLU activation.
- Hidden layer with 8 neurons and ReLU activation.
- Output layer with 3 neurons and softmax activation [file:11].

## Training Details

- Optimizer: Adam
- Loss function: Categorical Crossentropy
- Metric: Accuracy
- Batch size: 8
- Epochs: 50
- Validation split: 0.2 [file:11]

## Results

The model achieved strong performance on the test set, with an accuracy of **93.33%** and a classification report showing high precision and recall across all three classes [file:11].

### Example Prediction

For the sample flower:

- Sepal length: 5.8
- Sepal width: 2.7
- Petal length: 5.1
- Petal width: 1.9

The model predicted the species as **Virginica** [file:11].

## Files Saved

- `iris_ann_model.keras` — trained ANN model.
- `scaler.pkl` — fitted StandardScaler object [file:11].

## Requirements

- Python 3.x
- NumPy
- Pandas
- Scikit-learn
- TensorFlow
- Joblib

Install dependencies with:

```bash
pip install numpy pandas scikit-learn tensorflow joblib
```

## Usage

### Train the model
Run the notebook or script to:
- preprocess the data,
- train the ANN,
- evaluate the model,
- save the model and scaler [file:11].

### Make predictions
Load the saved model and scaler, then preprocess new flower measurements before predicting the species.

## Project Structure

```bash
.
├── Iris-Classification-ANN-Iris-model.ipynb
├── iris_ann_model.keras
├── scaler.pkl
└── README.md
```

## Conclusion

This project demonstrates how an ANN can be used for multiclass classification on the Iris dataset. With proper preprocessing and a compact neural network, the model learns to distinguish flower species effectively and can be reused for future predictions [file:11].
