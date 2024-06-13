
```django
{% for field in form %}
  {{ field.label_tag }}{% if field.field.required %}<span style="color:black; font-weight:bold">*</span>{% endif %}
  {{field}}
  {{field.errors}}
{% endfor %}
```

- or
```django
- or

```django
{% for field in form %}
  {{ field.label }}{% if field.field.required %}<span style="color:black; font-weight:bold">*</span>{% endif %}
  {{field}}
  {{field.errors}}
{% endfor %}
```
```