- just add these lines into 'views.py'
```python
from django.contrib.auth.views import LoginView
class UserLoginView(LoginView):
    template_name = 'login.html'
    def get_success_url(self) -> str:
        return reverse_lazy('profile')
    def form_valid(self, form):
        messages.success(self.request, 'login successfull')
        return super().form_valid(form)
    def form_invalid(self,form):
        messages.warning(self.request, 'login faild')
        return super().form_invalid(form)
```

- just add these lines into 'urls.py'
```python
path("login/", views.UserLoginView.as_view(), name="login"),
```

