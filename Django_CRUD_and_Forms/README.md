# Readings: Django CRUD and Forms

### How do Django Forms facilitate user input handling, and what are some key components of creating a form using the Django framework?
- Django Forms facilitate the handling of user input by providing a high-level, Pythonic way to define, validate, and process HTML forms. They abstract away the complexities of dealing with form rendering, data validation, and data manipulation. Here are some key components of creating a form using the Django framework:Form Class: django.forms.Form or django.forms.ModelForm, Fields:(CharField, EmailField, IntegerField, etc),Validation and Rendering


### Explain the purpose of Django Templates in web development and describe how template inheritance can be utilized to improve code reusability and maintainability.
- Django Templates are a powerful tool for generating dynamic HTML. They separate the presentation logic from the business logic by providing a way to define the structure and layout of HTML pages with placeholders for dynamic content. Some important aspects of Django Templates include:

- Template Language: Django provides its own template language (DTL) that allows you to embed Python code within HTML templates. It provides constructs like loops, conditionals, variable interpolation, and template tags for performing logic and displaying dynamic data.

- Template Inheritance: Template inheritance is a feature that allows you to create a base template with common elements and then define child templates that inherit from the base template. Child templates can override specific blocks or extend the base template as a whole. This approach improves code reusability and maintainability by reducing redundancy.

- Context: When rendering a template, you pass a context, which is a dictionary of variable names and their corresponding values. These variables can be accessed within the template for dynamic rendering.

### Describe the function of Django Views in handling HTTP requests, and outline the differences between function-based views and class-based views.
- Django Views handle HTTP requests and return HTTP responses. They encapsulate the logic for processing requests and producing responses. There are two types of views in Django: function-based views (FBVs) and class-based views (CBVs)
-  FBVs are simpler and suitable for smaller views, while CBVs offer more flexibility, code reuse, and maintainability for larger and more complex views.
