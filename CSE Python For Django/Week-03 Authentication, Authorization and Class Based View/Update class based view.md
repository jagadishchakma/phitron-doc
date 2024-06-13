
- just add these line 'views.py'
```python
from django.views.generic import UpdateView
from django.urls import reverse_lazy

class EditPostView(UpdateView):
     model = Post #model name
     form_class = forms.PostForm #form name
     template_name = 'add_post.html' #template name
     pk_url_kwarg = 'id' # pass id
     success_url = reverse_lazy('homepage') #redirect page
```

- just add these line 'urls.py'
```python
path("edit/<int:id>", views.EditPostView.as_view(),name="edit_post"),
```

