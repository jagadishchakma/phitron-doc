- go to 'models.py' in app folder
- then jus add it;
```python
# Create your models here.

class Student(models.Model):

    name = models.CharField(max_length=50)

    roll = models.IntegerField(primary_key=True)

    address = models.TextField()

    father_name = models.CharField(max_length=50,default="Bijoy Chakma")
```

- convert into sql code:
```python
py mange.py makemigrations
```
- execute converted sql code:
```python
py manage.py migrate
```

- If you don't specify which field will be 'primary_key' then django automatically create a 'id' field and make this primary_key. 
