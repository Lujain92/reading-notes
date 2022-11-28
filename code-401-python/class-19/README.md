# Django Models
## Using models
Django web applications access and manage data through Python objects referred to as models. Models define the structure of stored data, including the field types and possibly also their maximum size, default values, selection list options, help text for documentation, label text for forms.



## Designing the LocalLibrary models
Assume you want to make a bookstore...

We know that we need to store information about books (title, summary, author, written language, category, ISBN) and that we might have multiple copies available (with globally unique id, availability status, etc.). We might need to store more information about the author than just their name, and there might be multiple authors with the same or similar names. We want to be able to sort information based on book title, author, written language, and category.

## Types of Relationships

Django allows you to define relationships that are one to one (OneToOneField), one to many (ForeignKey) and many to many (ManyToManyField).


## Model definition

Models are usually defined in an application's models.py file. They are implemented as subclasses of django.db.models.Model, and can include fields, methods and metadata.

### Fields

A model can have an arbitrary number of fields, of any type — each one represents a column of data that we want to store in one of our database tables. Each database record (row) will consist of one of each field value.

Common field types

1. CharField

2. TextField
3. IntegerField

3. DateField and DateTimeField
4. EmailField

5. FileField and ImageField

6. AutoField

7. ForeignKey

8. ManyToManyField

### Metadata

One of the most useful features of this metadata is to control the default ordering of records returned when you query the model type.

### Methods

A model can also have methods.

Minimally, in every model you should define the standard Python class method __ str __( ) to return a human-rea able string for each object. This string is used to represent individual records in the administration site.

Another common method to include in Django models is get_absolute_url(), which returns a URL for displaying individual model records on the website.

### Model management

Once you've defined your model classes you can use them to create, update, or delete records, and to run queries to get all records or particular subsets of records.

# Refrences:
1. https://developer.mozilla.org/en-US/docs/Learn/Server-side/Django/Models

2. https://developer.mozilla.org/en-US/docs/Learn/Server-side/Django/Admin_site