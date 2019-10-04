# tuto_drf
Apprendre à créer des API Avec Django


## Apprendre

https://books.agiliq.com/projects/django-api-polls-tutorial/en/latest/


## Recherche

https://medium.com/better-programming/how-to-make-search-fields-dynamic-in-django-rest-framework-72922bfa1543


## Les champs dynamique

https://github.com/dbrgn/drf-dynamic-fields



## EX:

http://localhost:8000/polls/?fields=id,question,created_by.username&search=factor&search_fields=question

## Docummentation

### Swargger

```bash

pip install django-rest-swagger

# settings.py

INSTALLED_APPS = [
    # ...
    'polls',
    'rest_framework_swagger',
]


# urls.py

from rest_framework_swagger.views import get_swagger_view

schema_view = get_swagger_view(title='Polls API')

# ...
urlpatterns = [
    # ...
    path(r'swagger-docs/', schema_view),
]


```bash
