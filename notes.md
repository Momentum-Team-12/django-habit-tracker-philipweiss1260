# Configure Django App for Heroku

import django_on_heroku

# add to bottom of setting.py

django_on_heroku.settings(locals())
del DATABASES['default']['options']['sslmode']
