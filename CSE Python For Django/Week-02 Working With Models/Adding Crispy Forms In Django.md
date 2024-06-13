- Documentation: https://django-crispy-forms.readthedocs.io/en/latest/install.html#installing-django-crispy-forms
- $pip install django-crispy-forms
- INSTALLED_APPS = (
    ...
    'crispy_forms',
)
- Documentation: https://github.com/django-crispy-forms/crispy-bootstrap5
- $ pip install crispy-bootstrap5
- INSTALLED_APPS = (
    ...
    "crispy_forms",
    "crispy_bootstrap5",
    ...
)

CRISPY_ALLOWED_TEMPLATE_PACKS = "bootstrap5"

CRISPY_TEMPLATE_PACK = "bootstrap5"
- add this
```django
{% load crispy_forms_tags %}

{{form | crispy}}
```
