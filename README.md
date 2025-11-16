# House Price Prediction App

An end to end machine learning project that predicts US house prices using Linear Regression.
The project includes data cleaning, feature scaling, model training, and a fully working Streamlit web app.

## Project Overview

This project demonstrates how a complete ML workflow is built and deployed:

* Loading and exploring a large real estate dataset
* Cleaning missing values and preparing the data
* Selecting numeric features
* Scaling inputs using StandardScaler
* Training a Linear Regression model
* Saving the trained model and scaler using joblib
* Building a Streamlit app to make live predictions

This setup is suitable for junior data analyst or data science portfolio work.

## Features

* End to end ML pipeline
* Reusable model through `.pkl` files
* Clean and minimal Streamlit interface
* Accepts user input and returns predicted house price
* Includes a small sample dataset for reference
* Easy to run locally
* Uses standard Python libraries

## Project Structure

```
project/
  app.py
  model.pkl
  scaler.pkl
  sample_data.csv
  analytics_modeling.ipynb
  requirements.txt
  README.md
  Prediction_app_screenshot.png
```

## Dataset

A small sample of the dataset is included for demonstration:

* `sample_data.csv`: 500 randomly sampled rows showing feature structure

The full dataset is **not included** due to GitHub’s 100 MB file size limit.

Full dataset source:
**[https://www.kaggle.com/datasets/ahmedshahriarsakib/usa-real-estate-dataset/data]**

## How to Run This Project Locally

### 1. Clone the repository

git clone https://github.com/AhmedAli58/house_price_prediction.git
cd house_price_prediction

### 2. Create a virtual environment (optional but recommended)

python3 -m venv venv
source venv/bin/activate   # Mac / Linux
venv\Scripts\activate      # Windows

### 3. Install dependencies

pip install -r requirements.txt

### 4. Run the Streamlit app

streamlit run app.py

You will see a URL like this:
`http://localhost:8501`
Open it in your browser.

## How the Model Works

### Data Preparation

* Selected key numeric features such as price, bed, bath, house_size, and lot size
* Removed missing values
* Scaled feature values using StandardScaler

### Model

* Linear Regression trained on the cleaned dataset
* Joblib used to save scaler and model for reuse

### Prediction Flow

1. User enters feature values in Streamlit
2. Inputs are converted to a NumPy array
3. Array is scaled using the saved `scaler.pkl`
4. Model predicts price using `model.pkl`
5. Result is displayed on screen

## Technologies Used

* Python
* Pandas
* NumPy
* Scikit-Learn
* Streamlit
* Joblib
* Jupyter Notebook

## Key Learning Outcomes

* Loading and exploring a large real estate dataset
* Cleaning and preprocessing the data
* Selecting numeric columns
* Scaling the inputs
* Training a Linear Regression model
* Saving the trained model and scaler
* Building a Streamlit interface for predictions

## Future Improvements

* Add more features (location, zip_code, previous sale date)
* Use regularized regression (Ridge or Lasso)
* Add interactive visualizations
* Deploy online (Streamlit Cloud)

## Contact

**Ahmed Ali**
Data Analyst
GitHub: https://github.com/AhmedAli58
LinkedIn: https://www.linkedin.com/in/ahmedali79x/
