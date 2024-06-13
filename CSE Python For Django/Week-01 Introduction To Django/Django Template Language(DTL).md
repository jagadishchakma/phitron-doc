- ### For Value Showing Use:
- {{use double curly brackets}}
- ### Conditional Template Filtering
```django
{% if age > 20 %}
	you are adult
{% elif age < 20 %}
	you are boy
{% else %}
	you are nothing
{% endif %}
```
- ### Loop Template Filtering
```django
{% for item in items %}
	{{ item }}
{% endfor %}
```

