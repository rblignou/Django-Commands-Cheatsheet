# DJANGO TUTORIAL
## ******COMMAND FOR CREATING NEW PROJECT DIRECTORY******
### django-admin startproject project_name
- When we execute the startproject command after django-admin cli then following files are directories are created-
   - A folder is created with your project_name which contains another folder same as project_name and a python file manage.py is created. This Folder of project_name contains 5 files
      - __init__.py
      - asgi.py
      - settings.py
      - urls.py
      - wsgi.py 

## ******CREATING NEW APP IN THE PROJECT DIRECTORY******
### python manage.py startapp application_name
- After entering inside project folder run the above command. After running the above command a folder of the given application name is created which contains a folder named as migrations and 6 more files which are given below.
   - __init__.py
   - admin.py
   - apps.py
   - models.py
   - tests.py
   - views.py
- Inside the migrations folder __init__.py file is created. 
- Now register the app name in the settings.py which is inside the project_name folder.)

## ******COMMAND FOR RUNNING DJANGO APPLICATION******
### python manage.py runserver
( When we run this coomand for first time a db.sqlite3 file is created. This command runs the server for django application )

## ******COMMAND FOR CHECK DJANGO VERSION******
### python -m django --version

## ******COMMAND FOR OPENING IPYTHON SHELL******
### python manage.py shell

## ******COMMAND FOR VERIFYING DATABASE CONNECTION******
from django.db import connection
cursor = connection.cursor()
(If nothing happens it means database has configured successfully)

### ******COMMAND FOR KNOW ABOUT OPTIONS IN MANAGE.PY******
python manage.py help

(
Available subcommands:

[auth]
    *changepassword
    *createsuperuser

[contenttypes]
    remove_stale_contenttypes

[django]
    check
    compilemessages
    createcachetable
    dbshell
    diffsettings
    *dumpdata
    flush
    inspectdb
    *loaddata
    makemessages
    *migrate
    sendtestemail
    *showmigrations
    sqlflush
    *sqlmigrate
    sqlsequencereset
    squashmigrations
    *startapp
    *startproject
    *test
    testserver

[sessions]
    clearsessions

[staticfiles]
    collectstatic
    findstatic
    *runserver
)


## ******COMMAND FOR CREATING SUPERUSER FOR ADMIN-APP******
### python manage.py createsuperuser

## ******COMMAND FOR GENERATING SQL STATEMENTS******
### python manage.py makemigrations

## ******COMMAND FOR EXECUTING SQL STATEMENTS******
### python manage.py migrate file_name

## ******COMMAND FOR EXECUTING SQL STATEMENTS FOR ALL FILES******
### python manage.py migrate
