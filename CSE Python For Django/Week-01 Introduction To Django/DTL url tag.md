- url tag means use named routing into template.
```django
path('post/<int:id>/<int:roll>/<str:title>/')
<a href="{% url 'postpage' id=12 roll = 34234 title='how to make url tag'%}"></a>
```
