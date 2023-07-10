# API Deployment

### What are the key principles to follow when organizing and configuring Django settings for a project, according to the “Django Settings Best Practices” reading?

- Keep settings in environment variables. This makes it easy to change settings without having to modify the code or restart the server.
- Write default values for production configuration (excluding secret keys and tokens). This allows you to use the same settings file for development and production, but with different values for sensitive settings.
- Don't hardcode sensitive settings, and don't put them in VCS. This includes things like the secret key, database passwords, and API keys.
- Split settings into groups: Django, third-party, project. This makes it easier to find and understand the different settings.
- Follow naming conventions for custom (project) settings. This makes it easier to identify and understand the different settings.

### How does the White Noise library contribute to the efficient serving of static files in a Django application, and what are the steps to integrate it into a project?
- White Noise is a Django library that helps to improve the performance of static files by caching them and serving them from a CDN. This can significantly reduce the load on your web server and improve the user experience.

- To integrate White Noise into a project, you need to:

    1. Install the White Noise library.
    > pip install whitenoise

    2. Add the following lines to your settings.py file:
    ```python
    
    STATIC_URL = '/static/'
    STATICFILES_STORAGE = 'whitenoise.storage.CompressedManifestStaticFilesStorage'
    ```
    3. Collect static files   
    > python manage.py collectstatic
    

### What is the purpose of Cross-Origin Resource Sharing (CORS) in web applications, and how can it be implemented and configured in a Django project to control access to resources?
- Cross-Origin Resource Sharing (CORS) is a mechanism that allows a web application running at one origin to access the resources from a server running at a different origin. This is useful for making AJAX requests to a different domain.

- CORS can be implemented in a Django project by installing the django-cors-headers library and adding the following lines to your settings.py file:
```python

INSTALLED_APPS = [
    ...
    'corsheaders',
]

MIDDLEWARE = [
    ...
    'corsheaders.middleware.CorsMiddleware',
]

CORS_ALLOWED_ORIGINS = [
    'http://example.com',
    'https://example.com',
]

CORS_ALLOWED_HEADERS = [
    'accept',
    'accept-encoding',
    'authorization',
    'content-type',
    'dnt',
    'origin',
    'user-agent',
    'x-csrftoken',
    'x-requested-with',
]

CORS_ALLOWED_METHODS = [
    'GET',
    'POST',
    'PUT',
    'PATCH',
    'DELETE',
]

CORS_ALLOW_CREDENTIALS = True

```

- To configure CORS in a Django project, you need to:

    1. Install the django-cors-headers package.
    2. Add corsheaders to the INSTALLED_APPS list in your settings.py file.
    3. Add the corsheaders.middleware.CorsMiddleware middleware to the MIDDLEWARE list in your settings.py file.
    4. Configure the CORS settings in your settings.py file.
