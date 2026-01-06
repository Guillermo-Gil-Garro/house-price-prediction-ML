# House Price Prediction using Machine Learning

End-to-end Machine Learning project focused on predicting house prices using Python.  
The project follows a structured Data Science workflow, from data integration and cleaning to model optimization and overfitting analysis.

---

## 📌 Project Overview

The goal of this project is to build and evaluate predictive models for housing prices based on multiple heterogeneous data sources.  
The emphasis is not only on achieving good performance, but on **methodological correctness**, **generalization**, and **interpretability of results**.

Key objectives:
- Apply a correct and reproducible Data Science pipeline.
- Avoid common pitfalls such as data leakage.
- Compare baseline and optimized models.
- Diagnose overfitting using quantitative evidence.

---

## 🗂️ Data

The project integrates multiple datasets related to housing information, including:
- Structural features of the houses.
- External scores or ratings associated with locations.
- Zone-level or contextual information.

The datasets are merged into a single analytical table after:
- Schema inspection.
- Consistency checks.
- Validation of joins and key relationships.

> Raw data files are not included in this repository.  
> The `data/` folder contains documentation describing the datasets and their role in the project.

---

## 🔍 Methodology

The project follows a strict and explicit Data Science workflow:

1. **Data Loading & Integration**
   - Merging multiple datasets into a unified structure.

2. **Data Cleaning & Quality Control**
   - Removal of duplicates.
   - Treatment of missing values using statistically appropriate strategies (median, mode).
   - Outlier handling based on distribution analysis and domain reasoning.

3. **Exploratory Data Analysis (EDA)**
   - Univariate and bivariate analysis.
   - Relationship analysis between predictors and target variable.
   - Identification and removal of redundant or non-informative features.

4. **Preprocessing**
   - Train/Test split performed before any transformation.
   - Encoding of categorical variables.
   - Feature scaling where appropriate.
   - All transformations fitted **only on training data** and applied to test data to prevent data leakage.

5. **Modeling**
   - Baseline linear model.
   - Non-linear ensemble model (Random Forest).

6. **Optimization & Diagnostics**
   - Feature selection based on model relevance.
   - Hyperparameter tuning using `GridSearchCV` with 5-fold cross-validation.
   - MAE selected as the optimization metric.
   - Explicit comparison of training, cross-validation, and test performance.

7. **Evaluation**
   - Final evaluation on a hold-out test set.
   - Comparison across multiple models.
   - Error analysis and interpretation.

---

## 🤖 Models

The following models are implemented and compared:

- **Linear Regression**
  - Used as a baseline to assess linear relationships.

- **Random Forest (Base Model)**
  - Non-linear ensemble model with default parameters.

- **Random Forest (Optimized)**
  - Hyperparameters tuned via cross-validation to improve generalization.

---

## 📊 Evaluation Metrics

Models are evaluated using:

- **MAE (Mean Absolute Error)** — primary optimization metric.
- **RMSE (Root Mean Squared Error)** — penalizes large errors.
- **R² Score** — proportion of variance explained.

Performance is compared across:
- Training set
- Cross-validation folds
- Test set

This allows a clear diagnosis of generalization vs. overfitting.

---

## 🧠 Key Takeaways

- More complex models do not necessarily generalize better.
- Cross-validation is essential for detecting overfitting early.
- Feature relevance can differ between linear and non-linear models.
- A well-structured pipeline is more valuable than marginal metric improvements.
- Model diagnostics are as important as final performance numbers.

---

## 🛠️ Tech Stack

- Python
- pandas
- numpy
- scikit-learn
- matplotlib
- seaborn
- Jupyter Notebook
