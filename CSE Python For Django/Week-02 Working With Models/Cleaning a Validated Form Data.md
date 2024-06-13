- just do it
```python
#forms.py
class ContactForm(forms.Form):
	name = forms.CharField(widget=forms.TextInput)

	def clean_name(self):
		valname =  self.cleaned_data['name']
		if len(valname) < 10:
			raise forms.ValidationError("Name must be at least 10 character!")
		else:
			return valname
```


- just care of it
```python
#views.py
#which form render validation form ? normal form
```
