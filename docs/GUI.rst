
GUI
====

Datta Able Django
------------------

Datta Able Django is an Open-source dashboard generated by the AppSeed platform with basic modules, database, authentication and deployment scripts on top of **Datta Able** (free version). For newcomers, [Datta Able](https://appseed.us/admin-dashboards/django-dashboard-dattaable-pro) Bootstrap Lite is the most stylised Bootstrap 4 Lite Admin Template, around all other Lite/Free admin templates in the market. It comes with high feature-rich pages and components with fully developer-centric code. Before developing Datta Able our key points were performance and design.


**Features**

* UI-Ready app, SQLite Database, Django Native ORM
* Modular design, clean code-base
* Session-Based Authentication, Forms validation
* Deployment scripts: Docker, Gunicorn / Nginx
* Support via **Github** and Discord https://discord.gg/fZC6hup


**Links**

* Datta Able Django Product page https://appseed.us/admin-dashboards/django-datta-able
* Datta Able Django LIVE deployment https://django-datta-able.appseed-srv1.com/ 
* Datta Able Django product documentaion https://docs.appseed.us/products/django-dashboards/datta-able 

**How to use it**

.. code-block:: shell

  # Get the code
  git clone https://github.com/app-generator/django-datta-able.git
  cd django-datta-able

  # Virtualenv modules installation (Unix based systems)
  virtualenv env
  source env/bin/activate

  # Virtualenv modules installation (Windows based systems)
  # virtualenv env
  # .\env\Scripts\activate

  # Install modules
  # SQLIte version
  pip3 install -r requirements.txt

  # Create tables
  python manage.py makemigrations
  python manage.py migrate

  # Start the application (development mode)
  python manage.py runserver # default port 8000

  # Start the app - custom port 
  # python manage.py runserver 0.0.0.0:<your_port>

  # Access the web app in browser: http://127.0.0.1:8000/


Note: To use the app, please access the registration page and **create a new user**. After authentication, the app will unlock the private pages.


**Deployment**

The app is provided with a basic configuration to be executed in:

* Docker https://www.docker.com/

* Gunicorn https://gunicorn.org/

* Waitress https://docs.pylonsproject.org/projects/waitress/en/stable/


**Docker execution**

The application can be easily executed in a docker container. The steps:

1. Get the code

.. code-block:: shell

  git clone https://github.com/app-generator/django-dashboard-dattaable.git
  cd django-dashboard-dattaable

2. Start the app in Docker

.. code-block:: shell

  sudo docker-compose pull && sudo docker-compose build && sudo docker-compose up -d


3. Visit `http://localhost:5005` in your browser. The app should be up & running.


**Gunicorn**

Gunicorn 'Green Unicorn' is a Python WSGI HTTP Server for UNIX.

1. Install using pip

.. code-block:: shell

  pip install gunicorn

2. Start the app using gunicorn binary

.. code-block:: shell

  gunicorn --bind=0.0.0.0:8001 core.wsgi:application
  Serving on http://localhost:8001

3. Visit `http://localhost:8001` in your browser. The app should be up & running.


**Waitress**

Waitress (Gunicorn equivalent for Windows) is meant to be a production-quality pure-Python WSGI server with very acceptable performance. It has no dependencies except ones that live in the Python standard library.

1. Install using pip

.. code-block:: shell

  pip install waitress


2. Start the app using [waitress-serve](https://docs.pylonsproject.org/projects/waitress/en/stable/runner.html)

.. code-block:: shell

  waitress-serve --port=8001 core.wsgi:application
  Serving on http://localhost:8001


3. Visit `http://localhost:8001` in your browser. The app should be up & running.


**Credits & Links**

Django Admin Dashboards https://appseed.us/admin-dashboards/django

Index with UI-ready **admin dashboards** generated by the AppSeed platform in Django Framework https://www.djangoproject.com/
Start fast your next Django project by using functional admin dashboards enhanced with Database, ORM, authentication flow, helpers and deployment scripts.

What is Django https://docs.appseed.us/what-is/django/

Django https://www.djangoproject.com/ is a Python-based free and open-source web framework, which follows the model-template-view architectural pattern. It is maintained by the Django Software Foundation, an independent organization established as a 501 non-profit. Django's primary goal is to ease the creation of complex, database-driven websites.


What is a dashboard https://en.wikipedia.org/wiki/Dashboard

A dashboard is a set of pages that are easy to read and offer information to the user in real-time regarding his business. A dashboard usually consists of graphical representations of the current status and trends within an organization. Having a well-designed dashboard will give you the possibility to act and make informed decisions based on the data that your business provides - *definition provided by [Creative-Tim - Free Dashboard Templates](https://www.creative-tim.com/blog/web-design/free-dashboard-templates/?ref=appseed)*.

Datta Able Free Dashboard https://codedthemes.com/item/datta-able-bootstrap-lite/

Datta Able Bootstrap Lite is the most styled Bootstrap 4 Lite Admin Template, around all other Lite/Free admin templates in the market. It comes with high feature-rich pages and components with fully developer-centric code. Comes with error/bug-free, well structured, well-commented code and regularly with all latest updated code, which saves your large amount of developing backend application time and it is fully customizable. - provided by **CodedThemes**.


