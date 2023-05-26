# Django-blog

## Overview
This is my attempt at building a blog website using Django to resharpen my skills again. This is just a barebone application without any styling and other additional stuff. It is just able to update new articles via admin page and list them in a page.

### Setup

The first thing to do is to clone the repository:

```sh
$ git clone https://github.com/itzmidinesh/Django-blog.git
$ cd Django-blog
```

Create a virtual environment to install dependencies in and activate it:

```sh
$ virtualenv venv
$ venv/Scripts/activate
```

Install project dependencies:

```sh
(venv)$ pip install -r requirements.txt
```
Note the `(venv)` in front of the prompt. This indicates that this terminal
session operates in a virtual environment set up by `virtualenv`.

Once `pip` has finished installing the dependencies, apply the migrations and run the development server:
```sh
(venv)$ cd blog
(venv)$ python manage.py migrate
(venv)$ python manage.py runserver
```
And navigate to `http://127.0.0.1:8000/article/`.

If you want to use the admin page at `http://127.0.0.1:8000/admin/` create a superuser:
```sh
(env)$ python manage.py createsuperuser
```