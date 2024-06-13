- ### set cookie
```python
from datetime import datetime, timedelta
def home(request):
	response = render(request,'home.html')
	response.set_cookie('name', 'Jagadish Chakma')
	resposne.set_cookie('age','28', max_size=10)#how many durations stay on site this cookie
	response.set_cookie('study', 'BAA', expires=datetime.utcnow()+timedelta(days=9)) #stay cookie on site up to 9 days then delete
	return response
```


- ### get cookie value
- must try on different path
```python
def about(request):
	cookie_value = request.COOKIES.get('name')
	return render(request, 'about.html', {'name':cookie_value})
```
- ### delete cookie
- must try on different path
```python
def contact(request):
	response = render(request, 'contact.html')
	response.delete_cookie('name')
	return response
```