# class-33

## Authentication & Production Server

**Q: What is the primary purpose of JSON Web Tokens (JWTs) and how do they work in terms of encoding and decoding data?**

The primary purpose of JSON Web Tokens (JWTs) is to securely transmit information between parties as a compact and self-contained token. They are often used for authentication and authorization in web applications.

JWTs work by encoding data into a JSON object, which is then digitally signed to ensure its integrity and authenticity. The data can be read by anyone, but the signature ensures that it has not been tampered with. To decode a JWT, the recipient validates the signature using a secret or public key, depending on the type of signature used.

---------

**Q: How does JWT Authentication integrate with Django REST Framework to secure API endpoints, and what are the key components involved in this process?**

JWT Authentication integrates with Django REST Framework (DRF) to secure API endpoints by providing a token-based authentication mechanism. The key components involved in this process are:

1. **DRF's Authentication Classes:**

2. **Obtaining a Token:** 

3. **Token Issuance:** 

4. **Token Inclusion:** 

5. **Authentication Validation:** 

6. **User Identification:**

7. **Handling Expired Tokens:** 
---------

**Q: Why is Django’s built-in runserver not suitable for production environments, and what are some alternative server options that should be considered for deploying a Django application?** 

Django's built-in runserver is not suitable for production environments because it is not designed to handle the high traffic and security requirements of a production server. Some reasons include:

1. **Single-Threaded and Non-Production Optimized:**

2. **No Load Balancing:**

3. **Lack of Security Features:**

**For production environments, it is recommended to use production-ready server options like:**

1. **Gunicorn (Green Unicorn):** 

2. **uWSGI:**

3. **nginx + Gunicorn/uWSGI:**

4. **Dedicated Hosting Solutions:** 
