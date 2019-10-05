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


## Api key

https://florimondmanca.github.io/djangorestframework-api-key/



## Vue Js , Axios

<script src="https://unpkg.com/axios/dist/axios.min.js"></script>


```bash

onload() {

    //axios.defaults.xsrfCookieName = 'csrftoken'
    //axios.defaults.xsrfHeaderName = 'X-CSRFToken'


    axios.get('url')
        .then(response => {
            console.log(response.data)

        })
        .catch((err) => {
            console.log(err);
        })
},
```
