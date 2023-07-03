# Permissions & Postgresql

### What are the key components and purpose of Django Rest Framework (DRF) permissions, and how do they help in securing an API?
- The key components of DRF permissions are:

- Permission classes: These are classes that define the permissions for a particular resource. There are a number of built-in permission classes, such as IsAuthenticated and DjangoModelPermissions. You can also create your own custom permission classes.
- View permissions: These are permissions that are attached to views. When a view is called, DRF will check the view's permissions to determine if the user is allowed to access the view.
- Object permissions: These are permissions that are attached to individual objects. Object permissions allow you to control who can access, update, and delete specific objects

### In SQL, what is the purpose of the SELECT statement, and how would you use it to retrieve all columns from a table called ‘employees’?
- The SELECT statement is used to retrieve data from a database. It is the most common SQL statement, and it is used in a wide variety of applications.
- The syntax for the SELECT statement is:
```
SELECT [columns]
FROM [table]
[WHERE [conditions]]
[ORDER BY [column]]
[LIMIT [number]]
```
- To retrieve all columns from a table called 'employees', you would use the following SQL statement:
```sql
SELECT * FROM employees;
```

### Can you explain the role of DRF Generic Views and provide examples of their usage in building a RESTful API?
- DRF Generic Views are a set of pre-built views that can be used to quickly and easily create RESTful APIs. They provide a number of features that make it easy to develop APIs, such as:

        - Automatic serialization and deserialization of data
        - Support for different HTTP methods
        - Support for authentication and authorization
- DRF Generic Views can be used to create a wide variety of RESTful APIs. For example, you could use them to create an API for a product  

