f- just create a route
- then do it in 'views.py'
```python
##login page

from django.contrib.auth.forms import AuthenticationForm, PasswordChangeForm, SetPasswordForm

from django.contrib.auth import authenticate, login, logout, update_session_auth_hash

def pass_change(request):

    if request.user.is_authenticated:

        form  = PasswordChangeForm(user=request.user)

        if request.method == 'POST':

            form  = PasswordChangeForm(user=request.user,data=request.POST)

            if form.is_valid():

                form.save()

                update_session_auth_hash(request, form.user)

                return redirect('profile_page')

        return render(request, 'passchange.html', {'form':form})

    else:

        return redirect('homepage')
```

- without old password change password
```python
PasswordChangeForm instead use SetPasswordForm
```
