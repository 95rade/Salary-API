# REST API

## what is this?
simple api example using flask. a flask api object contains one or more functionalities (GET, POST, etc). 

## Create virtenv for the project:

$ virtualenv rest-api
$ source rest-api/bin/activate
$ mkdir ~/rest-app
$ cd ~/rest-app

## Clone the repo to 'rest-app' project workspace:

git clone https://github.com/95rade/Salary-API.git

## Import db to sqlite3:

$ sqlite3 salaries.db
sqlite> .mode csv salaries
sqlite> .import employee_chicago.csv salaries

## install modules:

```
pip install -r requirements.txt
```

## run
```
python app.py
```

then go to http://localhost:5000/departments

you could drill down by deparments too!

try http://localhost:5000/dept/police

## ToDo:  Add POST, PUT and DELETE methods.
