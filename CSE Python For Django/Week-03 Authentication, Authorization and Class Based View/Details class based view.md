- just add a template 'post_details.html'
- just add these line into 'views.py'
```python
from django.views.generic import DetailView
class DetailPostView(DetailView):
     model = Post
     pk_url_kwarg = 'id'
     template_name = 'post_details.html'
```

- just add these line into 'urls.py'
```python
path("details/<int:id>", views.DetailPostView.as_view(), name="detail_post")
```

- just add these line into deatils link 
```django
<a href="{% url 'post_details' id=post.id %}">Details See...</a>
```
