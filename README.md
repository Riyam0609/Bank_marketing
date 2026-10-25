# End-to-End Machine Learning Banking Domain Project

This repository contains an end-to-end machine learning project focused on predicting whether a client will subscribe to a bank term deposit based on marketing campaign data. The project uses a real-world banking dataset and demonstrates the full workflow from data preprocessing to model training, validation, and saving the final trained pipeline.

## Project Overview

Bank marketing campaigns often rely on identifying the most promising leads among prospective clients. This project builds a machine learning model that predicts whether a customer is likely to subscribe to a term deposit after being contacted by the bank.

The workflow includes:
- Data loading and exploration
- Feature engineering and preprocessing
- Train/validation/test splitting
- Model comparison and selection
- Saving model artifacts for reuse
- A notebook-based implementation for end-to-end experimentation

## Repository Structure


.
├── Bank Marketing.ipynb        # Main notebook with exploratory analysis and modeling
├── bank-additional-full.csv    # Raw dataset used for model training
├── df_train.csv                # Training dataset after preprocessing/splitting
├── df_valid.csv                # Validation dataset
├── df_test.csv                 # Test dataset
├── df_train_all.csv            # Full training data/combined data
├── df_mean.csv                 # Summary statistics or feature means
├── best_classifier.pkl         # Best trained classifier model
├── scaler.sav                 # Saved scaler for preprocessing
├── cols_input.sav              # Input feature columns used in the pipeline
├── .ipynb_checkpoints/         # Jupyter notebook checkpoint files


## Dataset

The project uses the Bank Marketing dataset, typically based on the "bank-additional-full.csv" file, which contains customer information and campaign-related features such as:

Age
Job
Marital status
Education
Housing loan status
Personal loan status
Contact communication type
Previous campaign outcomes
Economic indicators
Subscription target variable

The target is whether the client subscribed to a term deposit (yes / no).

## Objective

Predict whether a client will subscribe to a term deposit using customer and campaign data, enabling better targeting and decision-making for marketing teams.

## Tools and Libraries

This project is implemented in Python and is likely built using libraries such as:

pandas
numpy
scikit-learn
matplotlib / seaborn
joblib / pickle
Jupyter Notebook


## Workflow

The project follows a standard machine learning lifecycle:

Load the bank marketing dataset.
Inspect and clean the data.
Encode categorical variables and scale numerical features.
Split the data into train/validation/test sets.
Train and compare candidate classifiers.
Select the best-performing model.
Save the trained model and preprocessing artifacts.
Use the model for prediction tasks.


## Model Artifacts

The repository contains saved pipeline components:

best_classifier.pkl — best-performing trained model
scaler.sav — feature scaling object
cols_input.sav — list of input features used by the model
These artifacts can be reused for inference without retraining.


## Conclusion

This project demonstrates a practical machine learning pipeline for a banking campaign use case, converting raw customer data into a predictive model that helps optimize marketing outreach and improve decision-making.




