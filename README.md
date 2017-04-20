# python.training.flight

# PreRequisites
- Code Editor
- GitHub
- Python

# Branches

## master - Django installation
- Create a project folder;
- Setup the folder as a Git repository
  - $ git init
- Create the gitIgnore configuration file
  - New file: .gitignore
  - Enter the below content:
```
*.pyc
*.class
*.iml

*/.idea/**
.idea/misc.xml
.idea/modules.xml
.idea/vcs.xml
.idea/workspace.xml

__pycache__
myvenv
db.sqlite3
.DB_Store

```
- Create Python environment:
  - $ python3 -m venv myvenv
- Start the Python environment:
  - Windows
    - $ myvenv\Scripts\activate
  - Mac and Unix linke
    - $ source myvenv/bin/activate
- Update the PIP program (Python Index Package);
  - (myvenv)$ pip install --upgrade pip
- Install Python Django framework;
  - (myvenv)$ pip install django~=1.10.0

# project - create a Django project
- Create a project (do not forget the dot "." at the end)
  - (myvenv)$ django-admin startproject _myproject_ .
- Setup your project
  - File: _myproject_/settings.py
    - **TIME_ZONE** = 'America/Sao_Paulo'
  
    - **STATIC_URL** = '/static/'
    - **STATIC_ROOT** = os.path.join(BASE_DIR, 'static')
  
    - **ALLOWED_HOSTS** = ['127.0.0.1', '.pythonanywhere.com']
  
- Create the Data Base
  - (myvenv)$ python manage.py migrate
- Run the Web Server
  - (myvenv)$ python manage.py runserver
  
- Follow: [http://127.0.0.1:8000/](http://127.0.0.1:8000/)
  - You shall see **It Worked !**
