- ### Django Project Folder Structure
	- ##### Outer Project Folder/Root Directory
		- manage.py -> project command line utitlity
			- $py manage.py runserver
	- ##### Inner Project Folder
		- init.py -> python package built-in code have and use around in folder.
		- wsgi.py ->  web server getway interface communicates with web application.
		- asgi.py -> asynchronously wsgy.
		- settings.py -> all configurations have.
		- urls.py -> routing setup.
- ### Project vs Application
	- project -> multiple app combaine make a project
		- $django-admin startproject myproject
	- app -> inside a  project single feature is a app
		- $django-admin startapp myapp