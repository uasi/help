# Pipenv

## Initialize environment

```bash
$ pipenv --three # For Python 3
$ pipenv --two # For Python 2
# Will create Pipfile and ~/.local/share/virtualenvs/${dir}-${hash}/
```

## Manage packages

```bash
$ pipenv install foo bar
$ pipenv update foo bar
$ pipenv uninstall foo bar
# Will update Pipfile and Pipfile.lock
```

$ pipenv open foo
```bash
# Will open module dir in $EDITOR

## Manage environment
$ pipenv run foo_cmd
$ pipenv shell # Enter virtualenv
```

## Install pipenv

```bash
$ pip install pipenv
# Depending on your setup, pip may be pip3 or pip-3.6
```
