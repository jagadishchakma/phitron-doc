- for function based views
```python
from django.contrib.auth.decorators import login_required

@login_required
def profile():
	pass
```
- for class based views
```python
from django.contrib.auth.decorators import login_required
from django.utils.decorators import method_decorator

@method_decorator(login_required, name='dispatch')
class AddPost():
	pass
```


- settings.py
```python
LOGIN_REDIRECT_URL = 'profile'
LOGIN_URL = 'login'
```
