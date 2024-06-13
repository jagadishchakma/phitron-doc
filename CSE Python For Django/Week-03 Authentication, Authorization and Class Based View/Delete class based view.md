- just add these line in 'views.py'
```python
from django.views.generic import DeleteView
from django.urls import reverse_lazy

class DeletePostView(DeleteView):
     model = Post
    #  form_class = forms.PostForm
     template_name = 'post_confirm_delete.html'
     #pk_url_kwarg = 'id'
     success_url = reverse_lazy('homepage')
```

- just add these line in 'urls.py'
```python
path("delete/<int:pk>", views.DeletePostView.as_view(), name="delete_post")
```
