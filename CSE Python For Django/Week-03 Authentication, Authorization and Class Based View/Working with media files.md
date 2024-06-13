- just add these line in 'settings.py'
```python
#base url to server media files into apps
MEDIA_URL = '/media/' # add this line if you want to upload into apps folder

  

#path where media is stored in globally
MEDIA_ROOT = BASE_DIR / 'media' # add this line if you want to upload globally
```
- just create a 'media' folder app or globally
- just add these line into 'models.py'
```python
image = models.ImageField(upload_to='posts/media/uploads/', blank=True, null=True) # if you want to upload into apps folder

image = models.ImageField(upload_to='uploads/', blank=True, null=True) # if you want to upload into globally
```
- just add these line into 'ursl.py' (optional)
```python
from django.conf import settings
from django.conf.urls.static import static

urlpatterns = [
	path('admin/', admin.site.urls),
	...
]
if settings.DEBUG: urlpatterns += static(settings.MEDIA_URL, document_root=settings.MEDIA_ROOT) #if you want to url based access media files: http://localhost:8080/uploads/one.jpg
```
