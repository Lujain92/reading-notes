# API Deployment

 ## Configuring Django Settings: Best Practices

 ### Managing Django Settings: Issues

 **Different environments**

 Usually, you have several environments: local, dev, ci, qa, staging, production, etc. Each environment can have its own specific settings (for example: DEBUG = True, more verbose logging, additional apps, some mocked data, etc). You need an approach that allows you to keep all these Django setting configurations.

 **Sensitive data**

 You have SECRET_KEY in each Django project. On top of this there can be DB passwords and tokens for third-party APIs like Amazon or Twitter. This data cannot be stored in VCS.

 **Sharing settings between team members**

 You need a general approach to eliminate human error when working with the settings. For example, a developer may add a third-party app or some API integration and fail to add specific settings. On large (or even mid-size) projects, this can cause real issues.

 **Django settings are a Python code**

 This is a curse and a blessing at the same time. It gives you a lot of flexibility, but can also be a problem – instead of key-value pairs, settings.py can have a very tricky logic.

 ### Setting Django Configurations

 There is no built-in universal way to configure Django settings without hardcoding them. But books, open-source and work projects provide a lot of recommendations and approaches on how to do it best.

 **<u>settings_local.py</u>**

 The basic idea of this method is to extend all environment-specific settings in the settings_local.py file, which is ignored by VCS.

 _settings.py_

# References :

1. https://djangostars.com/blog/configuring-django-settings-best-practices/

 
2. https://www.hostinger.com/tutorials/ssh-tutorial-how-does-ssh-work
