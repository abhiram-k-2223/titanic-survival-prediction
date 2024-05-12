# Titanic Survival Prediction

This repository contains code for predicting survival on the Titanic using logistic regression. The dataset used in this project is generated from this [repository](https://github.com/abhiram-k-2223/csv-making).

## Overview

The project consists of Python code implemented in a Jupyter notebook. The dataset is divided into three classes based on passenger class (Pclass 1, Pclass 2, Pclass 3). Logistic regression models are trained and tested for each class to predict survival based on features such as age and sex.

## Dependencies

- pandas
- scikit-learn

## Dataset Preparation

The dataset is divided into three CSV files: `pclass1.csv`, `pclass2.csv`, and `pclass3.csv`. Each file contains information about passengers in the respective class including features like sex, age, and survival status.

## Model Training

- For each class, the sex feature is converted to numerical values (0 for female, 1 for male) for compatibility with logistic regression.
- Missing values in the age column are filled with the mean age of the respective class.
- The dataset is split into training and testing sets.
- Features are standardized using `StandardScaler`.
- Logistic regression models are trained on the training data.
- Predictions are made on the testing data.
- Model accuracy is evaluated using the `accuracy_score` metric.

## Model Export

Trained models are exported using the `pickle` library and saved as `clf.pkl`, `model1.pkl`, and `clf2.pkl` for each class.

## Files

- `titanic_passenger_class.ipynb`: Jupyter notebook containing the Python code.
- `clf.pkl`, `model1.pkl`, `clf2.pkl`: Exported trained models.
- `pclass1.csv`, `pclass2.csv`, `pclass3.csv`: Dataset files.

## Usage

To run the code:

1. Clone the repository.
2. Ensure dependencies are installed.
3. Open and execute the `titanic_passenger_class.ipynb` notebook in a Python environment with Jupyter installed.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
