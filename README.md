# hello-django

It's time for some hands-on experience building your first Django project!

Django's [official website](https://www.djangoproject.com/) has the following to say about the web framework: "Django is a high-level Python Web framework that encourages rapid development and clean, pragmatic design. Built by experienced developers, it takes care of much of the hassle of Web development, so you can focus on writing your app without needing to reinvent the wheel. It’s free and open source."

Sounds like a pretty sweet deal! Learning to use Django will allow us to build what we want, without encountering many of the web development woes that come with building something from scratch or employing a [microframework](https://en.wikipedia.org/wiki/Microframework), e.g., Express.js or Flask. 

To get a [feel](https://media.giphy.com/media/hokMyu1PAKfJK/giphy.gif) for what it's like to build a Django web application, let's focus on creating a simple project.

#### **Your Task**

Build a Django web application that displays ["hello, world"](https://blog.hackerrank.com/the-history-of-hello-world/).

To do this, you'll need the following:

*   a Django project named `hello_django`
*   a Django app named `hello_app`
*   a `urls.py` file in `hello_django`
    *   `urls.py`
        *   sets up an endpoint for the root of the application, i.e., [http://127.0.0.1:8000/](http://127.0.0.1:8000/)
            *   you'll want to hook this endpoint up with a view
        *   sets up an endpoint/path for the admin panel
            *   this should already be a part of your `urlpatterns` if you used `django-admin` to create your project
*   a `views.py` file in `hello_app`
    *   <span>`views.py` will contain a view called `index_view`</span>
    *   `index_view` will render the `index.html` template with context passed to the template i.e. "hello, world"
*   a folder named `templates`
    *   this folder should live at the same level as your <span>`hello_django` and `hello_app` folders</span>
*   a file in your `templates`directory called `index.html`
    *   this file will display the "hello, world" text
    *   "hello, world" _cannot_ be hardcoded into this file; it must come from the view.
*   a `settings.py` that is properly configured
    *   Django needs to know where to find the template folder
        *   configure the `TEMPLATES` variable in `settings.py`
    *   Django needs to know about the `hello_app` we're using
        *   configure the `INSTALLED_APPS` variable in `settings.py`
*   a `pyproject.toml` file with Django listed as a dependency

<pre>File Structure Preview: 
.
├── hello_app
│   ├── __init__.py
│   └── views.py
├── hello_django
│   ├── __init__.py
│   ├── asgi.py
│   ├── settings.py
│   ├── urls.py
│   └── wsgi.py
├── manage.py
├── pyproject.toml
├── poetry.lock
└── templates
    └── index.html
</pre>
