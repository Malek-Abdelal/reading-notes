# class-28

## Django CRUD and Forms

**Q: How do Django Forms facilitate user input handling, and what are some key components of creating a form using the Django framework?**

Django Forms facilitate user input handling by providing a high-level, Pythonic way to define and handle forms on web applications. Key components of creating a form using the Django framework include:

1. Form Class: Defining a Form class that subclasses `django.forms.Form` or `django.forms.ModelForm`. This class defines the fields and their validation rules.

2. Form Fields: Defining various types of form fields like text fields, checkboxes, radio buttons, etc., using classes provided by Django's forms module.

3. Rendering: Rendering the form in the template using Django's template system, which automatically generates HTML for the form fields based on their definitions.

4. Validation: Handling form data validation on the server-side, ensuring that the input adheres to the defined rules and constraints.

5. Handling Submitted Data: Processing user-submitted data in views, validating it, and performing necessary actions based on the form's contents.

----------

**Q: Explain the purpose of Django Templates in web development and describe how template inheritance can be utilized to improve code reusability and maintainability**

The purpose of Django Templates in web development is to separate the presentation layer from the business logic, promoting code modularity and maintainability. Templates allow developers to define the structure and layout of web pages using Django's template language.

Template inheritance in Django enables code reusability and maintainability by creating a base template containing the common structure of the website. Other templates can then extend this base template and override specific blocks to customize their content. This way, changes made to the base template are automatically reflected across all extended templates, streamlining development and updates.

---------

**Q: Describe the function of Django Views in handling HTTP requests, and outline the differences between function-based views and class-based views.**

Django Views handle HTTP requests by processing user input, interacting with the database, and returning an HTTP response.

**Differences:**

- Function-Based Views (FBVs) are defined as Python functions, while Class-Based Views (CBVs) are defined as Python classes.
- CBVs offer more built-in functionalities and code reusability through inheritance and mixins, while FBVs require more manual handling of HTTP methods and request/response processing.