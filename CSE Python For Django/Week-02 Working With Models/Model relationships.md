- ### Relationships in Django Model
	- One to One Relationships
	- One to Many Relationships
	- Many to Many Relationships
- ### One to One Relationships
```python
OneToOneField(to, on_delete, parent_link=False, **options)
```
- ==to(required):== It should be a reference to the related model class.
- ==on_delete(required):== 
	- models.CASCADE
	- models.PROTECT
	- models.SET_NUL
	- models.SET_DEFAULT
	- models.SET()
	- models.SET_ON_DELETE
- ### One to Many Relationships
```python
ForeignKey(to, on_delete,  parent_link=False, **options)
```
- one writers can have multiple post
- only one side have one to many relationship
- ### Many to Many Relationships
```python
ManyToMany(to, on_delete,  parent_link=False, **options)
```
-  both side have one to many relationship
- a post can have multiple category and a category can have multiple post.
