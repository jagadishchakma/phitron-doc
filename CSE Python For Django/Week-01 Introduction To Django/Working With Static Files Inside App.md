- Just create a folder name 'static' and paste some files.
- Don't need to necessary change settings.py , djagno automatically known when using app
- using template filter
```django
{% load static %}
<img src="{ static 'ryzen7.jpg'}" alt="ryzen 7 processor">
```
