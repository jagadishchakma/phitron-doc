- No excuse.
- Just same do it
```python
data = form.cleaned_data

        upfile = data['fileupload']

        with open('./navigation/upload/' + upfile.name, 'wb+') as destination:

            for chunk in upfile.chunks():

                destination.write(chunk)

        print(upfile)

        print(data)
```
