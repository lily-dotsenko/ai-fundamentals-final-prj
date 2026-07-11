# Linear Regression with Streamlit

A small course project that trains a linear-regression model and lets a user explore its predictions in a Streamlit interface.

## Setup

Create and activate a virtual environment, then install the dependencies:

```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
python -m pip install -r requirements.txt
```

## Train the model

Run the training script from the project folder:

```powershell
python model.py
```

It creates `linear_regression_model.joblib`, `X.joblib`, and `y.joblib`. Run this command again whenever the training data or model logic changes.

## Start the application

After the artifacts have been created, launch Streamlit:

```powershell
streamlit run app.py
```

Use the slider to choose an input feature, then select **Predict value** to see the predicted target and its comparison with the closest observation in the training data.

## Run tests

```powershell
python -m unittest discover -s tests -v
```
