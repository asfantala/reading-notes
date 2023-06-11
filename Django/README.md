# Django
### What are the key components of the Django framework, and how do they contribute to building a web application?
- View: A view is a request handler function, which receives HTTP requests and returns HTTP responses. Views access the data needed to satisfy requests via models, and delegate the formatting of the response to templates.
- Models: Models are Python objects that define the structure of an application's data, and provide mechanisms to manage (add, modify, delete) and query records in the database.
- Templates: A template is a text file defining the structure or layout of a file (such as an HTML page), with placeholders used to represent actual content. A view can dynamically create an HTML page using an HTML template, populating it with data from a model. A template can be used to define the structure of any type of file; it doesn't have to be HTML

![](basic-django.png)

### Explain the role of Django’s MTV (Model-View-Template) architecture and how it handles a typical web request-response cycle.
1. A user sends a request to a specific URL of the Django application.
2. Django's URL resolver matches the requested URL pattern to a corresponding view function.
3. The view function is invoked, which performs necessary operations like retrieving data from models, processing user input, or performing other business logic.
4. The view function then passes the data to a template, along with any other context required for rendering.
5. The template combines the data with the HTML markup, rendering a dynamic HTML page.
6. The generated HTML is returned as a response to the user's browser.
7. The user's browser receives the response and renders the HTML, displaying the web page to the user.

### What is the purpose of Tailwind CSS, and how does it differ from Bootstrap CSS?
- Tailwind CSS is a utility-first CSS framework for rapidly building custom user interfaces. It is a highly customizable, low-level CSS framework that gives you all of the building blocks you need to build bespoke designs without any annoying opinionated styles you have to fight to override.