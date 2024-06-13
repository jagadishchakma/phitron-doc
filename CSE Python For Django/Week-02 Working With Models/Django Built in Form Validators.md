- just do it.
```python
from django.core import validators

class signinForm(forms.Form):

    name = forms.CharField(widget=forms.TextInput, validators=[validators.MinLengthValidator(10,'Enter a name with at least 10 character')])
```

- then other validator google search:
- Global variable:
	- ==not clear now==
