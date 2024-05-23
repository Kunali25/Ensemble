Diabetic Prediction Ensemble Model
Overview
This project is an ensemble model for predicting diabetes using machine learning algorithms K-Nearest Neighbors (KNN) and LightGBM. The web application is built using Django for the backend and HTML, CSS, and jQuery for the frontend. The model takes nine input attributes to predict the likelihood of a person having diabetes.

Features
Machine Learning Models: Utilizes KNN and LightGBM to create an ensemble model for prediction.
Web Framework: Built with Django for robust backend support.
Frontend: User-friendly interface designed with HTML, CSS, and jQuery.
Prediction Input: Accepts nine input attributes to provide an accurate prediction.
Input Attributes
The model uses the following nine attributes to predict diabetes:

Pregnancies: Number of times pregnant.
Glucose: Plasma glucose concentration.
Blood Pressure: Diastolic blood pressure (mm Hg).
Skin Thickness: Triceps skin fold thickness (mm).
Insulin: 2-Hour serum insulin (mu U/ml).
BMI: Body mass index (weight in kg/(height in m)^2).
Diabetes Pedigree Function: A function that scores likelihood of diabetes based on family history.
Age: Age of the person.
Activity Level: Level of physical activity.
Installation
Prerequisites
Python 3.x
Django
pip (Python package installer)
Virtual environment tool (optional but recommended)
Setup

Clone the repository:
git clone https://github.com/yourusername/diabetic-prediction-ensemble-model.git
cd diabetic-prediction-ensemble-model

Create a virtual environment:
python -m venv env
source env/bin/activate  # On Windows use `env\Scripts\activate`

Install the required packages:
pip install -r requirements.txt

Run migrations:
python manage.py migrate

Start the Django development server:
python manage.py runserver

Open your web browser and navigate to:
http://127.0.0.1:8000/
Usage
Home Page:

The home page provides a form for the user to input the nine attributes required for prediction.
Input the Data:

Enter values for pregnancies, glucose, blood pressure, skin thickness, insulin, BMI, diabetes pedigree function, age, and activity level.
Get Prediction:

Submit the form to get the prediction result.
Project Structure
/diabetic_prediction/: Django project settings and configuration.
/prediction_app/: Main application containing models, views, and templates.
models.py: Contains the Django models.
views.py: Contains the view functions to handle requests and responses.
templates/: Contains the HTML templates for the frontend.
static/: Contains static files such as CSS and JavaScript.
/machine_learning/: Directory for machine learning model scripts and data processing.
knn_model.py: Script for the KNN model.
lightgbm_model.py: Script for the LightGBM model.
ensemble_model.py: Script for combining the models into an ensemble.
data_preprocessing.py: Script for data preprocessing and feature engineering.
requirements.txt: Lists all the Python packages required for the project.
