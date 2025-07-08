# IC50 Prediction Using Deep Learning

This project predicts the IC50 values (a measure of drug potency) using a neural network built in TensorFlow. Molecular data was taken from a CSV file containing SMILES representations, and features were extracted using RDKit to generate Morgan fingerprints. The model is trained to predict IC50 (in nM) using a feedforward neural network, and its performance is compared with Ridge Regression.

## Features
- Converts SMILES strings to molecular fingerprints using RDKit
- Trains a deep neural network on IC50 values
- Visualizes loss curves and prediction performance
- Compares predictions with Ridge Regression
- Exports predicted results to a CSV

## Requirements
- Python 3, NumPy, pandas, matplotlib, seaborn
- RDKit (`rdkit-pypi`)
- TensorFlow
- Scikit-learn
- Google Colab (for file upload widget)

## How to Use
1. Upload your `DataSet.csv` with SMILES and IC50 values in nM.
2. Run the notebook to process data, generate features, and train the model.
3. View training loss, prediction scatter plot, and save predictions to `IC50_Predictions.csv`.

## Output
- Training vs validation loss graph
- Predicted vs true IC50 scatter plot
- `IC50_Predictions.csv` with results

## Note
Large MSE values may indicate outliers or the need for data normalization. Further tuning is recommended for production use.

