# Car-Price-Prediction

## Vehicle dataset
Used Cars data form websites. 

This dataset contains information about used cars.
This data can be used for a lot of purposes such as price prediction to exemplify the use of linear regression in Machine Learning.
The columns in the given dataset are as follows:

name
year
selling_price
km_driven
fuel
seller_type
transmission
Owner

## Aim 

Predict the Sell Price for the car. 

# To deploy on Heroku you need two things:
+ requirements.txt file
+ Procfile

**How to Get the requirements.txt file**

# Method 1: using pip
pip freeze > requirements.txt

# Method 2: using pipreqs (recommended)
+ First install pipreqs
pip install pipreqs
+ Second use pipreqs to get the requirements.txt file of any project
pipreqs yourmlapp_folder

**For the  procfile can I simply use: web: gunicorn app:app?**
+ What to Put inside the Procfile
+ web: gunicorn app:app

**should the static and templates folder remain the same for deployment as the one we prepared during Productionization?**
+ Yes,  you will have to push them too to github

**Procfile**
For Heroku you need to say which is the first file bascially you need to execute. 
web:gunicorn app: app
Which is your file of Flask you want to run first? app.py

**setup.sh**
Script program for bash that helps us to execute code with respect to requirement.txt. 
It helps us to setup environment for streamlit library. 

**Flasgger**
This will help us to create the UI part in a much feasible and easy way. It won't be that decorative but it would be a good front end web app. In Flasgger, Swagger will automatically generate the frontend UI part. 
