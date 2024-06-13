

- just use it

```python
form.save()
```


```python
def about(request):

    form = forms.StudentForm()

    if request.method == 'POST':

        form = forms.StudentForm(request.POST)

        if form.is_valid():

              form.save(commit=False)

              print(form.cleaned_data)

        else:

            form = forms.StudentForm(request.POST)

    students = models.Student.objects.all()

    return render(request, 'about.html', {'data':students, 'form': form})
```