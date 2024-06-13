- ### Direct url pass
- first and last must be use slash (/)
```python
path('', views.home, name="homepage")
path('navigation/about/', views.about, name="aboutpage")
path('navigation/contact/', views.contact, name="contactpage")


<a href="/">Home</a>
<a href="/navigation/about/">About</a>
<a href="/navigation/contact/">Contact</a>
```
- ### Named url use
- 