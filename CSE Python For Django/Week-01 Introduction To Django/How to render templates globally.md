- make a 'templates' folder inside root directory
- then 'settings.py' inside templates add or register 'templates' name
- then create a html file inside templates folder
- then return a render from views 'html' file
```python
from django.shortcuts import render
def home(request):
	return render(request, 'index.html')
```
