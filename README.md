# Mercedes-Benz Manufacturing Prediction

This repository contains a Python script that uses machine learning to predict the time a car will spend on the test bench based on various features, as part of the Mercedes-Benz Greener Manufacturing challenge on Kaggle.

## Setup

1. Clone this repository to your local machine.
2. Install the necessary Python packages. This project requires `numpy`, `pandas`, `scikit-learn`. You can install these with pip:

```sh
pip install numpy pandas scikit-learn
```

## Data

The data used for this project is provided by Mercedes-Benz and contains features related to a car and the target variable is the time (in seconds) that the car spends on the test bench. The data consists of a training set and a test set.

## Preprocessing

The data is preprocessed by:
- Dropping the outliers from the training set.
- Dividing the data into features (X) and the target variable (y).
- Splitting the training data into a training set and a validation set.
- Performing ordinal encoding on the categorical features.
- Handling missing values by imputing the median.
- Scaling the features using Standard Scaler.
- Selecting the top features using mutual information regression.

## Model

The model used for this project is a Linear Regression model from the `scikit-learn` library. The model is trained on the preprocessed training set, and it is used to predict the target variable on the training set, validation set, and the test set.

## Evaluation

The performance of the model is evaluated using the R squared metric.

## Submission

The predictions made by the model on the test set are saved to a CSV file for submission to the Kaggle competition.

## Usage

To use this model, run the included Python script. The script includes code for importing the data, preprocessing the data, training the model, making predictions, and exporting the predictions to a CSV file.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
```
