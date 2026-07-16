# Linear Regression with Streamlit

A small Python course project for training and exploring regression models with Streamlit.

The main mode loads a saved `LinearRegression` model, shows a prediction, and plots it against the closest actual target value from the dataset.

## Regression comparison lab

The **Regression comparison lab** generates synthetic data and compares linear and polynomial regression models. Adjust the sample count, noise level, and polynomial degree to see their MSE, R², and prediction curves.

## Setup

```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
python -m pip install -r requirements.txt
```

## Run

```powershell
python model.py
streamlit run app.py
```

## Project files

- `model.py` — trains and saves the regression model and datasets.
- `app.py` — Streamlit interface, prediction visualization, and comparison lab.
- `requirements.txt` — project dependencies.
- `linear_regression_model.joblib` — saved trained model.
- `X.joblib` and `y.joblib` — saved dataset features and targets.
