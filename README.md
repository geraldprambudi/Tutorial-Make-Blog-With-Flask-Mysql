# Tutorial-Make-Blog-With-Flask-Mysql
Tutorial Make Blog With Flask and Mysql 

1. Install python
2. Install pip
3. Open cmd or terminal
4. Make project & move directories
5. Check phyton & pip
```
> python --version
Python 3.8.1
> pip --version
pip 19.2.3
```
6 Install environment virtualenv windows (Like Docker)
```
python3
example : python -m venv [projectName]
python -m venv virtualenv
```
7. Activate virtualenv Or Login environment virtualenv
```
Windows
example : [projectName]\Scripts\activate.bat
virtualenv\Scripts\activate.bat

WARNING : using backslash (\)

Mac & Linux
example : source [projectName]/bin/activate
source virtualenv/bin/activate

WARNING : using slash (/)
```
8. Check in virtualenv
```
pip list --format=columns
Result
Package    Version
---------- -------
pip        19.2.3
setuptools 41.2.0
```
9. Exit virtualenv
```
deactivate
```

10. create folder app
11. create file in folder app->__init__.py
```
from flask import Flask
app = Flask(__name__)
from app import routes
```

12. create file main.py 
```
from app import app
```

13. create file in folder app->routes.py
```
from app import app
@app.route('/')
@app.route('/index')
def index():
    return "hello world"
```


