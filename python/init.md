# Initialize my python development environment

Install [Python](https://www.python.org/)

## Welcome to PIP

[Python Packages Index](https://pypi.org/)

## Create a pipenv configuration

[How to install pipenv](https://pipenv.kennethreitz.org/en/latest/install/#installing-pipenv)

### Create a pipenv environement for my project (under windows)

```
md <projectdir>
pipenv --python 3.7
cd <virtualenv_path>
cd Scripts
copy *.bat \<projectdir>
cd \<projectdir>
activate
desactivate
```

### Installed !

We are now in the `\<projectdir>` directory
we `activate.bat` the pipenv configuration

We have the files :

- Pipfile
- Pipfile.lock
- activate.bat
- deactivate.bat

and the use of `pipenv` command line

### In VSCode

In VS Code, open the Command Palette (**View > Command Palette** or (Ctrl+Shift+P)). Then select the Python: **Select Interpreter command**

## If I want to do the same with Virtualenv (why not)

- https://docs.python-guide.org/dev/virtualenvs/
- https://medium.com/@Joachim8675309/python-virtualenv-c77e22bf5243

```
python -m venv _envmyname

copy _envmyname\scripts\activate.bat on.bat
copy _envmyname\scripts\deactivate.bat off.bat

activate
pip install <xyz>
deactivate

pip freeze > requirements.txt
pip install -r requirements.txt
```
