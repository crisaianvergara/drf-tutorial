cd ~
django-admin startproject tutorial
cd tutorial

python manage.py startapp snippets

INSTALLED_APPS = [
...
'rest_framework',
'snippets',
]

python manage.py makemigrations snippets
python manage.py migrate snippets

python manage.py runserver

curl localhost:8000/snippets/

python manage.py createsuperuser

# Requirements

touch requirements.txt
pip freeze > requirements.txt
pip install -r requirements.txt
