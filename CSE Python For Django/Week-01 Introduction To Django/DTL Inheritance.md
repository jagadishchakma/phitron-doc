- For reuse code
- Do use it:
```django
{% extends 'base.html' %}

{% block body %}
 <h1>Home Page </h1>
 {{ block.super }}
 <h2>Home Page</h2>
{% endblock %}
```
- {% block.super %} is usefull
- 