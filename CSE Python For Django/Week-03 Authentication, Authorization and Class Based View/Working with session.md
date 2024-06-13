- first of all must be migrations
- ### set session
```python
def home(request):
	request.session.update({'name':'jagadish'})
```
- ### get session
```python
def about(request):
	name = request.session.get('name')
```
- ### delete session
```python
def contact(request):
	del request.session['name']
	#or
	request.session.flush() #full session will be deleted
```
- ### Implement session cookie expired
- add this line in 'settings.py'
```python
SESSION_COOKIE_AGE = 32#after 32 seconds will be expired
```

- implement
```python
if 'name' in request.session:
	.....
else:
	redirect() or send httpresponse

```