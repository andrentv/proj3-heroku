criar pasta
git init
criar env / source <nameenv>/bin/activate
pip install django
django-admin startproject <nome> .
cd <nome>
python manage.py startapp <nomeapp>
python manage.py runserver


- Ações
requirements.txt
runtime.txt
Procfile
Pastas no root: static /staticfiles

heroku login
heroku create or heroku git:remote -a vacc-proj3
heroku config:set ALLOWED_HOSTS=vacc-proj3.herokuapp.com
heroku config:set DEBUG_VALUE=False
heroku config:set DISABLE_COLLECTSTATIC=1
heroku run python manage.py makemigrations
heroku run python manage.py migrate
heroku run python manage.py createsuperuser
heroku run bash
heroku config:set ALLOWED_HOSTS=<endsiteheroku> -a, --app <nomeappheroku>