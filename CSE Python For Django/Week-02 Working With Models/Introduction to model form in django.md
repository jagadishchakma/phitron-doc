- ### Model Form
- In django, a ModelForm is  a form that is automatically generated from an existing model.
- A ModelForm includes all the fields defined in the model,  alogn with any additional validation and processing logic that you define in the form class.
- ### Meta Class
- a metaclass is a class that defines how other classes should behave. 
- provides additional information about the model form.
	- ==model== The model that the form is based on.
	- ==fields== a list of fields to include in the form. If this option is not spicified, all  fields in the model.
	- ==exclude== a list of fields to exclude from the form.
	- ==widgets== a dictionary of field names and their associated widgets
	- ==labels== A dicitionary of field names and their associated labels.
	- ==help_text== a dictionary of field names and their associated help text.
	- ==error_messages== a dictionary of fields names and their assosited wie
- ==meta class use for customize the outside  class or modelForm.==
- ### Model Form Fields
| Model Field               | Form Field                                                                                            |
| ------------------------- | ----------------------------------------------------------------------------------------------------- |
| AutoField                 | Not Represented in the form                                                                           |
| BigAutoField              | Not Representd in the form                                                                            |
| BigIntegerFiedl           | Integer Field with min_value and max_value set                                                        |
| BinaryField               | CharField, if editable is set to True on the model field, otherwise not represented in the form.      |
| BooleanField              | BooleanField, or NullBooleanField if null=True                                                        |
| CharField                 | CharField with max_length set to the mdoel fields max_length and empty value set to None if null=True |
| DateField                 | DateField                                                                                             |
| DateTimeField             | DateTimeField                                                                                         |
| DecimalField              | DecimalField                                                                                          |
| DurationField             | DurationField                                                                                         |
| EmailField                | EmailField                                                                                            |
| FileField                 | FileField                                                                                             |
| FilePathField             | FilePathField                                                                                         |
| FloatField                | FloatField                                                                                            |
| ForeignKey                | ModelChoiceField                                                                                      |
| ImageField                | ImageField                                                                                            |
| IntegerField              | IntegerField                                                                                          |
| IPAddressField            | IPAddressField                                                                                        |
| GenericIPAddressField     | GenericIPAddressField                                                                                 |
| ManyToManyField           | ModelMultiplechoiceField                                                                              |
| NullBooleanField          | NullBooleanField                                                                                      |
| PositiveIntegerField      | IntegerField                                                                                          |
| PositiveSmallIntegerField | IntegerField                                                                                          |
| SlugField                 | SlugField                                                                                             |
| SmallAutoField            | Not Represented in the form                                                                           |
| SmallIntegerField         | IntegerField                                                                                          |
| TextField                 | CharField with widget=forms.Textarea                                                                  |
| TimeField                 | TimeField                                                                                             |
| URLField                  | URLField                                                                                              |
| UUIDField                 | UUIDField                                                                                             |
- ### save()
- save(commit=False/True) 
	- This method creates and saves a database object  form the data bound to the form. by default True.
	- if commit=False, the it will return an object that hasn't yet been saved to the database.