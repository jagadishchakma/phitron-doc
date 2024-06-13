- all of the same
- just change route and copy paste  the code of add code  into edit route
- the follow this line just
```python
def edit(request, id):
	data = model.Students.objects.get(pk=id)
	form_category = forms.CategoryForm(instance=data)
	if request.method == 'POST'
		form_category = forms.CategoryForm(request.POST, instance=data)
	#....all those same add
```