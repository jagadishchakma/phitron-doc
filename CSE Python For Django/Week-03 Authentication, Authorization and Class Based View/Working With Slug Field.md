- add into 'models.py'
```python
slug = models.SlugField(max_length=100, null=True, blank=True, unique=True)
```
- add into 'admin.py'
```python
from django.contrib import admin
from . import models
# Register your models here.
class CategoryAdmin(admin.ModelAdmin):
    prepopulated_fields = {'slug': ('name',)}
    list_display = ['name', 'slug']
admin.site.register(models.Category, CategoryAdmin)
```
