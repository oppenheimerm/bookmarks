# Bookmarks Social Website

## About
Building a social website to learn me some Django.  Users are able to join this online platform and interact with each other by sharing content.  Users will be able to bookmark any image on the internet and share it wih others.  They will also be able to see activity on the platform from the users they follow and like/unlike the image shared by them.

## Requirements

The [requirements.txt](./requirements.txt) has the following packages:

| Package | Description |
| ------- | ----------- |
| [Django](https://pypi.org/project/Django/) | Web application framework. |
| [pyscopg2-binary](https://pypi.org/project/psycopg-binary/) | PostgreSQL database adapter for Python. I had to downgrade to(pip install psycopg2==2.8.6) See also(https://www.psycopg.org/install/) |
| [django-cleanup](https://pypi.org/project/django-cleanup/) | The django-cleanup app automatically deletes files for FileField, ImageField and subclasses. When a FileField’s value is changed and the model is saved, the old file is deleted. When a model that has a FileField is deleted, the file is also deleted. A file that is set as the FileField’s default value will not be deleted.
| [python-dotenv](https://pypi.org/project/python-dotenv/) | Read key-value pairs from .env file and set them as environment variables. In this sample app, those variables describe how to connect to the database locally. <br><br> This package is used in the [manage.py](./manage.py) file to load environment variables. |
| [whitenoise](https://pypi.org/project/whitenoise/) | Static file serving for WSGI applications, used in the deployed app. <br><br> This package is used in the [azureproject/production.py](./azureproject/production.py) file, which configures production settings. |
| [python-dotenv](https://pypi.org/project/python-dotenv/) | Python-dotenv reads key-value pairs from a .env file and can set them as environment variables.