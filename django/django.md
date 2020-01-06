
# Django 3.0 Documentation FR


- [Premiers pas](https://docs.djangoproject.com/fr/3.0/)
- [SQLLiteBrowser](https://sqlitebrowser.org/)

## Debug avec Visual Code Studio

- [django tutorial](https://code.visualstudio.com/docs/python/tutorial-django)

## Settings

- [settings.py](https://docs.djangoproject.com/fr/3.0/ref/settings/)


## Modèles

- [Modèles](https://docs.djangoproject.com/fr/3.0/topics/db/models/)
- [Référence des champs de modèle](https://docs.djangoproject.com/fr/3.0/ref/models/fields/#module-django.db.models.fields)


## Urls

-[Distribution des URL](https://docs.djangoproject.com/fr/3.0/topics/http/urls/)


## Vues génériques 

- [Vues génériques fondées sur les classes, fournies par Django](https://docs.djangoproject.com/fr/3.0/topics/class-based-views/generic-display/)

- [Vues génériques d’édition](https://docs.djangoproject.com/fr/3.0/ref/class-based-views/generic-editing/)


## Formulaires

- [Création de formulaires à partir de modèles](https://docs.djangoproject.com/fr/3.0/topics/forms/modelforms/)
- [django-crispy-forms](https://django-crispy-forms.readthedocs.io/en/latest/install.html#installing-django-crispy-forms)
- [Creating your own layout objects](https://django-crispy-forms.readthedocs.io/en/latest/layouts.html#creating-your-own-layout-objects)

## Login, logout, signup

Recherche de login.html, urls,LOGIN_REDIRECT_URL, LOGOUT_REDIRECT_URKL

- [setup django.contrib.auths](https://docs.djangoproject.com/fr/3.0/topics/auth/default/)
- [model django.contrib.auths](https://docs.djangoproject.com/fr/3.0/ref/contrib/auth/)

```
<a href="{% url 'login' %}">Login</a>
<a href="{% url 'logout' %}">Logout</a>
{{ user.username }}
{{ user.is_authenticated }}
{{ user.is_staff }}
```

## Exceptions

- [django.core.exceptions](https://docs.djangoproject.com/fr/3.0/ref/exceptions/)

```
    MultipleObjectsReturned,
    ValidationError,
    ObjectDoesNotExist,
```

## Utilitaires Django

- [django.utils.text](https://docs.djangoproject.com/fr/3.0/ref/utils/)

```
    slugify()
```

## Écriture de commandes django-admin personnalisées

- [app/management/commands](https://docs.djangoproject.com/fr/3.0/howto/custom-management-commands/)