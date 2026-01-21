##Titanic Machine Learning Pipeline (MLOps Practice)

This project demonstrates a clean, script-based machine learning pipeline built using the Titanic dataset.
It focuses on reproducibility, modular design, and MLOps-oriented structure, moving beyond notebook-only experimentation.

##Project Overview

The goal of this project is to predict passenger survival on the Titanic using supervised machine learning.
Unlike exploratory notebook-only projects, this repository emphasizes:

Modular data loading and preprocessing

Script-driven training pipeline

Clear separation of concerns

Production-ready project structure

##Dataset

Dataset: Titanic dataset (Seaborn)

Target variable: survived

Selected features:

pclass

sex

age

sibsp

parch

fare

Preprocessing Steps

Removed missing values

Encoded categorical variable:

male → 1

female → 0

# #Project Structure
ML_in_practice/
│
├── src/
│   ├── train_and_evaluate.py   # Training pipeline script
│   ├── utils.py                # Utility/helper functions
│
├── model/
│   ├── titanic_model.pkl       # Trained ML model
│   ├── scaler.pkl              # Feature scaling artifact
│
├── Notebooks/
│   ├── Titanic ML Model Pipeline v1_user input.ipynb
│   ├── Titanic ML Model Pipeline v2_Streamlit.ipynb
│
├── requirements.txt
├── README.md

## Training Pipeline

The entire ML workflow is handled by a standalone Python script:

src/train_and_evaluate.py

Pipeline Flow

Load dataset using Seaborn

Select relevant features

Clean and preprocess data

Split features (X) and target (y)

Train and evaluate the model

Save trained artifacts for reuse

## How to Run
 Install Dependencies
pip install -r requirements.txt

 Run the Training Pipeline
python src/train_and_evaluate.py

 Sample Output
Training pipeline started
Data loaded (714, 6)
Pipeline executed successfully

#3 Why This Project Matters

This repository showcases:

 Transition from notebooks → reproducible scripts

 MLOps-ready structure

 Clean data preprocessing pipeline

 Model artifact versioning

 Industry-style logging and execution flow

## Future Improvements

Planned enhancements include:

Model evaluation metrics (accuracy, ROC-AUC, confusion matrix)

Hyperparameter tuning

Cross-validation

CI/CD integration

Model inference API (FastAPI / Streamlit)

Experiment tracking (MLflow)

## Author

Aayushi Shekhat
AI / ML | Data Science | MLOps Enthusiast
