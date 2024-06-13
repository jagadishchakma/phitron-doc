- first do it
```python
#form.py
from django import forms
class SiginForm(forms.Form):
	uname = forms.CharField()
	email = forms.EmailField()
```
- next do it
```python
#views.py
from . import forms
def signing(request):
	if reques.method == POST:
		form = forms.SignInForm(request.POST)
		if form.is_valid():
			data = form.cleaned_data
			print(data['name'])
			print(data['email'])
	form = forms.SignInForm()
	return render(request, 'signing.html', {'form': form})
```

- next do it
```django
#signing.html
{{form}}
```

