# REST API

## what is this?
simple api example using flask. a flask api object contains one or more functionalities (GET, POST, etc). 

First , i downloaded the data-set as CSV and dumped it into my sqlite database.

$ sqlite3 salaries.db
sqlite> .mode csv salaries
sqlite> .import employee_chicago.csv salaries
and imported CSV.

Now we are going to build a flask app that serves this data as a REST API.

$ virtualenv rest-api
$ source rest-api/bin/activate
$ mkdir ~/rest-app
$ cd ~/rest-app

## Clone the repo to rest-app workspace:

git clone https://github.com/95rade/Salary-API.git

## install

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

