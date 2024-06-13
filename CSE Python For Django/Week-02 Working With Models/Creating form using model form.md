- a model create
- create 'forms.py'
- just add these line into:
```python
from django import forms
class StudentForm(forms.ModelForm):

    class Meta:

        model = models.StudentModel

        fields = '__all__'

        labels = {

        }

        widgets={

        }
        error_messages={
        
        }
```
  