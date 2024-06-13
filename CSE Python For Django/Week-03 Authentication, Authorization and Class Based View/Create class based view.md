- just add these line in 'views.py'
```python
from django.views.generic import CreateView
from django.urls import reverse_lazy

class AddPostCreateView(CreateView):
	model =  Post #form model
    form_class = forms.PostForm #formname
    template_name = 'add_post.html' #templatename
    success_url = reverse_lazy('add_post') #redirect named route
    def form_valid(self, form): #valid function check
        form.instance.author = self.request.user  #extra instance add
        return super().form_valid(form)
```

- then add these line in 'urls.py'
```python
path("add/", views.AddPostCreateView.as_view(),name="add_post"),
```
