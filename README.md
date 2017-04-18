# python.training.flight

# PreRequisites
- Code Editor
- GitHub
- Python

# Branches

## master
- Create a python project;
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
  - $ python -m venv myvenv
- Start the Python environment:
  - Windows
    - $ myvenv\Scripts\activate
  - Mac and Unix linke
    - $ source myvenv/bin/activate
- Update the PIP program (Python Index Package);
  - (myvenv)$ pip install --upgrade pip
- Install Python Django framework;
  - (myvenv)$ pip install django~=1.10.0
