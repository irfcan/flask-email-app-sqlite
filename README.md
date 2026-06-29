# flask-email-app-sqlite
flask-email-app-sqlite

# Hands-on Flask-05.1 : Handling SQL with Flask Web Application

Purpose of the this hands-on training is to give the students introductory knowledge of how to handle forms, how to connect to database and how to use sql within Flask web application

## Learning Outcomes

At the end of the this hands-on training, students will be able to;

- build a web application with Python Flask framework.

- handle forms using the flask-wtf module.

- configure connection to the `sqlite` database.

- work with a database using the SQL within Flask application.

- use git repo to manage the application versioning.


## Students are expected to 

- Examine and run the `app-with-sqlite.py`  

## Outline

- Run the  Sample Web Application with SQLite and database implementation

## - Examine and Run the Sample Web Application with SQLite and database implementation in your Local

- Examine which module are imported for this project 

- Examine the anatomy of the `Database` configuration of `app-with-sqlite.py`

```
- It adds required environmental variables for SQLite  according to documentation    
   https://flask-sqlalchemy.palletsprojects.com/en/2.x/config/

- It drops users table if exists, creates new users table and adds some rows for sample

- It Executes sql commands to  commit data to tables

```

- Examine the anatomy of the `Functions`  determined in `app-with-sqlite.py`

```
- Function named `find_emails` which find emails using keyword from the user table in the db,
 and returns result as tuples `(name, email)`.

- Function named `insert_email` which adds new email to users table the db.
```

- Examine the anatomy of  the `Decorators `  determined in `app-with-sqlite.py`

```
- Function named `emails`  finds email addresses by keyword using `GET` and `POST` methods,
uses template files named `emails.html` given under `templates` folder
and it assigns to the static route of ('/')

- Function named `add_email` inserts new email to the database using `GET` and `POST` methods,
uses template files named `add-email.html` given under `templates` folder and  it assign to the static route of ('add')

- The Flask application  can be reached from any host on port 8080.
```

- Be sure that you install `flask-mysql, sqlalchemy, Flask-SQLAlchemy` via  `sudo pip3 install `

- Run the  application `app-with-sqlite.py` 

- Check the database tables via SQLite Browser ( You can download the SQLite Browser from the link : 
https://sqlitebrowser.org/)
