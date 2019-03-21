# REST API

## what is this?
simple api example using flask. a flask api object contains one or more functionalities (GET, POST, etc). 

## Create virtenv for the project:

1. $ virtualenv rest-api
2. $ source rest-api/bin/activate
3. $ mkdir ~/rest-app
4. $ cd ~/rest-app

## Clone the repo to 'rest-app' project workspace:

git clone https://github.com/95rade/Salary-API.git

## Import db to sqlite3:

1. $ sqlite3 salaries.db
2. sqlite> .mode csv salaries
3. sqlite> .import employee_chicago.csv salaries

Note: Every time db is updated you have to re-import it into sqlite3:

## install modules:

```
pip install -r requirements.txt
pip freeze
```

## run
```
python app.py
```

then go to http://localhost:5000/departments

you could drill down by deparments too!

try http://localhost:5000/dept/police

My code walk-through is as follows

*  I downloaded latest Salary dataset from chicago data site

*  Dumped that CSV  into my SQLite db.

*  Used SQLAlchemy to connect to database and do select operations.

*  Created Flask-Restful classes to map functions with API URL

*  Returned the queried data as JSON ,which can be used universally.

See how simple it is to create a data API. We can also add support to PUT,POST and DELETE on data too.We can also have an authentication system for fetching data through API. Python and Flask are very powerful tools to create API rapidly. GitHub link is given below. Give it a try and extend it with the things mentioned above.

https://github.com/narenaryan/Salary-API

## ToDo:  Add POST, PUT and DELETE methods.
