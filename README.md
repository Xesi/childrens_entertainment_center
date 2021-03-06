# childrens-entertainment-center
web-app with auth, sqlite, redis, mongoDB

---

## How to run

### install and activate Venv

```
$ apt install python3-venv
$ python3 -m venv env
$ source env/bin/activate
```
### install libs
```
$ pip install flask flask-sqlalchemy flask-login redis Pillow babel flask_pymongo
```

### init databases
```
$ python init_db.py

$ python -c "from childrens_entertainment_center import db, create_app, models; db.create_all(app=create_app())"
```

### run app!
```
$ export FLASK_APP=../childrens-entertainment-center
$ export FLASK_DEBUG=1

$ flask run 
```
