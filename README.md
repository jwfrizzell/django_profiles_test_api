# Profiles Rest API

#REST API providing basic functionality for managing user profiles.

#Vargrant command to run vagrant file
vagrant up

#Connect to vagrant VM
vagrant ssh

#Create virtual environment in VM using virtualenvwrapper.
#Use python3
mkvirtaulenv profiles_api --python=python3

# **_To stop VM_**

deactivate

# **_To Switch bach to VM_**

workon profiles_api

#Install django
pip install django==1.11
#Install django rest api
pip install djangorestframework==3.6.2

#If src directory doesn't exist, create src
mkdir src

#navigate to src run following command
django-admin.py startproject profiles_project

#cd into profiles_project
cd profiles_project

#Create app in project using the manage.py file.
python manage.py startapp profiles_api

#In src/profiles_project run command to run server.
python manage.py runserver 0.0.0.0:8080

#Make migrations
python manage.py makemigrations

#Run migrations
python manage.py migrate
