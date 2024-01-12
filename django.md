# Django Cheat Sheet

A cheat sheet for Django commands.

#

[variable] = placeholder for a variable

#

## Django Installation

### Install Python

https://www.python.org/downloads/
https://www.infoworld.com/article/3530140/how-to-install-python-the-smart-way.html#:~:text=By%20default%20the%20Python%20installer,directory%20(e.g.%20C%3A%5CPython3.
https://www.youtube.com/watch?v=i-MuSAwgwCU&t=77s

### Create project directory

### Install Python virtual environment into project directory

> python -m venv [venv_folder_name]

https://www.infoworld.com/article/3239675/virtualenv-and-venv-python-virtual-environments-explained.html

https://www.youtube.com/watch?v=ohlRbcasPAc&t=7s

### Start the venv

> [venv_folder_name]\Scripts\activate

### update pip

> python -m pip install --upgrade pip
> https://pip.pypa.io/en/stable/installation/

### Install Django

> python -m pip install Django
> https://docs.djangoproject.com/en/4.1/topics/install/#installing-official-release

### Start Django Project

> django-admin startproject [projectname]

### Start Django App

> cd projectname
> python manage.py startapp [appname]

### Run migrations

> python manage.py migrate

### Create superuser

> python manage.py createsuperuser

### Start the Server

> python manage.py runserver

### Check if its running succesfully and go to:

http://localhost:8000

### stop the server with ctrl+C

### Registering the Application inside of settings.py add appname to INSTALLED_APPS

go to [projectname]/urls.py and add:

> from django.urls import include
> path('', include('appname.urls')),

### create an urls.py file in the app directory

#

(create the API with Rest Framework)

### Install React

https://www.digitalocean.com/community/tutorials/build-a-to-do-application-using-django-and-react
