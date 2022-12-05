# Django Custom User
Django ships with a built-in User model for authentication. for a real-world project, the official Django documentation highly recommends using a custom user model instead. This provides far more flexibility down the line so, as a general rule, always use a custom user model for all new Django projects.

### Setup
Install Django

Make a new Django project called django_project

Make a new app accounts

Start the local web server


## AbstractUser vs AbstractBaseUser
There are two modern ways to create a custom user model in Django: AbstractUser and AbstractBaseUser. In both cases we can subclass them to extend existing functionality however AbstractBaseUser requires much, much more work.

## Custom User Model
Creating our initial custom user model requires four steps:

update django_project/settings.py

create a new CustomUser model

create new UserCreation and UserChangeForm

update the admin
## Superuser
It's helpful to create a superuser that we can use to log in to the admin and test out log in/log out. On the command line type the following command and go through the prompts.
```
python manage.py createsuperuser
```
# References
1. https://learndjango.com/tutorials/django-custom-user-model