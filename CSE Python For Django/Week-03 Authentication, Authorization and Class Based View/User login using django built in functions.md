- all of do in 'views.py'
```python
##login page

from django.contrib.auth.forms import AuthenticationForm
from django.contrib.auth import authenticate, login, logout



def user_login(request):

    if request.user.is_authenticated:

        return redirect('profile_page')

    else:

        loginform = AuthenticationForm()

        if request.method == 'POST':

            loginform = AuthenticationForm(request=request,data=request.POST)

            if loginform.is_valid():

                name = loginform.cleaned_data['username']

                password  = loginform.cleaned_data['password']

                user = authenticate(username = name, password = password)

                print(user)

                if user is not None:

                    login(request, user)

                    return  redirect('profile_page')

        return render(request, 'login.html', {'form':loginform })
```
