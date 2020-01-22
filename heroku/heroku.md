# Deploy on Heroku



## Related links

https://devcenter.heroku.com/articles/django-app-configuration

https://devcenter.heroku.com/articles/getting-started-with-python#run-the-app-locally

https://devcenter.heroku.com/articles/heroku-postgresql#connecting-with-django


## .env

```
PYTHONPATH=<>
SECRET_KEY=<>
DATABASE_URL=<>
DEBUG_DJANGO=0
```

## .gitignore

```
.env
```

## settings

```
import django_heroku
import dj_database_url
from dotenv import load_dotenv

...
dotenv_path = BASE_DIR + "\.env"
load_dotenv(dotenv_path)

...
SECRET_KEY = os.getenv("SECRET_KEY")
DEBUG = strtobool(os.getenv("DEBUG_DJANGO", "0"))

...
DATABASES = {
    "default": dj_database_url.config(),
}
DATABASES["default"] = dj_database_url.config(conn_max_age=600, ssl_require=True)

...
django_heroku.settings(locals())


```