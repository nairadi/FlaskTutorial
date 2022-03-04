
# Learn Flask For Python - [YouTube](https://www.youtube.com/watch?v=Z1RJmh_OqeA)

## Overview
Basic scheduler app with tasks that you can add, delete or update hosted at https://fcc-flask-crud-app-tutorial.herokuapp.com/

## Flask App (Local Development):
_Setup:_
<br>
`pip install --user virtualenv`
<br>
`python -m virtualenv env`
<br>
`.\env\Scripts\activate`
<br>
`pip3 install flask flask-sqlalchemy`
<br>

_Run:_
<br>
`python .\app.py`
<br>
(should open in [localhost:5000](http://localhost:5000/))

## DB:
_Setup:_ after env is activated
<br>
`python - open python shell`
<br>
`from app import db`
<br>
`db.create_all()`
<br>

_Run:_
<br>
`python .\app.py`


## Generate Requirements
`pip3 freeze > requirements.txt`


## Heroku Deployment
create `Procfile` with `web: gunicorn app:app`
<br>
`heroku login`
<br>
`git init`
<br>
`git add .`
<br>
`git commit -m "Init app"`
<br>
`heroku create fcc-flask-crud-app-tutorial`
<br>
`git remote -v`
<br>
`git push heroku master`
<br>
should be deployed to [heroku](https://fcc-flask-crud-app-tutorial.herokuapp.com/)