- just add these line in 'urls.py'
```python
form django.contrib.auth.views import LogOutView

path("logout/", views.LogoutView.as_view(next_page="homepage"), name="logout"),
```
