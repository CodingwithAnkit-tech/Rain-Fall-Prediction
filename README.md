# PROJECT OBJECTIVE--
The core goal is to determine whether it  will rain or not (Yes/No). Logistic Regression is used because it is a binary classifier, making it suitable for this type of problem.

# Rain Fall Prediction-
In this Rainfall Prediction project, we use three main weather factors: 
Precipitation (amount of rain), temperature (both highest and lowest of the day), and wind speed. 
Using this data, we train a Logistic Regression model to predict if it will rain or not. The aim is to help people, like farmers or event planners, make better decisions based on whether it's likely to rain.

# In This Project we use these modules:-

 1. Pandas and NumPy: For data manipulation and analysis.
 2. Scikit-Learn:     For building the Logistic Regression model and saving it as rfp.pkl.
 3. Pickle:           For saving and loading the trained model.

# For User Interface:

 Django Framework: To create the web application and integrate the machine learning model.
 HTML/CSS:         For designing the front-end of the web page where users input data.

# Key Points :-
 1) Acquire the dataset
 2) Import all the crucial libraries
 3) Import the dataset
 4) Extract the independent variables
 5) Extract the dependent variable
 6) Identifying and handling the missing values
 7) Encoding the categorical data
 8) Splitting the dataset
 9) A Confusion Matrix is created which summarizes the performance of the model on a set of test data. It offers a thorough analysis of the model’s Accuracy.
 10) Now we dump the file using pickle (a python module), so that we  create a model and a new file is created with the extension .pkl  

# How to Integrate PKL Model in Django-- 
1. First install Django Framework :  pip install Django

2. Create a Django Project and App: django-admin startproject myproject cd myproject python manage.py startapp myapp

3. Load the Model in Django Views: Load your model in the Django app views.
4. Set Up URL Configuration:- Add a URL pattern for the prediction view.
5. Create a Template : Create a simple form template for input and displaying results.
6. Create an External CSS File:
Create a new file named style.css in your app's static folder:
Directory Structure:
myapp/
├── static/
│   └── myapp/
│       └── style.css
└── templates/
    └── predict.html

In your predict.html file, link the external CSS:
<!-- Link to external CSS -->
{% load static %} 
<link rel="stylesheet" href="{% static 'myapp/style.css' %}">

7. Configure Django to Use Static Files :

Ensure your Django settings allow static files by adding the following in  
settings.py:

# settings.py
import os
STATIC_URL = '/static/'
STATICFILES_DIRS = [os.path.join(BASE_DIR, 'myapp/static’)]

8. Run the Django Server:
   python manage.py runserver

Visit http://127.0.0.1:8000 to make predictions using the integrated model.

# Applications of Rain Fall Prediction:

1. Agriculture
2. Disaster Management
3. Water Resource Management
4. Tourism and Outdoor Events

# How to run the code :
      1. First open cmd . 
      2. Then select Project Directory  using cd
      3. For run the project use command :python manage.py runserver
      4. Then we open chrome and run : localhost:8000	




