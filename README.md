# 6001CMD – Hotel Booking Demand Machine Learning Analysis

## Project Overview

This project investigates the Hotel Booking Demand dataset using machine learning techniques. The analysis focuses on predicting whether a hotel booking will be cancelled based on information associated with the booking.

The project evaluates the machine learning problem, compares supervised and unsupervised learning paradigms, investigates data quality issues, and develops and evaluates a preprocessing strategy.

## Dataset

**Dataset:** Hotel Booking Demand

**Dataset Source:** Kaggle

**Dataset URL:**  
https://www.kaggle.com/datasets/jessemostipak/hotel-booking-demand

The original Hotel Booking Demand dataset contains 119,390 booking records and 32 variables covering hotel bookings from two hotel properties.

### Target Variable

The target variable is:

- `is_canceled` – indicates whether a booking was cancelled.
  - `0` = Not cancelled
  - `1` = Cancelled

Therefore, the machine learning problem is formulated as a **binary classification problem**.

## Project Objectives

The objectives of this project are to:

1. Formulate the hotel booking cancellation problem as a machine learning problem.
2. Compare supervised and unsupervised learning approaches for the dataset.
3. Critically investigate the quality of the dataset.
4. Design and evaluate an appropriate preprocessing pipeline.
5. Investigate data cleaning, transformation, feature engineering, dimensionality reduction, encoding and data balancing techniques.
6. Evaluate the effect of preprocessing and balancing strategies on model performance.

## Dataset Characteristics

The original dataset contains:

- 119,390 records
- 32 variables
- Numerical and categorical features
- A binary target variable
- Missing values
- Duplicate records
- Skewed numerical variables
- Extreme values and invalid ADR values
- Class imbalance

## Machine Learning Approach

The project uses supervised machine learning because the dataset contains a labelled target variable, `is_canceled`.

The main modelling approach uses Logistic Regression with a preprocessing pipeline implemented using Python and scikit-learn.

## Data Preprocessing

The preprocessing investigation includes:

- Removal of data leakage variables
- Duplicate removal
- Missing-value treatment
- Invalid ADR treatment
- Feature engineering
- Numerical standardisation
- Categorical encoding
- SMOTE class balancing
- PCA dimensionality reduction
- Evaluation of alternative transformation techniques

The final preprocessing pipeline uses a combination of numerical imputation and standardisation together with categorical imputation and one-hot encoding.

## Model Evaluation

Model performance is evaluated using:

- Accuracy
- Precision
- Recall
- F1-score
- Confusion matrix

SMOTE was also evaluated to investigate its effect on the minority cancellation class.

## Project Structure

```text
6001CMD-Hotel-Booking-Machine-Learning/
│
|-- README.md
│
|-- Hotel_Booking_ML_Analysis.ipynb
