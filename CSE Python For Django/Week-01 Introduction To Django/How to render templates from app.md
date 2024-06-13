- just create a folder name 'templates' inside app directory.
- then all html file inlcudes into it.
- that's right.
- and not necessary settings.py edit like globally.
```python
from django.shortcuts import render
def home(request):
	return render(request, 'home.html')
```
- and remember this globally templates file name and app templtes file name must be unique.