- Context means data pass to views
- Context means when we pass data backend to fornt-end in encryption is called context.
- In django use dictionary formate for pass data to views
```python
return render(request, 'home.html', {'fname':'Jagadish', 'lname':'Chakma', 'age': 28})
```

```django
<p>First Name: {{fname}}</p>
<p>Last Name: {{lname}}</p>
<p>Age: {{age}}</p>
```
