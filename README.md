# House Price Prediction using Machine Learning

End-to-end Machine Learning project for predicting house prices using Python, with a strong focus on methodological correctness, generalization, and model evaluation.

## Project goal
The objective of this project is to build and compare predictive models for house prices using a structured Data Science workflow:
- integrating heterogeneous data sources,
- cleaning and validating the dataset,
- performing exploratory analysis,
- training baseline and non-linear models,
- and evaluating generalization performance carefully.

## What this project demonstrates
This repository showcases:
- data integration and preprocessing,
- careful train/test separation,
- prevention of data leakage,
- model comparison,
- hyperparameter tuning with cross-validation,
- and explicit overfitting diagnosis.

## Models used
- Linear Regression
- Random Forest (baseline)
- Random Forest (optimized with `GridSearchCV`)

## Evaluation approach
The models are evaluated using:
- `MAE`
- `RMSE`
- `R²`

Performance is compared across:
- training set
- cross-validation
- hold-out test set

This makes it possible to evaluate not only raw performance, but also whether the model generalizes well.

## Methodology summary
1. Data loading and integration  
2. Data cleaning and quality checks  
3. Exploratory Data Analysis  
4. Preprocessing after train/test split  
5. Baseline modeling  
6. Hyperparameter tuning  
7. Final evaluation and interpretation

## Repository contents
- `README.md` — project summary
- notebooks / scripts / supporting files used for the analysis and modeling
- data documentation or references where applicable

## Notes
- Raw datasets are not included in the repository.
- The project is focused on reproducibility, sound methodology, and interpretation rather than only maximizing a metric.

## Tech stack
- Python
- pandas
- numpy
- scikit-learn
- matplotlib
- seaborn
- Jupyter Notebook

## Why this project matters
A good ML project is not just about fitting a model.  
This repository emphasizes the part that matters most in real work: building a pipeline that is technically correct, interpretable, and able to generalize.

## Author
Guillermo Gil Garro
