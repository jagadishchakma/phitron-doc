- just setup a url with a single primary key
- then add that url views.py
```python
stu = models.Student.objects.get(pk=roll).delete()
```
- then redirect
```python
return redirect('postpage')
```
- pk = primary key
