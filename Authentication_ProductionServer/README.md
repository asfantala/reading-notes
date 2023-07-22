# Authentication & Production Server

### What is the primary purpose of JSON Web Tokens (JWTs) and how do they work in terms of encoding and decoding data?

- The primary purpose of JSON Web Tokens (JWTs) is to securely transmit information between parties. JWTs are encoded as a JSON object that is digitally signed, which ensures that the information cannot be tampered with.

- To encode a JWT, the header and payload are first encoded as JSON. Then, the signature is generated using the secret or public/private key pair. The signature, header, and payload are then concatenated together and encoded using Base64url.

- To decode a JWT, the token is first decoded using Base64url. Then, the header, payload, and signature are separated. The signature is then verified using the secret or public/private key pair. If the signature is valid, then the token is considered to be authentic.

### How does JWT Authentication integrate with Django REST Framework to secure API endpoints, and what are the key components involved in this process?
- JWT Authentication is a popular way to secure API endpoints in Django REST Framework. It works by using JSON Web Tokens (JWTs) to transmit authentication information between the client and server.

- The key components involved in the process of integrating JWT Authentication with Django REST Framework are:

        - The JWT token: The JWT token is a JSON object that contains the user's identity and other relevant information. It is generated by the server and sent to the client in the response to a successful login request.
        - The JWT authentication backend: The JWT authentication backend is a class that is responsible for verifying JWT tokens. It is typically implemented as a subclass of the rest_framework.authentication.BaseAuthentication class.
        - The JWT_AUTH settings: The JWT_AUTH settings are a set of configuration options that control the behavior of JWT Authentication. These settings are typically defined in the Django project's settings.py file.


### Why is Django’s built-in runserver not suitable for production environments, and what are some alternative server options that should be considered for deploying a Django application?

- Django's built-in runserver is not suitable for production environments because it is not designed for high-traffic or high-performance applications. It is a single-threaded server, which means that it can only handle one request at a time. This can lead to performance bottlenecks and timeouts if your application receives a lot of traffic.

- server options that should be considered for deploying a Django application include:

1. Gunicorn
2. Nginx
3. Apache