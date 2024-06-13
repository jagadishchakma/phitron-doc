- route setup
- then
```python
def user_logout(request):

    if request.user.is_authenticated:

        logout(request)

        return redirect('loginpage')

    else:

        return redirect('homepage')
```
