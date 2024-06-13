
- ### Create app
- $django-admin startapp myapp
- after creating an app must be included this app name in settings.py istalled apps list.
- ### App Folder Structure
- __init.py__
- apps.py
- models.py
- test.py
- views.py
- admin.py
- migrations folder
- urls.py -> need to create pre-installed not have
- ### route and view
- are the same of project route
- but one thing
```python
from django.urls import path,include
path('navigation', include('navigation.urls'))
```
