- just do it in 'views.py'
```python
from django.contrib import messages

if from.is_valid():
	form.save()
	messages.success(request,'success message')
	messages.info(request, 'info message')
	messages.warning(request, 'warning message')
```

- hold it on '.html'
```python
{% if messages %}
{% for m in messages %}
{{m}}
{% endfor %}
{% endif %}
```



- different message

```django
		{% if messages %}
          {% for m in messages %}
          <div class="alert {% if m.tags %} alert-{{m.tags}} {% endif %}" role="alert">
            {{m}}
          </div>
          {% endfor %}
        {% endif %}
```

