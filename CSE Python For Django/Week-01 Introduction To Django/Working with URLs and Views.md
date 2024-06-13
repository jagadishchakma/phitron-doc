
- ### Inside Project Folder
	- Not have 'views.py' but have 'urls.py'
- ### Inside App Folder
	- Not have 'urls.py' but have 'views.py'

- ### URLs
-  urls must be enclosed with slash (/) without home route
- urls can handle named route and mostly used named route
- for working with urls two files need to import
- ==for urls use 'urls' mdoule
```python
from django.urls import path # one file 
form . import views # two file
urlpatterns=[
	path('', views.home, name='homepage')
	path('conatct/', views.contact, name="contactpage")
]
```

- ### Views
- views1
- ==for views use 'http' module
```python
from django.http import HttpResponse
def home(request):
	return HttpResponse("this is home page')

def contact(request):
	return HttpResponse('this is contact page')
```
