```python
for item in items.category.all()
	print(item)

```

```django
{% for item in items.category.all %}

{{item.name}}

{% enfor %}
```
