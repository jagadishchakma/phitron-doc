```python
name = forms.CharField(
	label="Your Name: ",
	initial="Jhon Doe",
	help_text="Name length must be withing 50 characters",
	required=False/True,
	disabled=True/False,
	max_length=23,
	min_length=21,
	widget=forms.TextInput(attrs={
		'placeholder':'Enter your name',
		'id': 'uname',
		'class': 'form-control ublock'
		})
)



unknown = forms.CharField(
		widget=forms.TextInput(),
		widget=forms.NumberInput(),
		widget=forms.EmailField(),
		widget=forms.TextAreaField()
)
 
date = forms.DateField(
		widget=forms.DateInput(attrs={'type':'date'})
)
```