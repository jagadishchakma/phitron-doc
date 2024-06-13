- Go to 'admin.py' into app folder
- import models.py
- add this line
```python
admin.site.register(models.Student)
admin.site.register(models.Teacher)
```

- ### Arranging Showing
- jus add this line on models.py on specific class
```python
def __str__(self):
	return self.name
```
