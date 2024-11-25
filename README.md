# Project Overview

This project aims to predict and classify energy consumption data using machine learning models. The dataset contains information about energy usage, reactive power, CO2 emissions, and power factor, along with the load type and week status for each recorded time. The goal is to apply both classification and regression techniques to analyze and model the data effectively.

---

## Dataset

The dataset contains time-series data of energy consumption, measured every 15 minutes. The key features include:

- **Usage_kWh**: Energy consumption in kilowatt-hours.
- **Lagging_Current_Reactive.Power_kVarh**: Reactive power in kilovolt-amperes reactive (kVarh) for lagging current.
- **Leading_Current_Reactive_Power_kVarh**: Reactive power in kVarh for leading current.
- **CO2(tCO2)**: Carbon dioxide emissions in tons.
- **Lagging_Current_Power_Factor**: Power factor for lagging current.
- **Leading_Current_Power_Factor**: Power factor for leading current.
- **NSM**: A numerical value representing the timestamp.
- **WeekStatus**: Indicates if the time is a weekday or weekend.
- **Day_of_week**: The day of the week (e.g., Monday, Tuesday).
- **Load_Type**: Type of load (e.g., Light_Load, Heavy_Load).

This dataset serves as input for both regression and classification models to predict energy consumption and analyze power factors.

---

## Data Preparation

The `data_preparation.ipynb` notebook is responsible for cleaning and preparing the data for analysis. 

## Classification Models

The `classification_models.ipynb` notebook applies various classification algorithms to predict categorical outcomes. The models used include:

- **Logistic Regression**
- **K-Nearest Neighbors (KNN)**
- **Decision Tree Classifier**
- **Naive Bayes**
- **Random Forest Classifier**
- **AdaBoost Classifier**
- **ExtraTrees Classifier**
- **Support Vector Classifier (SVC)**
- **XGBoost Classifier**

These models are evaluated using accuracy, classification reports, confusion matrix, and ROC-AUC scores. Hyperparameter tuning with GridSearchCV is used to optimize model performance.

---

## Regression Models

The `regression_models.ipynb` notebook applies regression models to predict continuous outcomes such as energy consumption. The models used include:

- **Linear Regression**
- **Ridge Regression**
- **Decision Tree Regressor**
- **Random Forest Regressor**
- **Gradient Boosting Regressor**
- **K-Nearest Neighbors Regressor**
- **Bayesian Ridge**
- **XGBoost Regressor**

The models are evaluated using Mean Squared Error (MSE) and R-squared (R²) scores. GridSearchCV is used to find the best hyperparameters for each model.