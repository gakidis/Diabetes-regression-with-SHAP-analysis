# Diabetes Progression Prediction & Model Interpretability

This project focuses on predicting diabetes progression using various machine learning regression algorithms. It includes a complete pipeline from data preprocessing and hyperparameter tuning to model evaluation and interpretability using SHAP (SHapley Additive exPlanations).

## Project Overview
The goal of this analysis is to model the progression of diabetes based on several physiological variables. We compare multiple regression models to find the most accurate one and then use SHAP analysis to explain the model's decisions, ensuring transparency and trust in the predictions.

## Dataset
The project uses the **Scikit-learn Diabetes dataset**.
- **Features:** Age, Sex, BMI, Blood Pressure, and six blood serum measurements.
- **Target:** A quantitative measure of disease progression one year after baseline.

## Machine Learning Models
The following regressors were implemented and compared:
- **Gaussian Process Regressor (GPR)**
- **Random Forest Regressor (RF)**
- **Support Vector Regressor (SVR)**
- **Gradient Boosting Regressor (GBR)**

## Workflow
1. **Exploratory Data Analysis (EDA):** Visualizing target distribution and checking for missing values.
2. **Data Preprocessing:** Feature scaling using `MinMaxScaler`.
3. **Cross-Validation:** Implementation of **6-Fold Cross-Validation** for robust evaluation.
4. **Hyperparameter Optimization:** Used `RandomizedSearchCV` for model tuning.
5. **Evaluation Metrics:** RMSE, MAE, MAPE, and Max Error.
6. **Explainable AI (XAI):** Applied **SHAP Analysis** to interpret the Support Vector Regressor (SVR) model.

## Repository Structure
- `test.ipynb`: The main Jupyter Notebook containing the source code.
- `results.csv`: Evaluation metrics exported after training.
- `shap_results_SVR/`: Directory containing generated SHAP interpretation plots.
- `requirements.txt`: List of Python dependencies.

## Installation & Usage
1. **Clone the repository:**
   ```bash
   git clone [https://github.com/gakidis/Diabetes-regression-with-SHAP-analysis.git](https://github.com/gakidis/Diabetes-regression-with-SHAP-analysis.git)