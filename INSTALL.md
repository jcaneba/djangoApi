sudo apt-get install libmysqlclient-dev
python3 -m venv ./venv
source ./venv/bin/activate
pip3 install django djangorestframework mysqlclient
django-admin startproject api
cd api
python manage.py startapp main
python manage.py makemigrations
python manage.py migrate

python manage.py runserver
