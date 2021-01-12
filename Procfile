release: python manage.py migrate
web: daphne chatApp.asgi:application --port $PORT --bind 0.0.0.0 -v2
worker: python manage.py runworker channels --settings=chatApp.settings -v2