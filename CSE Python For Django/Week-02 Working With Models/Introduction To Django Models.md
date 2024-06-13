- In Python Django have built in a database called 'SQLite'
- ### ORM
- Object-Relational Mapper is  a programming tools/technique that helps application to interact with database such a SQLite, MySQL, PostgreSQL, Oracle.
- ==create a database schema== from defined classes or models.
- ==generate SQL from python code== for a  paritcular database which means developer do not need to  write SQL code.
- helps to ==change the database== easily
- ==use connectors== to connect databases with a web application.
- ### QuerySet
- A QuerySet can be defined as a list containing all those objects we have created using the  Django model.
- QuerySets helps us
	- read the data from the database.
	- filter it.
	- order it.
- ### Model
- A model is the single, definitive source of information about our data.
- It contains the:
	- essential ==fields and behaviors== of the data.
	- each model maps to ==a single database table==.
- ### Model Class
- Model class is a class which will represent a table in database.
- Each model is a python class that subclasses django.db.models.Model
- Each attributes represents a  database field.
- Django gives automatically-generated database-access API
- Django provides sqlite database by default.
- We can use other database like  MYSQL, Oracle SQL etch.
- ### Migrations
- Migrations are way of propagating changes to make models( adding a field, deleting a model, etc) into your database schema.
- ==makemigrations:==  is used to convert model class into sql statements.
```python
python manage.py makemigrations
```
- ==migrate:== is used to execute sql statements generated by makemigrations.
```python
python manage.py migrate
```
- ==showmigrations:== This list a project's migrations.
- ### Built-in Field
- IntegerField
- AutoField
- FloatField
- TextField
- CharField
- BooleanField
- EmailField
- URLField
- ### Built-in Field Options
- ==null :-== contain either True or False. If True, Django will store empty values as NULL in the database. Default is False.
- ==blank :-=== contain either True or False. If True, the field is allowed to be blank.
	- Note: null is purely database-related, whereas blank is validation-related.
- ==default :-== default value for the field.
- ==verbose_name :-== A human-readable name for the field. If the verbose name isn't given, Django will automatically create it using the field's attribute name, converting underscores to space.
- ==db_column :-== The name of the database column to use for this field. If this isn't given, Django will use the field's name.
- ==primary_ke :-== If True, that filed will be primary key for the model.
- ==unique:== True/False
- 