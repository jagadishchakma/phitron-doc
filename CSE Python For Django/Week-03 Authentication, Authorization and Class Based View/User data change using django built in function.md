- add these line in 'forms.py'
```python
from django.contrib.auth.models import User
from django.contrib.auth.forms import UserCreationForm, UserChangeForm
from django import forms

class UserChange(UserChangeForm):
     password = None
     class Meta:
        model= User
        fields= ['username', 'first_name', 'last_name', 'email']
```

- add these line in 'views.py'
```python
from . import forms

def profile(request):
    if request.user.is_authenticated:
        form = forms.UserChange(instance=request.user)
        if request.method == 'POST':
            form = forms.UserChange(request.POST, instance=request.user)
            if form.is_valid():
                messages.success(request, 'Account Updated Successfully!')
                form.save()
        return render(request, 'profile.html', {'user': request.user, 'form': form})
    else:
        return redirect('loginpage')
```


