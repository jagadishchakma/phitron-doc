 - add these line in 'forms.py'
```python
from django.contrib.auth.models import User
from django.contrib.auth.forms import UserCreationForm

class RegisterForm(UserCreationForm):
    class Meta:
	    model = User
        fields = ['username', 'first_name', 'last_name', 'email',]
```

- then..........same all of those. save and view
- add this line in views.py
```python
uname = register_form.cleaned_data['username']
upass = register_form.cleaned_data['password1']
user = authenticate(username=uname,password=upass)
login(request, user)
return redirect('profile')
```
- jus add like this for customize in '.html'
```python
<!-- {{ form | crispy }} -->
{% for frm in form %}

{{frm.label_tag}}

{{frm}}

{{frm.errors}}

{% endfor %}
```