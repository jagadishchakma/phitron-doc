- create a static folder any kind of name and palced some static files
- but in settings.py must be add it:
```python
STATIC_URL = 'static/'

STATICFILES_DIRS = [

    BASE_DIR / STATIC_URL

]
```


- direct url pass:
```django
<img src="static/ryzen7.jpg" alt="ryzen 7 processor">
```

- load it using filtering:
- not need to static/ add.
```Django
{% load static %}
<img src="{% static 'ryzen7.jpg'%}" alt="ryzen 7 processor">
```

